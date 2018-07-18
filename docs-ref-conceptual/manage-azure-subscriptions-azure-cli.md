---
title: Administración de suscripciones de Azure con la CLI de Azure
description: Administre las suscripciones de Azure con la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/15/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: f5fdfba785d849b1fd4f5919870ec9c341bb9c7d
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967816"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="bfdde-103">Administración de varias suscripciones de Azure</span><span class="sxs-lookup"><span data-stu-id="bfdde-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="bfdde-104">La mayoría de los usuarios de Azure solo tendrán una suscripción.</span><span class="sxs-lookup"><span data-stu-id="bfdde-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="bfdde-105">Sin embargo, si forma parte de varias organizaciones o su organización ha dividido el acceso a determinados recursos mediante agrupaciones, habrá varias suscripciones dentro de Azure.</span><span class="sxs-lookup"><span data-stu-id="bfdde-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="bfdde-106">La CLI permite administrar varias suscripciones fácilmente, ya sea estableciendo una suscripción global para todos los comandos, o seleccionando una suscripción por comando.</span><span class="sxs-lookup"><span data-stu-id="bfdde-106">Multiple subscriptions can be easily managed with the CLI either by setting a global subscription for all commands, or selecting a subscription on a per-command basis.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="bfdde-107">Inquilinos, usuarios y suscripciones</span><span class="sxs-lookup"><span data-stu-id="bfdde-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="bfdde-108">Quizás no tenga muy clara la diferencia entre los inquilinos, los usuarios y las suscripciones de Azure.</span><span class="sxs-lookup"><span data-stu-id="bfdde-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="bfdde-109">Un _inquilino_ es la entidad de Azure Active Directory que abarca toda la organización.</span><span class="sxs-lookup"><span data-stu-id="bfdde-109">A _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="bfdde-110">Este inquilino tiene al menos una _suscripción_ y un _usuario_.</span><span class="sxs-lookup"><span data-stu-id="bfdde-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="bfdde-111">Un usuario es un individuo que está asociado a un único inquilino, la organización a la que pertenece.</span><span class="sxs-lookup"><span data-stu-id="bfdde-111">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="bfdde-112">Los usuarios son las cuentas que inician sesión en Azure para aprovisionar y usar los recursos.</span><span class="sxs-lookup"><span data-stu-id="bfdde-112">Users are those accounts which sign in to Azure to provision and use resources.</span></span>
<span data-ttu-id="bfdde-113">Un usuario puede tener acceso a varias _suscripciones_, que son los acuerdos con Microsoft para usar los servicios en la nube, incluido Azure.</span><span class="sxs-lookup"><span data-stu-id="bfdde-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="bfdde-114">Cada recurso está asociado a una suscripción.</span><span class="sxs-lookup"><span data-stu-id="bfdde-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="bfdde-115">Para más información sobre las diferencias entre inquilinos, usuarios y suscripciones, vea el [diccionario de terminología de la nube de Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="bfdde-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="bfdde-116">Para más información sobre cómo agregar una nueva suscripción a su inquilino de Azure Active Directory, consulte [Adición de una suscripción de Azure a Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="bfdde-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="bfdde-117">Si trabaja con varios inquilinos, debe iniciar sesión en un inquilino específico.</span><span class="sxs-lookup"><span data-stu-id="bfdde-117">When working with multiple tenants, you may need to sign in to a specific tenant.</span></span> <span data-ttu-id="bfdde-118">Para ello, consulte [Inicio de sesión con la CLI de Azure](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="bfdde-118">To do this, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="work-with-multiple-subscriptions"></a><span data-ttu-id="bfdde-119">Trabajo con varias suscripciones</span><span class="sxs-lookup"><span data-stu-id="bfdde-119">Work with multiple subscriptions</span></span>

<span data-ttu-id="bfdde-120">Para acceder a los recursos dentro de una suscripción, debe cambiar la suscripción activa.</span><span class="sxs-lookup"><span data-stu-id="bfdde-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="bfdde-121">Se puede cambiar la suscripción para todos los comandos de la CLI de Azure con [az account set](/cli/azure/account#az-account-set), o para cada comando con el argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="bfdde-121">Switching your subscription can be done for all Azure CLI commands with [az account set](/cli/azure/account#az-account-set), or done on a per-command basis by using the `--subscription` argument.</span></span>

<span data-ttu-id="bfdde-122">Para empezar, necesitará una lista de las suscripciones disponibles.</span><span class="sxs-lookup"><span data-stu-id="bfdde-122">To start, you will need a list of your available subscriptions.</span></span> <span data-ttu-id="bfdde-123">Para ello, use el comando [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="bfdde-123">To get it, use the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli-interactive
az account list --output table
```

<span data-ttu-id="bfdde-124">Para cambiar la suscripción activa globalmente, use `az account set` junto con el identificador o el nombre de la suscripción:</span><span class="sxs-lookup"><span data-stu-id="bfdde-124">To change the active subscription globally, use `az account set` along with either the subscription ID or subscription name:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="bfdde-125">Para usar una suscripción específica para un comando, use simplemente el argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="bfdde-125">To use a specific subscription for a command, just use the `--subscription` argument.</span></span> <span data-ttu-id="bfdde-126">Este argumento necesita un identificador o un nombre de suscripción:</span><span class="sxs-lookup"><span data-stu-id="bfdde-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
