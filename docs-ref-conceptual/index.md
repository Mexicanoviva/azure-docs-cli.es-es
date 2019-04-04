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
ms.openlocfilehash: 3b9589c769a90e82c35aa64c583dffdac4e4f063
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421990"
---
# <a name="azure-command-line-interface-cli"></a><span data-ttu-id="24173-103">Interfaz de la línea de comandos (CLI) de Azure</span><span class="sxs-lookup"><span data-stu-id="24173-103">Azure Command-Line Interface (CLI)</span></span>

<span data-ttu-id="24173-104">La interfaz de la línea de comandos (CLI) de Azure es la experiencia de línea de comandos multiplataforma de Microsoft para administrar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="24173-104">The Azure command-line interface (CLI) is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="24173-105">Úsela en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o [instálela](install-azure-cli.md) en macOS, Linux y Windows y ejecútela desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="24173-105">Use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="24173-106">Es muy fácil empezar a trabajar con la CLI de Azure y está indicada para crear scripts de automatización que funcionan con Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="24173-106">The Azure CLI is easy to get started with, and best used for building automation scripts that work with the Azure Resource Manager.</span></span>
<span data-ttu-id="24173-107">Mediante la CLI de Azure, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="24173-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> <span data-ttu-id="24173-108">En los scripts y en el sitio de documentación de Microsoft, los ejemplos de la CLI de Azure están escritos para el shell de `bash`.</span><span class="sxs-lookup"><span data-stu-id="24173-108">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="24173-109">Los ejemplos de una línea funcionarán en cualquier plataforma.</span><span class="sxs-lookup"><span data-stu-id="24173-109">One-line examples will run on any platform.</span></span> <span data-ttu-id="24173-110">Los ejemplos más largos que incluyan continuaciones de línea (`\`) o asignación de variables deben modificarse para que funcionen en otros shells, incluido PowerShell.</span><span class="sxs-lookup"><span data-stu-id="24173-110">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="24173-111">Ejecutar o instalar</span><span class="sxs-lookup"><span data-stu-id="24173-111">Run or Install</span></span>

<span data-ttu-id="24173-112">Puede instalar la CLI localmente, ejecutarla en el explorador con Azure Cloud Shell o ejecutarla en un contenedor de Docker.</span><span class="sxs-lookup"><span data-stu-id="24173-112">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span> <span data-ttu-id="24173-113">Para obtener la versión actual de la CLI, ejecute `az --version`.</span><span class="sxs-lookup"><span data-stu-id="24173-113">To get the current version of the CLI, run `az --version`.</span></span>

* <span data-ttu-id="24173-114">Para ejecutarla en el explorador con Azure Cloud Shell, consulte [Inicio rápido de Bash en Azure Cloud Shell](/azure/cloud-shell/quickstart) o [Inicio rápido de PowerShell en Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="24173-114">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="24173-115">Para instalar la CLI, consulte [Instalación de la CLI de Azure](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="24173-115">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="24173-116">Para ejecutarla como un contenedor de Docker, consulte [Ejecución de la CLI de Azure en un contenedor de Docker](run-azure-cli-docker.md)</span><span class="sxs-lookup"><span data-stu-id="24173-116">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="24173-117">Desarrollo de aptitudes con Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="24173-117">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="24173-118">Administración de máquinas virtuales con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="24173-118">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="24173-119">Control de los servicios de Azure con la CLI</span><span class="sxs-lookup"><span data-stu-id="24173-119">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="24173-120">Más aprendizaje interactivo...</span><span class="sxs-lookup"><span data-stu-id="24173-120">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="24173-121">Introducción</span><span class="sxs-lookup"><span data-stu-id="24173-121">Get started</span></span>

<span data-ttu-id="24173-122">Lea el artículo de [introducción](get-started-with-azure-cli.md) para conocer los conceptos básicos de la CLI.</span><span class="sxs-lookup"><span data-stu-id="24173-122">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="24173-123">Los ejemplos siguientes muestran algunos casos de uso comunes:</span><span class="sxs-lookup"><span data-stu-id="24173-123">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="24173-124">Máquinas virtuales Linux</span><span class="sxs-lookup"><span data-stu-id="24173-124">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="24173-125">Máquinas virtuales Windows</span><span class="sxs-lookup"><span data-stu-id="24173-125">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="24173-126">Aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="24173-126">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="24173-127">SQL Database</span><span class="sxs-lookup"><span data-stu-id="24173-127">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="24173-128">Hay también disponible una [referencia](/cli/azure/reference-index) detallada que muestra cómo utilizar cada comando de la CLI de Azure de forma individual.</span><span class="sxs-lookup"><span data-stu-id="24173-128">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="24173-129">Si utiliza la versión anterior de la CLI (CLI clásica de Azure), aún podrá seguir usándola.</span><span class="sxs-lookup"><span data-stu-id="24173-129">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="24173-130">Sin embargo, se recomienda actualizar a la última versión de la CLI de Azure para disfrutar de una mejor experiencia.</span><span class="sxs-lookup"><span data-stu-id="24173-130">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="24173-131">Si utiliza ambas CLI, recuerde que `azure` es la CLI clásica y que `az` es la CLI más reciente.</span><span class="sxs-lookup"><span data-stu-id="24173-131">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>
