---
title: Diferencias entre los productos de la CLI de Azure
description: Obtenga información sobre cómo se denominan y versionan los productos de la CLI de Azure y cómo realizar la actualización.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/12/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a39f6b0fbccf937aec2b227ed4e3f4ff8d92137f
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158940"
---
# <a name="differences-between-azure-cli-products"></a>Diferencias entre los productos de la CLI de Azure

A partir de finales de junio de 2018, se quitaron los números de versión explícita de los nombres de producto de la CLI de Azure. Este cambio ayuda a eliminar la confusión que a veces aparecía en la documentación en la que se informaba a los usuarios sobre el uso de "la CLI de Azure", pero no quedaba claro a qué versión del producto se hace referencia. Si está familiarizado con los nombres de producto anteriores, aquí se muestra cómo han cambiado:

* Las versiones de la CLI de Azure 2.0 y posteriores ahora se conocen como la "CLI de Azure".
* Las versiones anteriores de la CLI de Azure (1.x y anteriores) ahora se conocen como la "CLI clásica de Azure".

El cambio de nombre en la CLI clásica de Azure deja claro que esta herramienta está diseñada para usarse solo con el modelo de implementación clásico. Además, la CLI clásica ya no se actualiza ni mantiene. Por este motivo y muchos otros, se recomienda mover las implementaciones clásicas para que usen el modelo de Azure Resource Manager y migrar a la última versión disponible de la CLI de Azure.

Si todavía usa la CLI clásica, puede obtener información sobre el proceso de migración en los siguientes artículos:

* [Migración del modelo clásico a Azure Resource Manager](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [Instalación de la CLI de Azure](install-azure-cli.md)
* [Migración desde la CLI clásica de Azure a la CLI de Azure](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
