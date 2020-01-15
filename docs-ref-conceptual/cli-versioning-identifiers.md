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
# <a name="differences-between-azure-cli-products"></a>Diferencias entre los productos de la CLI de Azure

A partir de finales de junio de 2018, se quitaron los números de versión explícita de los nombres de producto de la CLI de Azure. Este cambio ayuda a eliminar la confusión que a veces aparecía en la documentación en la que se informaba a los usuarios sobre el uso de "la CLI de Azure", pero no quedaba claro a qué versión del producto se hace referencia. Si está familiarizado con los nombres de producto anteriores, aquí se muestra cómo han cambiado:

* Las versiones de la CLI de Azure 2.0 y posteriores ahora se conocen como la "CLI de Azure".
* Las versiones anteriores de la CLI de Azure (1.x y anteriores) ahora se conocen como la "CLI clásica de Azure".

El cambio de nombre en la CLI clásica de Azure deja claro que esta herramienta está diseñada para usarse solo con el modelo de implementación clásico. Además, la CLI clásica ya no se actualiza ni mantiene. Por este motivo y muchos otros, se recomienda mover las implementaciones clásicas para que usen el modelo de Azure Resource Manager y migrar a la última versión disponible de la CLI de Azure.

Si todavía usa la CLI clásica, puede obtener información sobre el proceso de migración en los siguientes artículos:

* [Migración del modelo clásico a Azure Resource Manager](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [Instalación de la CLI de Azure](install-azure-cli.md)
* [Migración desde la CLI clásica de Azure a la CLI de Azure](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
