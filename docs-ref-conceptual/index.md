---
title: Introducción a la CLI de Azure 2.0
description: Introducción a la CLI de Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388395"
---
# <a name="azure-cli-20"></a>CLI de Azure 2.0

La CLI de Azure 2.0 es la experiencia de línea de comandos multiplataforma de Microsoft para administrar los recursos de Azure.
Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.

Es muy fácil empezar a trabajar con la CLI de Azure 2.0, y está indicada para crear scripts de automatización que funcionan con Azure Resource Manager. Mediante la CLI de Azure 2.0, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a>Ejecutar o instalar

Puede instalar la CLI localmente, ejecutarla en el explorador con Azure Cloud Shell o ejecutarla en un contenedor de Docker.

* Para ejecutarla en el explorador con Azure Cloud Shell, consulte [Inicio rápido de Bash en Azure Cloud Shell](/azure/cloud-shell/quickstart) o [Inicio rápido de PowerShell en Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Para instalar la CLI, consulte [Instalación de la CLI de Azure 2.0](install-azure-cli.md).
* Para ejecutarla como un contenedor de Docker, consulte [Ejecución de la CLI de Azure 2.0 en un contenedor de Docker](run-azure-cli-docker.md).

## <a name="get-started"></a>Introducción

Lea el artículo de [introducción](get-started-with-azure-cli.md) para conocer los conceptos básicos de la CLI. Los ejemplos siguientes muestran algunos casos de uso comunes:

- [Máquinas virtuales Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Máquinas virtuales Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Aplicaciones web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Hay una detallada [referencia](/cli/azure/reference-index) también disponible que muestra cómo utilizar cada comando de la CLI de Azure 2.0 de forma individual.

> [!NOTE]
> Si utiliza la versión anterior de la CLI (CLI de Azure 1.0), aún podrá seguir usándola.
> Sin embargo, se recomienda actualizar a la CLI de Azure 2.0 para disfrutar de una mejor experiencia.
> Si utiliza ambas CLI, recuerde que `azure` es la antigua CLI (CLI de Azure) y que `az` es la nueva CLI (CLI de Azure 2.0).
