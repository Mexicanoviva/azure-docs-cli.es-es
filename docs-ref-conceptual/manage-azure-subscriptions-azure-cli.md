---
title: Administración de suscripciones de Azure con la CLI de Azure
description: Administre las suscripciones de Azure con la CLI de Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: dad217dff159baa39bd1361258fb308eea872564
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/28/2020
ms.locfileid: "77780067"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="a7776-103">Uso de varias suscripciones de Azure</span><span class="sxs-lookup"><span data-stu-id="a7776-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="a7776-104">La mayoría de los usuarios de Azure solo tendrán una suscripción.</span><span class="sxs-lookup"><span data-stu-id="a7776-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="a7776-105">Sin embargo, si forma parte de varias organizaciones o su organización ha dividido el acceso a determinados recursos mediante agrupaciones, habrá varias suscripciones dentro de Azure.</span><span class="sxs-lookup"><span data-stu-id="a7776-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="a7776-106">La CLI admite la selección de una suscripción global y por comando.</span><span class="sxs-lookup"><span data-stu-id="a7776-106">The CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="a7776-107">Para obtener información detallada sobre las suscripciones, facturación y administración de costos, consulte la [documentación sobre administración de costos y facturación](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="a7776-107">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="a7776-108">Inquilinos, usuarios y suscripciones</span><span class="sxs-lookup"><span data-stu-id="a7776-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="a7776-109">Quizás no tenga muy clara la diferencia entre los inquilinos, los usuarios y las suscripciones de Azure.</span><span class="sxs-lookup"><span data-stu-id="a7776-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="a7776-110">Un _inquilino_ es la entidad de Azure Active Directory que abarca toda la organización.</span><span class="sxs-lookup"><span data-stu-id="a7776-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="a7776-111">Este inquilino tiene al menos una _suscripción_ y un _usuario_.</span><span class="sxs-lookup"><span data-stu-id="a7776-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="a7776-112">Un usuario es un individuo que está asociado a un único inquilino, la organización a la que pertenece.</span><span class="sxs-lookup"><span data-stu-id="a7776-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="a7776-113">Los usuarios son las cuentas que inician sesión en Azure para crear, administrar y usar los recursos.</span><span class="sxs-lookup"><span data-stu-id="a7776-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="a7776-114">Un usuario puede tener acceso a varias _suscripciones_, que son los acuerdos con Microsoft para usar los servicios en la nube, incluido Azure.</span><span class="sxs-lookup"><span data-stu-id="a7776-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="a7776-115">Cada recurso está asociado a una suscripción.</span><span class="sxs-lookup"><span data-stu-id="a7776-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="a7776-116">Para más información sobre las diferencias entre inquilinos, usuarios y suscripciones, vea el [diccionario de terminología de la nube de Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="a7776-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="a7776-117">Para más información sobre cómo agregar una nueva suscripción a su inquilino de Azure Active Directory, consulte [Adición de una suscripción de Azure a Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="a7776-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="a7776-118">Para más información sobre cómo iniciar sesión un inquilino específico, consulte [Inicio de sesión con la CLI de Azure](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="a7776-118">To learn how to sign in to a specific tenant, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="a7776-119">Cambio de la suscripción activa</span><span class="sxs-lookup"><span data-stu-id="a7776-119">Change the active subscription</span></span>

<span data-ttu-id="a7776-120">Para acceder a los recursos dentro de una suscripción, cambie la suscripción activa o use el argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="a7776-120">To access the resources for a subscription, switch your active subscription or use the `--subscription` argument.</span></span> <span data-ttu-id="a7776-121">Para cambiar la suscripción para todos los comandos, se usa [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="a7776-121">Switching your subscription for all commands is done with [az account set](/cli/azure/account#az-account-set).</span></span>

<span data-ttu-id="a7776-122">Para cambiar su suscripción activa:</span><span class="sxs-lookup"><span data-stu-id="a7776-122">To switch your active subscription:</span></span>

1. <span data-ttu-id="a7776-123">Obtenga la lista de suscripciones con el comando [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="a7776-123">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

    ```azurecli-interactive
    az account list --output table
    ```
2. <span data-ttu-id="a7776-124">Use `az account set` con el identificador de suscripción o el nombre al que desee cambiar.</span><span class="sxs-lookup"><span data-stu-id="a7776-124">Use `az account set` with the subscription ID or name you want to switch to.</span></span>

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

<span data-ttu-id="a7776-125">Para ejecutar solo un comando con una suscripción diferente, use el argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="a7776-125">To run only a single command with a different subscription, use the `--subscription` argument.</span></span> <span data-ttu-id="a7776-126">Este argumento necesita un identificador o un nombre de suscripción:</span><span class="sxs-lookup"><span data-stu-id="a7776-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
