---
title: CLI de Azure 2.0
description: "Introducción a la CLI de Azure 2.0."
keywords: CLI de Azure 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 2f4f9950dd663ae85f41bf4efe114b15770ace5d
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: es-ES
---
# <a name="azure-cli-20"></a>CLI de Azure 2.0

La CLI 2.0 de Azure es la nueva experiencia de línea de comandos de Azure para administrar recursos de Azure.  Se puede usar en macOS, Linux y Windows. 

La CLI de Azure 2.0 está optimizada para administrar recursos de Azure desde la línea de comandos y para generar scripts de automatización que funcionan con Azure Resource Manager. Mediante la CLI de Azure 2.0, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Revise el artículo de la [instalación](install-azure-cli.md) para que la CLI de Azure 2.0 esté rápidamente en pleno rendimiento en el sistema. A continuación, lea el artículo de [introducción](get-started-with-azure-cli.md) para empezar a usarlo.
Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).

Los ejemplos siguientes pueden ayudarle a obtener información sobre cómo realizar escenarios comunes con la CLI de Azure 2.0:
- [Máquinas virtuales Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas virtuales Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Base de datos SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Hay una detallada [referencia](/cli/azure/) también disponible que muestra cómo utilizar cada comando de la CLI de Azure 2.0 de forma individual.

[Empiece](get-started-with-azure-cli.md) ya a trabajar con la CLI de Azure 2.0.


> [!NOTE]
> Si utiliza la versión anterior de la CLI (CLI de Azure), aún podrá seguir usándola.
> Si utiliza ambas CLI, recuerde que `azure` es la antigua CLI (CLI de Azure) y que `az` es la nueva CLI (CLI de Azure 2.0). 