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
ms.openlocfilehash: 36a08835b9c4f6e71c5ddadbce8ba946c52a1e9b
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2017
---
# <a name="azure-cli-20"></a><span data-ttu-id="d1ff5-104">CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="d1ff5-104">Azure CLI 2.0</span></span>

<span data-ttu-id="d1ff5-105">La CLI 2.0 de Azure es la nueva experiencia de línea de comandos de Azure para administrar recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-105">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="d1ff5-106">Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="d1ff5-107">La CLI de Azure 2.0 está optimizada para administrar recursos de Azure desde la línea de comandos y para generar scripts de automatización que funcionan con Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="d1ff5-108">Mediante la CLI de Azure 2.0, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="d1ff5-108">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="d1ff5-109">Use [Cloud Shell](/azure/cloud-shell/overview) para ejecutar la CLI en el explorador o [instálela](install-azure-cli.md) en Windows, Linux o macOS.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-109">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="d1ff5-110">Lea el artículo de [introducción](get-started-with-azure-cli.md) para empezar a usar la CLI.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-110">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="d1ff5-111">Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d1ff5-111">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="d1ff5-112">Los ejemplos siguientes pueden ayudarle a obtener información sobre cómo realizar escenarios comunes con la CLI de Azure 2.0:</span><span class="sxs-lookup"><span data-stu-id="d1ff5-112">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="d1ff5-113">Máquinas virtuales Linux</span><span class="sxs-lookup"><span data-stu-id="d1ff5-113">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="d1ff5-114">Máquinas virtuales Windows</span><span class="sxs-lookup"><span data-stu-id="d1ff5-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="d1ff5-115">Web Apps</span><span class="sxs-lookup"><span data-stu-id="d1ff5-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="d1ff5-116">Base de datos SQL</span><span class="sxs-lookup"><span data-stu-id="d1ff5-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="d1ff5-117">Hay una detallada [referencia](/cli/azure/) también disponible que muestra cómo utilizar cada comando de la CLI de Azure 2.0 de forma individual.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-117">A detailed [reference](/cli/azure/) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="d1ff5-118">[Empiece](get-started-with-azure-cli.md) ya a trabajar con la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="d1ff5-119">Si utiliza la versión anterior de la CLI (CLI de Azure), aún podrá seguir usándola.</span><span class="sxs-lookup"><span data-stu-id="d1ff5-119">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="d1ff5-120">Si utiliza ambas CLI, recuerde que `azure` es la antigua CLI (CLI de Azure) y que `az` es la nueva CLI (CLI de Azure 2.0).</span><span class="sxs-lookup"><span data-stu-id="d1ff5-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span> 