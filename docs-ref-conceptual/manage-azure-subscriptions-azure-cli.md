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
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="feaf2-104">Administración de varias suscripciones de Azure</span><span class="sxs-lookup"><span data-stu-id="feaf2-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="feaf2-105">Si es nuevo en Azure, probablemente solo tenga una única suscripción.</span><span class="sxs-lookup"><span data-stu-id="feaf2-105">If you are brand new to Azure, you probably only have a single subscription.</span></span>
<span data-ttu-id="feaf2-106">Pero si ya lleva usando Azure durante un tiempo, puede haber creado varias suscripciones de Azure.</span><span class="sxs-lookup"><span data-stu-id="feaf2-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span>
<span data-ttu-id="feaf2-107">Si es así, puede configurar la CLI de Azure 2.0 para ejecutar comandos en una suscripción determinada.</span><span class="sxs-lookup"><span data-stu-id="feaf2-107">If so, you can configure Azure CLI 2.0 to execute commands against a particular subscription.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

1. <span data-ttu-id="feaf2-108">Obtenga una lista de todas las suscripciones de su cuenta.</span><span class="sxs-lookup"><span data-stu-id="feaf2-108">Get a list of all subscriptions in your account.</span></span>

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

1. <span data-ttu-id="feaf2-109">Establezca el valor predeterminado.</span><span class="sxs-lookup"><span data-stu-id="feaf2-109">Set the default.</span></span>
 
   ```azurecli-interactive
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > <span data-ttu-id="feaf2-110">El parámetro `--subscription` toma el nombre o el identificador de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="feaf2-110">The `--subscription` parameter takes either the subscription name or the subscription ID.</span></span>

<span data-ttu-id="feaf2-111">Puede comprobar el cambio ejecutando el comando `az account list --output table` de nuevo.</span><span class="sxs-lookup"><span data-stu-id="feaf2-111">You can verify the change by running the `az account list --output table` command again.</span></span>

<span data-ttu-id="feaf2-112">Cuando esté establecida la suscripción predeterminada, todos los comandos de la CLI de Azure subsiguientes se ejecutarán en esta suscripción.</span><span class="sxs-lookup"><span data-stu-id="feaf2-112">Once you set your default subscription, all subsequent Azure CLI commands run against this subscription.</span></span>