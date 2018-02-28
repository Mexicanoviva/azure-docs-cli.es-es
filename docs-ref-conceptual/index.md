---
title: CLI de Azure 2.0
description: "Introducción a la CLI de Azure 2.0."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 5f3d514200b138d498043e0efb2cf5c2f478d108
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="azure-cli-20"></a>CLI de Azure 2.0

La CLI 2.0 de Azure es la nueva experiencia de línea de comandos de Azure para administrar recursos de Azure.
Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.

La CLI de Azure 2.0 está optimizada para administrar recursos de Azure desde la línea de comandos y para generar scripts de automatización que funcionan con Azure Resource Manager. Mediante la CLI de Azure 2.0, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Use [Cloud Shell](/azure/cloud-shell/overview) para ejecutar la CLI en el explorador o [instálela](install-azure-cli.md) en Windows, Linux o macOS.
Lea el artículo de [introducción](get-started-with-azure-cli.md) para empezar a usar la CLI.
Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).

Los ejemplos siguientes pueden ayudarle a obtener información sobre cómo realizar escenarios comunes con la CLI de Azure 2.0:
- [Máquinas virtuales Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas virtuales Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Hay una detallada [referencia](/cli/azure/) también disponible que muestra cómo utilizar cada comando de la CLI de Azure 2.0 de forma individual.

[Empiece](get-started-with-azure-cli.md) ya a trabajar con la CLI de Azure 2.0.


> [!NOTE]
> Si utiliza la versión anterior de la CLI (CLI de Azure), aún podrá seguir usándola.
> Si utiliza ambas CLI, recuerde que `azure` es la antigua CLI (CLI de Azure) y que `az` es la nueva CLI (CLI de Azure 2.0).
