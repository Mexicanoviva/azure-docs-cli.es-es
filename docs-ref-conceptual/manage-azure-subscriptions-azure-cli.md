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
# <a name="manage-multiple-azure-subscriptions"></a>Administración de varias suscripciones de Azure

La mayoría de los usuarios de Azure solo tendrán una suscripción. Sin embargo, si forma parte de varias organizaciones o su organización ha dividido el acceso a determinados recursos mediante agrupaciones, habrá varias suscripciones dentro de Azure. La CLI permite administrar varias suscripciones fácilmente, ya sea estableciendo una suscripción global para todos los comandos, o seleccionando una suscripción por comando.

## <a name="tenants-users-and-subscriptions"></a>Inquilinos, usuarios y suscripciones

Quizás no tenga muy clara la diferencia entre los inquilinos, los usuarios y las suscripciones de Azure. Un _inquilino_ es la entidad de Azure Active Directory que abarca toda la organización. Este inquilino tiene al menos una _suscripción_ y un _usuario_. Un usuario es un individuo que está asociado a un único inquilino, la organización a la que pertenece. Los usuarios son las cuentas que inician sesión en Azure para aprovisionar y usar los recursos.
Un usuario puede tener acceso a varias _suscripciones_, que son los acuerdos con Microsoft para usar los servicios en la nube, incluido Azure. Cada recurso está asociado a una suscripción.

Para más información sobre las diferencias entre inquilinos, usuarios y suscripciones, vea el [diccionario de terminología de la nube de Azure](/azure/azure-glossary-cloud-terminology).  Para más información sobre cómo agregar una nueva suscripción a su inquilino de Azure Active Directory, consulte [Adición de una suscripción de Azure a Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Si trabaja con varios inquilinos, debe iniciar sesión en un inquilino específico. Para ello, consulte [Inicio de sesión con la CLI de Azure](/cli/azure/authenticate-azure-cli).

## <a name="work-with-multiple-subscriptions"></a>Trabajo con varias suscripciones

Para acceder a los recursos dentro de una suscripción, debe cambiar la suscripción activa. Se puede cambiar la suscripción para todos los comandos de la CLI de Azure con [az account set](/cli/azure/account#az-account-set), o para cada comando con el argumento `--subscription`.

Para empezar, necesitará una lista de las suscripciones disponibles. Para ello, use el comando [az account list](/cli/azure/account#az-account-list):

```azurecli-interactive
az account list --output table
```

Para cambiar la suscripción activa globalmente, use `az account set` junto con el identificador o el nombre de la suscripción:

```azurecli-interactive
az account set --subscription "My Demos"
```

Para usar una suscripción específica para un comando, use simplemente el argumento `--subscription`. Este argumento necesita un identificador o un nombre de suscripción:

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
