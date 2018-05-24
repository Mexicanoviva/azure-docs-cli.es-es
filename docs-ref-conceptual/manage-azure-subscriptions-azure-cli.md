---
title: Administración de suscripciones de Azure con la CLI de Azure 2.0
description: Administración de suscripciones de Azure con la CLI de Azure 2.0 en Linux, Mac o Windows.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: ee7e0ca03b1ed9c1bfc040fd5714bb9b3549e3cd
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/18/2018
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="42b2a-103">Administración de varias suscripciones de Azure</span><span class="sxs-lookup"><span data-stu-id="42b2a-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="42b2a-104">La mayoría de los usuarios de Azure solo tendrán una suscripción.</span><span class="sxs-lookup"><span data-stu-id="42b2a-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="42b2a-105">Sin embargo, si forma parte de varias organizaciones o su organización ha dividido el acceso a determinados recursos mediante agrupaciones, habrá varias suscripciones dentro de Azure.</span><span class="sxs-lookup"><span data-stu-id="42b2a-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="42b2a-106">Las distintas suscripciones se pueden administrar fácilmente con la CLI y, para realizar las operaciones, solo tiene que seleccionar una suscripción.</span><span class="sxs-lookup"><span data-stu-id="42b2a-106">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="42b2a-107">Inquilinos, usuarios y suscripciones</span><span class="sxs-lookup"><span data-stu-id="42b2a-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="42b2a-108">Quizás no tenga muy clara la diferencia entre los inquilinos, los usuarios y las suscripciones de Azure.</span><span class="sxs-lookup"><span data-stu-id="42b2a-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="42b2a-109">Por lo general, un _inquilino_ es la entidad de Azure Active Directory que abarca toda la organización.</span><span class="sxs-lookup"><span data-stu-id="42b2a-109">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="42b2a-110">Este inquilino tiene al menos una _suscripción_ y un _usuario_.</span><span class="sxs-lookup"><span data-stu-id="42b2a-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="42b2a-111">Un usuario es un individuo que está asociado a un único inquilino, la organización a la que pertenece.</span><span class="sxs-lookup"><span data-stu-id="42b2a-111">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="42b2a-112">Los usuarios son las cuentas que inician sesión en Azure para aprovisionar y usar los recursos.</span><span class="sxs-lookup"><span data-stu-id="42b2a-112">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="42b2a-113">Un usuario puede tener acceso a varias _suscripciones_, que son los acuerdos con Microsoft para usar los servicios en la nube, incluido Azure.</span><span class="sxs-lookup"><span data-stu-id="42b2a-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="42b2a-114">Cada recurso está asociado a una suscripción.</span><span class="sxs-lookup"><span data-stu-id="42b2a-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="42b2a-115">Para más información sobre las diferencias entre inquilinos, usuarios y suscripciones, vea el [diccionario de terminología de la nube de Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="42b2a-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="42b2a-116">Para más información sobre cómo agregar una nueva suscripción a su inquilino de Azure Active Directory, consulte [Adición de una suscripción de Azure a Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="42b2a-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="42b2a-117">Si trabaja con varios inquilinos, debe iniciar sesión en un inquilino específico.</span><span class="sxs-lookup"><span data-stu-id="42b2a-117">When working with multiple tenants, you may need to log into a specific tenant.</span></span> <span data-ttu-id="42b2a-118">Para ello, consulte [Inicio de sesión con la CLI de Azure 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="42b2a-118">To do this, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="42b2a-119">Trabajo con varias suscripciones</span><span class="sxs-lookup"><span data-stu-id="42b2a-119">Working with multiple subscriptions</span></span>

<span data-ttu-id="42b2a-120">Para acceder a los recursos dentro de una suscripción, debe cambiar la suscripción activa.</span><span class="sxs-lookup"><span data-stu-id="42b2a-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="42b2a-121">Todo el trabajo con las suscripciones se realiza mediante el comando `az account`, que hace referencia al acuerdo de servicio que representa una suscripción, y no la cuenta individual.</span><span class="sxs-lookup"><span data-stu-id="42b2a-121">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="42b2a-122">Para empezar a trabajar con las suscripciones disponibles, obtenga una lista de las suscripciones disponibles en su cuenta:</span><span class="sxs-lookup"><span data-stu-id="42b2a-122">To start working with your available subscriptions, get a list of those available in your account:</span></span>

```azurecli-interactive
az account list --output table
```

```Output
Name                                         CloudName    SubscriptionId                        State     IsDefault
-------------------------------------------  -----------  ------------------------------------  --------  -----------
My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
```

<span data-ttu-id="42b2a-123">Para cambiar la suscripción activa, puede utilizar `az account set`:</span><span class="sxs-lookup"><span data-stu-id="42b2a-123">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="42b2a-124">Para seleccionar la suscripción, puede usar el nombre o el identificador de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="42b2a-124">You can use either the subscription ID or the subscription name to select the subscription.</span></span>
