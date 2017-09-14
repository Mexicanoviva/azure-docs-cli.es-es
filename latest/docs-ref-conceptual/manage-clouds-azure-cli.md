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
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Administración de varias nubes con la CLI de Azure 2.0

Si tiene varias suscripciones asociadas a Azure, puede tener más de una nube disponible. Cada nube tiene sus propios puntos de conexión y funcionalidades asociados y, a menudo, está asociada a una región determinada que tiene normas o requisitos de protección de datos diferente.

Para poder trabajar eficazmente con varias nubes, debe poder cambiar entre las que están activas, y poder crear nubes nuevas.

## <a name="listing-clouds"></a>Listas de nubes

Puede enumerar las nubes disponibles con el comando [cloud list](/cli/azure/cloud#list). Esto le indicará qué nube está actualmente activa y cuál es su perfil actual, y puede proporcionar información sobre los nombres de host y los sufijos regionales.

Para obtener una lista de las nubes disponibles y la nube activa actualmente:

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

## <a name="switching-the-active-cloud"></a>Cambio de la nube activa

Para cambiar la nube actualmente activa, ejecute el comando [cloud set](/cli/azure/cloud#set). Este comando toma un argumento necesario, el nombre de la nube.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Si nunca se ha autenticado en la nube activa, debe hacerlo antes de realizar ninguna otra operación de la CLI. Para obtener instrucciones sobre la autenticación, consulte [Inicio de sesión con la CLI de Azure 2.0](/cli/azure/authenticate-azure-cli).

## <a name="register-or-unregister-a-cloud"></a>Registro o anulación del registro de una nube

Registro de una nube nueva si tiene sus propios puntos de conexión o necesita un perfil diferente. Las nubes se crean con el comando [cloud register](/cli/azure/cloud#register). Este comando requiere un nombre y, opcionalmente, un conjunto de funcionalidades y designaciones de puntos de conexión.

Para crear una nube con un punto de conexión especializado para el administrador de recursos, con un perfil específico:

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

Esto crea la nube, pero _no_ la selecciona automáticamente.

Si ya no necesita la nube creada, puede anular el registro con el comando [cloud unregister](/cli/azure/cloud#unregister):

```azurecli
az cloud unregister --name MyCloud
```

