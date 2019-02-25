---
title: Introducción a la CLI de Azure
description: Introducción a la interfaz de la línea de comandos (CLI) de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
---

# <a name="azure-command-line-interface-cli"></a>Interfaz de la línea de comandos (CLI) de Azure

La interfaz de la línea de comandos (CLI) de Azure es la experiencia de línea de comandos multiplataforma de Microsoft para administrar los recursos de Azure.
Úsela en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o [instálela](install-azure-cli.md) en macOS, Linux y Windows y ejecútela desde la línea de comandos.

Es muy fácil empezar a trabajar con la CLI de Azure y está indicada para crear scripts de automatización que funcionan con Azure Resource Manager.
Mediante la CLI de Azure, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> En los scripts y en el sitio de documentación de Microsoft, los ejemplos de la CLI de Azure están escritos para el shell de `bash`. Los ejemplos de una línea funcionarán en cualquier plataforma. Los ejemplos más largos que incluyan continuaciones de línea (`\`) o asignación de variables deben modificarse para que funcionen en otros shells, incluido PowerShell.

## <a name="run-or-install"></a>Ejecutar o instalar

Puede instalar la CLI localmente, ejecutarla en el explorador con Azure Cloud Shell o ejecutarla en un contenedor de Docker. Para obtener la versión actual de la CLI, ejecute `az --version`.

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
