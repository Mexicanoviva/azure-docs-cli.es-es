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
# <a name="select-clouds-with-the-azure-cli"></a>Selección de nubes con la CLI de Azure

Si trabaja en diferentes regiones o usa [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), puede que necesite utilizar más de una nube. Microsoft pone a su disposición nubes para el cumplimiento de las leyes locales. En este artículo se muestra cómo obtener información sobre las nubes, cómo cambiar la nube actual y cómo registrar o anular el registro de nuevas nubes.

## <a name="list-available-clouds"></a>Lista de las nubes disponibles

Para enumerar las nubes disponibles, use el comando [az cloud list](/cli/azure/cloud#az-cloud-list). Este comando muestra qué nube está actualmente activa y cuál es su perfil actual, así como información sobre los nombres de host y los sufijos regionales.

Para obtener la nube activa y una lista de todas las nubes disponibles:

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

La nube actualmente activa tiene `True` en la columna `IsActive`. Solo puede haber una nube activa en un momento dado. Para obtener información más detallada acerca de una nube, incluidos los puntos de conexión que usa para los servicios de Azure, use el comando `cloud show`:

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

## <a name="switch-the-active-cloud"></a>Cambio de la nube activa

Para establecer la nube predeterminada mediante un archivo de configuración, consulte [Valores de configuración de la CLI y variables de entorno](/cli/azure/azure-cli-configuration?view=azure-cli-latest#cli-configuration-values-and-environment-variables).  Para cambiar la nube activa, ejecute el comando [az cloud set](/cli/azure/cloud#az-cloud-set). Este comando toma un argumento necesario, el nombre de la nube.

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Si la autenticación de la nube activada ha expirado, debe volver a autenticarse antes de realizar otras tareas con la CLI. Si es la primera vez que cambia a la nueva nube, debe establecer la suscripción activa.
> Para obtener instrucciones sobre la autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md). Para más información sobre la administración de suscripciones, consulte [Administración de suscripciones de Azure con la CLI de Azure](manage-azure-subscriptions-azure-cli.md)

## <a name="register-a-new-cloud"></a>Registro de una nube nueva

Registre una nube nueva si tiene sus propios puntos de conexión para Azure Stack. Las nubes se crean con el comando [az cloud register](/cli/azure/cloud#az-cloud-register). Este comando requiere un nombre y un conjunto de puntos de conexión de servicio. Para más información sobre cómo registrar una nube para usarla con Azure Stack, consulte [Uso de los perfiles de la versión de la API con la CLI de Azure en Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).

No es necesario registrar la información para las regiones de China, Gobierno de EE. UU. o Alemania. Microsoft administra estas nubes y están disponibles de forma predeterminada.  Para más información sobre la configuración de todos los puntos de conexión disponibles, consulte la [documentación de `az cloud register`](/cli/azure/cloud#az-cloud-register).

Al registrar una nube no se cambia automáticamente a ella. Use el comando `az cloud set` para seleccionar la nube recién creada.

## <a name="update-an-existing-cloud"></a>Actualización de una nube existente

Si tiene permisos, también puede actualizar una nube existente. Al actualizar una nube se cambia a un perfil de servicios de Azure diferente o modifica los puntos de conexión.
Actualice una nube con el comando [az cloud update](/cli/azure/cloud#az-cloud-update), que toma los mismos argumentos que `az cloud register`.

## <a name="unregister-a-cloud"></a>Anulación del registro de una nube

Si ya no necesita la nube creada, puede anular el registro con el comando [cloud unregister](/cli/azure/cloud#az-cloud-unregister):

```azurecli-interactive
az cloud unregister --name MyCloud
```
