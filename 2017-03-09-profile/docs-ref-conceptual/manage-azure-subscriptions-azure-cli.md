---
title: "Administración de suscripciones de Azure con la CLI de Azure 2.0"
description: "Administración de suscripciones de Azure con la CLI de Azure 2.0 en Linux, Mac o Windows."
keywords: "CLI de Azure 2.0, Linux, Mac, Windows, OS X, suscripción"
author: kamaljit
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: 0f453ad1bff621250c8aa3147b5f5e916e712e30
ms.sourcegitcommit: 16426a08c0f2f62d0b9dca3df8132cece659acff
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2017
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="5910f-104">Administración de varias suscripciones de Azure</span><span class="sxs-lookup"><span data-stu-id="5910f-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="5910f-105">La mayoría de los usuarios de Azure solo tendrán una suscripción.</span><span class="sxs-lookup"><span data-stu-id="5910f-105">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="5910f-106">Sin embargo, si forma parte de varias organizaciones o su organización ha dividido el acceso a determinados recursos mediante agrupaciones, habrá varias suscripciones dentro de Azure.</span><span class="sxs-lookup"><span data-stu-id="5910f-106">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="5910f-107">Las distintas suscripciones se pueden administrar fácilmente con la CLI y, para realizar las operaciones, solo tiene que seleccionar una suscripción.</span><span class="sxs-lookup"><span data-stu-id="5910f-107">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="5910f-108">Inquilinos, usuarios y suscripciones</span><span class="sxs-lookup"><span data-stu-id="5910f-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="5910f-109">Quizás no tenga muy clara la diferencia entre los inquilinos, los usuarios y las suscripciones de Azure.</span><span class="sxs-lookup"><span data-stu-id="5910f-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="5910f-110">Por lo general, un _inquilino_ es la entidad de Azure Active Directory que abarca toda la organización.</span><span class="sxs-lookup"><span data-stu-id="5910f-110">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="5910f-111">Este inquilino tiene al menos una _suscripción_ y un _usuario_.</span><span class="sxs-lookup"><span data-stu-id="5910f-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="5910f-112">Un usuario es un individuo que está asociado a un único inquilino, la organización a la que pertenece.</span><span class="sxs-lookup"><span data-stu-id="5910f-112">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="5910f-113">Los usuarios son las cuentas que inician sesión en Azure para aprovisionar y usar los recursos.</span><span class="sxs-lookup"><span data-stu-id="5910f-113">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="5910f-114">Un usuario puede tener acceso a varias _suscripciones_, que son los acuerdos con Microsoft para usar los servicios en la nube, incluido Azure.</span><span class="sxs-lookup"><span data-stu-id="5910f-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="5910f-115">Cada recurso está asociado a una suscripción.</span><span class="sxs-lookup"><span data-stu-id="5910f-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="5910f-116">Para más información sobre las diferencias entre inquilinos, usuarios y suscripciones, vea el [diccionario de terminología de la nube de Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="5910f-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="5910f-117">Para más información sobre cómo agregar una nueva suscripción a su inquilino de Azure Active Directory, consulte [Adición de una suscripción de Azure a Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="5910f-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="5910f-118">Trabajo con varias suscripciones</span><span class="sxs-lookup"><span data-stu-id="5910f-118">Working with multiple subscriptions</span></span>

<span data-ttu-id="5910f-119">Para acceder a los recursos dentro de una suscripción, debe cambiar la suscripción activa.</span><span class="sxs-lookup"><span data-stu-id="5910f-119">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="5910f-120">Todo el trabajo con las suscripciones se realiza mediante el comando `az account`, que hace referencia al acuerdo de servicio que representa una suscripción, y no la cuenta individual.</span><span class="sxs-lookup"><span data-stu-id="5910f-120">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="5910f-121">Para empezar a trabajar con las suscripciones disponibles, obtenga una lista de las suscripciones disponibles en su cuenta:</span><span class="sxs-lookup"><span data-stu-id="5910f-121">To start working with your available subscriptions, get a list of those available in your account:</span></span>

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

<span data-ttu-id="5910f-122">Para cambiar la suscripción activa, puede utilizar `az account set`:</span><span class="sxs-lookup"><span data-stu-id="5910f-122">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="5910f-123">Para seleccionar la suscripción, puede usar el nombre o el identificador de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="5910f-123">You can use either the subscription ID or the subscription name to select the subscription.</span></span>
