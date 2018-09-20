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
# <a name="azure-cli-20"></a><span data-ttu-id="1c494-103">CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="1c494-103">Azure CLI 2.0</span></span>

<span data-ttu-id="1c494-104">La CLI de Azure 2.0 es la experiencia de línea de comandos multiplataforma de Microsoft para administrar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="1c494-104">The Azure CLI 2.0 is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="1c494-105">Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="1c494-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="1c494-106">Es muy fácil empezar a trabajar con la CLI de Azure 2.0, y está indicada para crear scripts de automatización que funcionan con Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="1c494-106">Azure CLI 2.0 is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="1c494-107">Mediante la CLI de Azure 2.0, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="1c494-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="1c494-108">Ejecutar o instalar</span><span class="sxs-lookup"><span data-stu-id="1c494-108">Run or Install</span></span>

<span data-ttu-id="1c494-109">Puede instalar la CLI localmente, ejecutarla en el explorador con Azure Cloud Shell o ejecutarla en un contenedor de Docker.</span><span class="sxs-lookup"><span data-stu-id="1c494-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="1c494-110">Para ejecutarla en el explorador con Azure Cloud Shell, consulte [Inicio rápido de Bash en Azure Cloud Shell](/azure/cloud-shell/quickstart) o [Inicio rápido de PowerShell en Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="1c494-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="1c494-111">Para instalar la CLI, consulte [Instalación de la CLI de Azure 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1c494-111">To install the CLI, see [Install the Azure CLI 2.0](install-azure-cli.md).</span></span>
* <span data-ttu-id="1c494-112">Para ejecutarla como un contenedor de Docker, consulte [Ejecución de la CLI de Azure 2.0 en un contenedor de Docker](run-azure-cli-docker.md).</span><span class="sxs-lookup"><span data-stu-id="1c494-112">To run as a Docker container, see [Run Azure CLI 2.0 in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="get-started"></a><span data-ttu-id="1c494-113">Introducción</span><span class="sxs-lookup"><span data-stu-id="1c494-113">Get started</span></span>

<span data-ttu-id="1c494-114">Lea el artículo de [introducción](get-started-with-azure-cli.md) para conocer los conceptos básicos de la CLI.</span><span class="sxs-lookup"><span data-stu-id="1c494-114">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="1c494-115">Los ejemplos siguientes muestran algunos casos de uso comunes:</span><span class="sxs-lookup"><span data-stu-id="1c494-115">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="1c494-116">Máquinas virtuales Linux</span><span class="sxs-lookup"><span data-stu-id="1c494-116">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="1c494-117">Máquinas virtuales Windows</span><span class="sxs-lookup"><span data-stu-id="1c494-117">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="1c494-118">Aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="1c494-118">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="1c494-119">SQL Database</span><span class="sxs-lookup"><span data-stu-id="1c494-119">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="1c494-120">Hay una detallada [referencia](/cli/azure/reference-index) también disponible que muestra cómo utilizar cada comando de la CLI de Azure 2.0 de forma individual.</span><span class="sxs-lookup"><span data-stu-id="1c494-120">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

> [!NOTE]
> <span data-ttu-id="1c494-121">Si utiliza la versión anterior de la CLI (CLI de Azure 1.0), aún podrá seguir usándola.</span><span class="sxs-lookup"><span data-stu-id="1c494-121">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="1c494-122">Sin embargo, se recomienda actualizar a la CLI de Azure 2.0 para disfrutar de una mejor experiencia.</span><span class="sxs-lookup"><span data-stu-id="1c494-122">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="1c494-123">Si utiliza ambas CLI, recuerde que `azure` es la antigua CLI (CLI de Azure) y que `az` es la nueva CLI (CLI de Azure 2.0).</span><span class="sxs-lookup"><span data-stu-id="1c494-123">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
