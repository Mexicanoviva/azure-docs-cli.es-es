---
title: Selección de nubes con la CLI de Azure
description: Cree, inicie sesión y administre varias nubes con la CLI de Azure.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f102414b9539c9f8ad7d088c2ddf802583c22721
ms.sourcegitcommit: 503cf343422ab8d2a587d2ccb795953b8ad66376
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/31/2019
ms.locfileid: "75559616"
---
# <a name="select-clouds-with-the-azure-cli"></a><span data-ttu-id="3c508-103">Selección de nubes con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="3c508-103">Select clouds with the Azure CLI</span></span>

<span data-ttu-id="3c508-104">Si trabaja en diferentes regiones o usa [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), puede que necesite utilizar más de una nube.</span><span class="sxs-lookup"><span data-stu-id="3c508-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="3c508-105">Microsoft pone a su disposición nubes para el cumplimiento de las leyes locales.</span><span class="sxs-lookup"><span data-stu-id="3c508-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="3c508-106">En este artículo se muestra cómo obtener información sobre las nubes, cómo cambiar la nube actual y cómo registrar o anular el registro de nuevas nubes.</span><span class="sxs-lookup"><span data-stu-id="3c508-106">This article shows you how to get information on clouds, change the current cloud, and register or unregister new clouds.</span></span>

## <a name="list-available-clouds"></a><span data-ttu-id="3c508-107">Lista de las nubes disponibles</span><span class="sxs-lookup"><span data-stu-id="3c508-107">List available clouds</span></span>

<span data-ttu-id="3c508-108">Para enumerar las nubes disponibles, use el comando [az cloud list](/cli/azure/cloud#az-cloud-list).</span><span class="sxs-lookup"><span data-stu-id="3c508-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="3c508-109">Este comando muestra qué nube está actualmente activa y cuál es su perfil actual, así como información sobre los nombres de host y los sufijos regionales.</span><span class="sxs-lookup"><span data-stu-id="3c508-109">This command shows which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="3c508-110">Para obtener la nube activa y una lista de todas las nubes disponibles:</span><span class="sxs-lookup"><span data-stu-id="3c508-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli-interactive
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

<span data-ttu-id="3c508-111">La nube actualmente activa tiene `True` en la columna `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="3c508-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="3c508-112">Solo puede haber una nube activa en un momento dado.</span><span class="sxs-lookup"><span data-stu-id="3c508-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="3c508-113">Para obtener información más detallada acerca de una nube, incluidos los puntos de conexión que usa para los servicios de Azure, use el comando `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="3c508-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```json
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switch-the-active-cloud"></a><span data-ttu-id="3c508-114">Cambio de la nube activa</span><span class="sxs-lookup"><span data-stu-id="3c508-114">Switch the active cloud</span></span>

<span data-ttu-id="3c508-115">Para establecer la nube predeterminada mediante un archivo de configuración, consulte [Valores de configuración de la CLI y variables de entorno](/cli/azure/azure-cli-configuration?view=azure-cli-latest#cli-configuration-values-and-environment-variables).</span><span class="sxs-lookup"><span data-stu-id="3c508-115">To set the default cloud using a configuration file, see [CLI configuration values and environment variables](/cli/azure/azure-cli-configuration?view=azure-cli-latest#cli-configuration-values-and-environment-variables).</span></span>  <span data-ttu-id="3c508-116">Para cambiar la nube activa, ejecute el comando [az cloud set](/cli/azure/cloud#az-cloud-set).</span><span class="sxs-lookup"><span data-stu-id="3c508-116">To switch the active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="3c508-117">Este comando toma un argumento necesario, el nombre de la nube.</span><span class="sxs-lookup"><span data-stu-id="3c508-117">This command takes one required argument, the name of the cloud.</span></span>

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="3c508-118">Si la autenticación de la nube activada ha expirado, debe volver a autenticarse antes de realizar otras tareas con la CLI.</span><span class="sxs-lookup"><span data-stu-id="3c508-118">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="3c508-119">Si es la primera vez que cambia a la nueva nube, debe establecer la suscripción activa.</span><span class="sxs-lookup"><span data-stu-id="3c508-119">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="3c508-120">Para obtener instrucciones sobre la autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="3c508-120">For instructions on authenticating, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span> <span data-ttu-id="3c508-121">Para más información sobre la administración de suscripciones, consulte [Administración de suscripciones de Azure con la CLI de Azure](manage-azure-subscriptions-azure-cli.md)</span><span class="sxs-lookup"><span data-stu-id="3c508-121">For information on subscription management, see [Manage Azure subscriptions with Azure CLI](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-new-cloud"></a><span data-ttu-id="3c508-122">Registro de una nube nueva</span><span class="sxs-lookup"><span data-stu-id="3c508-122">Register a new cloud</span></span>

<span data-ttu-id="3c508-123">Registre una nube nueva si tiene sus propios puntos de conexión para Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3c508-123">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="3c508-124">Las nubes se crean con el comando [az cloud register](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="3c508-124">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="3c508-125">Este comando requiere un nombre y un conjunto de puntos de conexión de servicio.</span><span class="sxs-lookup"><span data-stu-id="3c508-125">This command requires a name and a set of service endpoints.</span></span> <span data-ttu-id="3c508-126">Para más información sobre cómo registrar una nube para usarla con Azure Stack, consulte [Uso de los perfiles de la versión de la API con la CLI de Azure en Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="3c508-126">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="3c508-127">No es necesario registrar la información para las regiones de China, Gobierno de EE. UU. o Alemania.</span><span class="sxs-lookup"><span data-stu-id="3c508-127">You don't need to register information for the China, US Government, or German regions.</span></span> <span data-ttu-id="3c508-128">Microsoft administra estas nubes y están disponibles de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3c508-128">These clouds are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="3c508-129">Para más información sobre la configuración de todos los puntos de conexión disponibles, consulte la [documentación de `az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="3c508-129">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="3c508-130">Al registrar una nube no se cambia automáticamente a ella.</span><span class="sxs-lookup"><span data-stu-id="3c508-130">Registering a cloud doesn't automatically switch to it.</span></span> <span data-ttu-id="3c508-131">Use el comando `az cloud set` para seleccionar la nube recién creada.</span><span class="sxs-lookup"><span data-stu-id="3c508-131">Use the `az cloud set` command to select the newly created cloud.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="3c508-132">Actualización de una nube existente</span><span class="sxs-lookup"><span data-stu-id="3c508-132">Update an existing cloud</span></span>

<span data-ttu-id="3c508-133">Si tiene permisos, también puede actualizar una nube existente.</span><span class="sxs-lookup"><span data-stu-id="3c508-133">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="3c508-134">Al actualizar una nube se cambia a un perfil de servicios de Azure diferente o modifica los puntos de conexión.</span><span class="sxs-lookup"><span data-stu-id="3c508-134">Updating a cloud switches to a different Azure services profile or modifies the connection endpoints.</span></span>
<span data-ttu-id="3c508-135">Actualice una nube con el comando [az cloud update](/cli/azure/cloud#az-cloud-update), que toma los mismos argumentos que `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="3c508-135">Update a cloud with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="3c508-136">Anulación del registro de una nube</span><span class="sxs-lookup"><span data-stu-id="3c508-136">Unregister a cloud</span></span>

<span data-ttu-id="3c508-137">Si ya no necesita la nube creada, puede anular el registro con el comando [cloud unregister](/cli/azure/cloud#az-cloud-unregister):</span><span class="sxs-lookup"><span data-stu-id="3c508-137">If you no longer need a created cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli-interactive
az cloud unregister --name MyCloud
```
