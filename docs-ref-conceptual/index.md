---
title: Introducción a la CLI de Azure
description: Introducción a la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 047a953a0ab8ccaf145d56e4d774d2bf9852ed6f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177732"
---
# <a name="azure-cli"></a>Azure CLI

La CLI de Azure es la experiencia de línea de comandos multiplataforma de Microsoft para administrar los recursos de Azure.
Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.

Es muy fácil empezar a trabajar con la CLI de Azure y está indicada para crear scripts de automatización que funcionan con Azure Resource Manager. Mediante la CLI de Azure, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a>Ejecutar o instalar

Puede instalar la CLI localmente, ejecutarla en el explorador con Azure Cloud Shell o ejecutarla en un contenedor de Docker.

* Para ejecutarla en el explorador con Azure Cloud Shell, consulte [Inicio rápido de Bash en Azure Cloud Shell](/azure/cloud-shell/quickstart) o [Inicio rápido de PowerShell en Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Para instalar la CLI, consulte [Instalación de la CLI de Azure](install-azure-cli.md).
* Para ejecutarla como un contenedor de Docker, consulte [Ejecución de la CLI de Azure en un contenedor de Docker](run-azure-cli-docker.md)

## <a name="build-your-skills-with-microsoft-learn"></a>Desarrollo de aptitudes con Microsoft Learn

- [Administración de máquinas virtuales con la CLI de Azure](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [Control de los servicios de Azure con la CLI](/learn/modules/control-azure-services-with-cli/)
- [Más aprendizaje interactivo...](/learn/browse/?products=azure-clis)

## <a name="get-started"></a>Introducción

Lea el artículo de [introducción](get-started-with-azure-cli.md) para conocer los conceptos básicos de la CLI. Los ejemplos siguientes muestran algunos casos de uso comunes:

- [Máquinas virtuales Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas virtuales Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Aplicaciones web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Hay también disponible una [referencia](/cli/azure/reference-index) detallada que muestra cómo utilizar cada comando de la CLI de Azure de forma individual.

> [!NOTE]
> Si utiliza la versión anterior de la CLI (CLI clásica de Azure), aún podrá seguir usándola.
> Sin embargo, se recomienda actualizar a la última versión de la CLI de Azure para disfrutar de una mejor experiencia.
> Si utiliza ambas CLI, recuerde que `azure` es la CLI clásica y que `az` es la CLI más reciente.
