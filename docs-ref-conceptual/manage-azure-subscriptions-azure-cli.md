---
title: "Administración de suscripciones de Azure con la CLI de Azure 2.0"
description: "Administración de suscripciones de Azure con la CLI de Azure 2.0 en Linux, Mac o Windows."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: b0c0b3f5e4d9bc651ad4781cb0906dc98d8531a3
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2018
---
# <a name="manage-multiple-azure-subscriptions"></a>Administración de varias suscripciones de Azure

La mayoría de los usuarios de Azure solo tendrán una suscripción. Sin embargo, si forma parte de varias organizaciones o su organización ha dividido el acceso a determinados recursos mediante agrupaciones, habrá varias suscripciones dentro de Azure. Las distintas suscripciones se pueden administrar fácilmente con la CLI y, para realizar las operaciones, solo tiene que seleccionar una suscripción.

## <a name="tenants-users-and-subscriptions"></a>Inquilinos, usuarios y suscripciones

Quizás no tenga muy clara la diferencia entre los inquilinos, los usuarios y las suscripciones de Azure. Por lo general, un _inquilino_ es la entidad de Azure Active Directory que abarca toda la organización. Este inquilino tiene al menos una _suscripción_ y un _usuario_. Un usuario es un individuo que está asociado a un único inquilino, la organización a la que pertenece. Los usuarios son las cuentas que inician sesión en Azure para aprovisionar y usar los recursos. Un usuario puede tener acceso a varias _suscripciones_, que son los acuerdos con Microsoft para usar los servicios en la nube, incluido Azure. Cada recurso está asociado a una suscripción.

Para más información sobre las diferencias entre inquilinos, usuarios y suscripciones, vea el [diccionario de terminología de la nube de Azure](/azure/azure-glossary-cloud-terminology).
Para más información sobre cómo agregar una nueva suscripción a su inquilino de Azure Active Directory, consulte [Adición de una suscripción de Azure a Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Si trabaja con varios inquilinos, debe iniciar sesión en un inquilino específico. Para ello, consulte [Inicio de sesión con la CLI de Azure 2.0](/cli/azure/authenticate-azure-cli).

## <a name="working-with-multiple-subscriptions"></a>Trabajo con varias suscripciones

Para acceder a los recursos dentro de una suscripción, debe cambiar la suscripción activa. Todo el trabajo con las suscripciones se realiza mediante el comando `az account`, que hace referencia al acuerdo de servicio que representa una suscripción, y no la cuenta individual.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

Para empezar a trabajar con las suscripciones disponibles, obtenga una lista de las suscripciones disponibles en su cuenta:

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

Para cambiar la suscripción activa, puede utilizar `az account set`:

```azurecli-interactive
az account set --subscription "My Demos"
```

Para seleccionar la suscripción, puede usar el nombre o el identificador de la suscripción.
