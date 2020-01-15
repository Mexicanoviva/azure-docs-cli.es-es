---
title: Diferencias entre los productos de la CLI de Azure
description: Obtenga información sobre cómo se denominan y versionan los productos de la CLI de Azure y cómo realizar la actualización.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/12/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 77b3629d0cc79d2b329007fd93b49022d5f29783
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913600"
---
# <a name="differences-between-azure-cli-products"></a><span data-ttu-id="e3040-103">Diferencias entre los productos de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="e3040-103">Differences between Azure CLI products</span></span>

<span data-ttu-id="e3040-104">A partir de finales de junio de 2018, se quitaron los números de versión explícita de los nombres de producto de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="e3040-104">As of the end of June 2018, explicit version numbers have been removed from Azure CLI product names.</span></span> <span data-ttu-id="e3040-105">Este cambio ayuda a eliminar la confusión que a veces aparecía en la documentación en la que se informaba a los usuarios sobre el uso de "la CLI de Azure", pero no quedaba claro a qué versión del producto se hace referencia.</span><span class="sxs-lookup"><span data-stu-id="e3040-105">This change helps eliminate confusion that sometimes showed up in documentation where users were told to use "the Azure CLI" but it was unclear what version of the product was being referenced.</span></span> <span data-ttu-id="e3040-106">Si está familiarizado con los nombres de producto anteriores, aquí se muestra cómo han cambiado:</span><span class="sxs-lookup"><span data-stu-id="e3040-106">If you're familiar with the old product names, here is how they have changed:</span></span>

* <span data-ttu-id="e3040-107">Las versiones de la CLI de Azure 2.0 y posteriores ahora se conocen como la "CLI de Azure".</span><span class="sxs-lookup"><span data-stu-id="e3040-107">Azure CLI versions 2.0 and later are now referred to only as "Azure CLI."</span></span>
* <span data-ttu-id="e3040-108">Las versiones anteriores de la CLI de Azure (1.x y anteriores) ahora se conocen como la "CLI clásica de Azure".</span><span class="sxs-lookup"><span data-stu-id="e3040-108">Earlier Azure CLI versions (1.x and lower) are now referred to as "Azure classic CLI."</span></span>

<span data-ttu-id="e3040-109">El cambio de nombre en la CLI clásica de Azure deja claro que esta herramienta está diseñada para usarse solo con el modelo de implementación clásico.</span><span class="sxs-lookup"><span data-stu-id="e3040-109">The name change to Azure classic CLI makes it clear that this tool is meant to be used only with the classic deployment model.</span></span> <span data-ttu-id="e3040-110">Además, la CLI clásica ya no se actualiza ni mantiene.</span><span class="sxs-lookup"><span data-stu-id="e3040-110">The classic CLI is also no longer updated or maintained.</span></span> <span data-ttu-id="e3040-111">Por este motivo y muchos otros, se recomienda mover las implementaciones clásicas para que usen el modelo de Azure Resource Manager y migrar a la última versión disponible de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="e3040-111">For this reason, and many more, it's recommended that you move any classic deployments to use the Azure Resource Manager model and migrate to the latest available version of the Azure CLI.</span></span>

<span data-ttu-id="e3040-112">Si todavía usa la CLI clásica, puede obtener información sobre el proceso de migración en los siguientes artículos:</span><span class="sxs-lookup"><span data-stu-id="e3040-112">If you are still using the classic CLI, you can learn about the process of migrating in the following articles:</span></span>

* [<span data-ttu-id="e3040-113">Migración del modelo clásico a Azure Resource Manager</span><span class="sxs-lookup"><span data-stu-id="e3040-113">Migrate from Classic to Azure Resource Manager</span></span>](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [<span data-ttu-id="e3040-114">Instalación de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="e3040-114">Install the Azure CLI</span></span>](install-azure-cli.md)
* [<span data-ttu-id="e3040-115">Migración desde la CLI clásica de Azure a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="e3040-115">Migrating from Azure classic CLI to Azure CLI</span></span>](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
