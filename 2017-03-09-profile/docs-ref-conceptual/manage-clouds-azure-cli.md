---
title: "Administración de varias nubes con la CLI de Azure 2.0"
description: "Cree, inicie sesión y administre diferentes nubes con la CLI de Azure 2.0."
keywords: "CLI de Azure 2.0, Azure, nubes, centros de datos, gobierno, región, china, alemania"
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="4406e-104">Administración de varias nubes con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="4406e-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="4406e-105">Si tiene varias suscripciones asociadas a Azure, puede tener más de una nube disponible.</span><span class="sxs-lookup"><span data-stu-id="4406e-105">If you have multiple subscriptions associated with Azure, you may have more than one cloud available.</span></span> <span data-ttu-id="4406e-106">Cada nube tiene sus propios puntos de conexión y funcionalidades asociados y, a menudo, está asociada a una región determinada que tiene normas o requisitos de protección de datos diferente.</span><span class="sxs-lookup"><span data-stu-id="4406e-106">Each cloud has its own associated endpoints and capabilities, and is often associated with a particular region that has different data protection standards or requirements.</span></span>

<span data-ttu-id="4406e-107">Para poder trabajar eficazmente con varias nubes, debe poder cambiar entre las que están activas, y poder crear nubes nuevas.</span><span class="sxs-lookup"><span data-stu-id="4406e-107">To effectively work with multiple clouds, you will need to be able to switch between which is currently active, and possibly create new clouds.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="4406e-108">Listas de nubes</span><span class="sxs-lookup"><span data-stu-id="4406e-108">Listing clouds</span></span>

<span data-ttu-id="4406e-109">Puede enumerar las nubes disponibles con el comando [cloud list](/cli/azure/cloud#list).</span><span class="sxs-lookup"><span data-stu-id="4406e-109">You may list your available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="4406e-110">Esto le indicará qué nube está actualmente activa y cuál es su perfil actual, y puede proporcionar información sobre los nombres de host y los sufijos regionales.</span><span class="sxs-lookup"><span data-stu-id="4406e-110">This will tell you which cloud is currently active, what its current profile is, and can provide information on regional suffixes and host names.</span></span>

<span data-ttu-id="4406e-111">Para obtener una lista de las nubes disponibles y la nube activa actualmente:</span><span class="sxs-lookup"><span data-stu-id="4406e-111">To get a list of the available clouds and the currently active one:</span></span>

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

## <a name="switching-the-active-cloud"></a><span data-ttu-id="4406e-112">Cambio de la nube activa</span><span class="sxs-lookup"><span data-stu-id="4406e-112">Switching the active cloud</span></span>

<span data-ttu-id="4406e-113">Para cambiar la nube actualmente activa, ejecute el comando [cloud set](/cli/azure/cloud#set).</span><span class="sxs-lookup"><span data-stu-id="4406e-113">In order to switch the currently active cloud, you run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="4406e-114">Este comando toma un argumento necesario, el nombre de la nube.</span><span class="sxs-lookup"><span data-stu-id="4406e-114">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="4406e-115">Si nunca se ha autenticado en la nube activa, debe hacerlo antes de realizar ninguna otra operación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="4406e-115">If you have never authenticated for the active cloud, you will need to do so before performing any other CLI operations.</span></span> <span data-ttu-id="4406e-116">Para obtener instrucciones sobre la autenticación, consulte [Inicio de sesión con la CLI de Azure 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="4406e-116">For instructions on authenticating, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="register-or-unregister-a-cloud"></a><span data-ttu-id="4406e-117">Registro o anulación del registro de una nube</span><span class="sxs-lookup"><span data-stu-id="4406e-117">Register or unregister a cloud</span></span>

<span data-ttu-id="4406e-118">Registro de una nube nueva si tiene sus propios puntos de conexión o necesita un perfil diferente.</span><span class="sxs-lookup"><span data-stu-id="4406e-118">Register a new cloud if you have your own endpoints or require a different profile.</span></span> <span data-ttu-id="4406e-119">Las nubes se crean con el comando [cloud register](/cli/azure/cloud#register).</span><span class="sxs-lookup"><span data-stu-id="4406e-119">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="4406e-120">Este comando requiere un nombre y, opcionalmente, un conjunto de funcionalidades y designaciones de puntos de conexión.</span><span class="sxs-lookup"><span data-stu-id="4406e-120">This command requires a name, and optionally a set of capabilities and endpoint designations.</span></span>

<span data-ttu-id="4406e-121">Para crear una nube con un punto de conexión especializado para el administrador de recursos, con un perfil específico:</span><span class="sxs-lookup"><span data-stu-id="4406e-121">To create a cloud with a specialized endpoint for the resource manager, with a specific profile:</span></span>

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

<span data-ttu-id="4406e-122">Esto crea la nube, pero _no_ la selecciona automáticamente.</span><span class="sxs-lookup"><span data-stu-id="4406e-122">This creates the cloud, but does _not_ automatically select it.</span></span>

<span data-ttu-id="4406e-123">Si ya no necesita la nube creada, puede anular el registro con el comando [cloud unregister](/cli/azure/cloud#unregister):</span><span class="sxs-lookup"><span data-stu-id="4406e-123">If you no longer require the created cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```

