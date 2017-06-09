---
title: "Administración de suscripciones de Azure con la CLI de Azure 2.0"
description: "Administración de suscripciones de Azure con la CLI de Azure 2.0 en Linux, Mac o Windows."
keywords: "CLI de Azure 2.0, Linux, Mac, Windows, OS X, suscripción"
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: 383fb6ebd90ac79f60869187b402d53d4f1791fd
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2017
---
# <a name="manage-multiple-azure-subscriptions"></a>Administración de varias suscripciones de Azure

Si es nuevo en Azure, probablemente solo tenga una única suscripción.
Pero si ya lleva usando Azure durante un tiempo, puede haber creado varias suscripciones de Azure.
Si es así, puede configurar la CLI de Azure 2.0 para ejecutar comandos en una suscripción determinada.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

1. Obtenga una lista de todas las suscripciones de su cuenta.

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

1. Establezca el valor predeterminado.
 
   ```azurecli-interactive
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > El parámetro `--subscription` toma el nombre o el identificador de la suscripción.

Puede comprobar el cambio ejecutando el comando `az account list --output table` de nuevo.

Cuando esté establecida la suscripción predeterminada, todos los comandos de la CLI de Azure subsiguientes se ejecutarán en esta suscripción.