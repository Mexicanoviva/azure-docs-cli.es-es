---
title: Administración de varias nubes con la CLI de Azure 2.0
description: Cree, inicie sesión y administre varias nubes con la CLI de Azure 2.0.
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: c17506cc81adc859ff5778b109c1832c857764e6
ms.sourcegitcommit: c9da729f4a42a839f13106f7589deaa0ca19cc4e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/06/2018
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Administración de varias nubes con la CLI de Azure 2.0

Si trabaja en diferentes regiones o usa [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), puede que necesite utilizar más de una nube. Microsoft pone a su disposición nubes para el cumplimiento de las leyes locales. En este artículo se muestra cómo obtener información sobre las nubes disponibles para su cuenta, cómo cambiar la nube actual y cómo registrar o anular el registro de nuevas nubes para su uso con Azure Stack.

## <a name="listing-clouds"></a>Listas de nubes

Para enumerar las nubes disponibles, use el comando [az cloud list](/cli/azure/cloud#az-cloud-list). Le indicará qué nube está actualmente activa y cuál es su perfil actual, así como información sobre los nombres de host y los sufijos regionales.

Para obtener la nube activa y una lista de todas las nubes disponibles:

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

La nube actualmente activa tiene `True` en la columna `IsActive`. Solo puede haber una nube activa en un momento dado. Para obtener información más detallada acerca de una nube, incluidos los puntos de conexión que usa para los servicios de Azure, use el comando `cloud show`:

```azurecli
az cloud show --name AzureChinaCloud --output json
```

```output
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

## <a name="switching-the-active-cloud"></a>Cambio de la nube activa

Para cambiar la nube actualmente activa, ejecute el comando [az cloud set](/cli/azure/cloud#az-cloud-set). Este comando toma un argumento necesario, el nombre de la nube.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Si la autenticación de la nube activada ha expirado, debe volver a autenticarse antes de realizar otras tareas con la CLI. Si es la primera vez que cambia a la nueva nube, debe establecer la suscripción activa.
> Para obtener instrucciones sobre la autenticación, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md). Para más información sobre la administración de suscripciones, vea [Administración de suscripciones de Azure con la CLI de Azure 2.0](manage-azure-subscriptions-azure-cli.md)

## <a name="register-a-cloud"></a>Registro de una nube

Registre una nube nueva si tiene sus propios puntos de conexión para Azure Stack. Las nubes se crean con el comando [az cloud register](/cli/azure/cloud#az-cloud-register). Este comando requiere un nombre y un conjunto de funcionalidades con puntos de conexión asociados. Para más información sobre cómo registrar una nube para su uso con Azure Stack, consulte [Instalación y configuración de la CLI para su uso con Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).

No es necesario registrar su propia nube para las regiones de China, Gobierno de EE. UU. o Alemania. Microsoft las administra y están disponibles de forma predeterminada.  Para más información sobre la configuración de todos los puntos de conexión disponibles, consulte la [documentación de `az cloud register`](/cli/azure/cloud#az-cloud-register).

Al registrar una nube no se cambia automáticamente a ella. Use el comando `az cloud set` para seleccionar la nube recién creada, tal y como se describió anteriormente.

## <a name="update-an-existing-cloud"></a>Actualización de una nube existente

Si tiene permisos, también puede actualizar una nube existente. Hágalo cuando necesita cambiar a un perfil de Azure diferente o para agregar o cambiar un punto de conexión.
Para ello, se usa el comando [az cloud update](/cli/azure/cloud#az-cloud-update), que tiene los mismos argumentos que `az cloud register`.

## <a name="unregister-a-cloud"></a>Anulación del registro de una nube

Si ya no necesita una nube registrada, puede anular el registro con el comando [az cloud unregister](/cli/azure/cloud#az-cloud-unregister):

```azurecli
az cloud unregister --name MyCloud
```
