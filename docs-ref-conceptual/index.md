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
ms.openlocfilehash: 98f122a9b7a33bf2270664a9e5077d4cd206a6af
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2018
---
# <a name="azure-cli-20"></a><span data-ttu-id="448f0-103">CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="448f0-103">Azure CLI 2.0</span></span>

<span data-ttu-id="448f0-104">La CLI 2.0 de Azure es la nueva experiencia de línea de comandos de Azure para administrar recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="448f0-104">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="448f0-105">Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="448f0-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="448f0-106">La CLI de Azure 2.0 está optimizada para administrar recursos de Azure desde la línea de comandos y para generar scripts de automatización que funcionan con Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="448f0-106">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="448f0-107">Mediante la CLI de Azure 2.0, puede crear máquinas virtuales en Azure simplemente con escribir el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="448f0-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="448f0-108">Use [Cloud Shell](/azure/cloud-shell/overview) para ejecutar la CLI en el explorador o [instálela](install-azure-cli.md) en Windows, Linux o macOS.</span><span class="sxs-lookup"><span data-stu-id="448f0-108">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="448f0-109">Lea el artículo de [introducción](get-started-with-azure-cli.md) para empezar a usar la CLI.</span><span class="sxs-lookup"><span data-stu-id="448f0-109">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="448f0-110">Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="448f0-110">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="448f0-111">Los ejemplos siguientes pueden ayudarle a obtener información sobre cómo realizar escenarios comunes con la CLI de Azure 2.0:</span><span class="sxs-lookup"><span data-stu-id="448f0-111">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="448f0-112">Máquinas virtuales Linux</span><span class="sxs-lookup"><span data-stu-id="448f0-112">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="448f0-113">Máquinas virtuales Windows</span><span class="sxs-lookup"><span data-stu-id="448f0-113">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="448f0-114">Web Apps</span><span class="sxs-lookup"><span data-stu-id="448f0-114">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="448f0-115">SQL Database</span><span class="sxs-lookup"><span data-stu-id="448f0-115">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="448f0-116">Hay una detallada [referencia](/cli/azure/reference-index) también disponible que muestra cómo utilizar cada comando de la CLI de Azure 2.0 de forma individual.</span><span class="sxs-lookup"><span data-stu-id="448f0-116">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="448f0-117">[Empiece](get-started-with-azure-cli.md) ya a trabajar con la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="448f0-117">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="448f0-118">Si utiliza la versión anterior de la CLI (CLI de Azure), aún podrá seguir usándola.</span><span class="sxs-lookup"><span data-stu-id="448f0-118">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="448f0-119">Si utiliza ambas CLI, recuerde que `azure` es la antigua CLI (CLI de Azure) y que `az` es la nueva CLI (CLI de Azure 2.0).</span><span class="sxs-lookup"><span data-stu-id="448f0-119">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
