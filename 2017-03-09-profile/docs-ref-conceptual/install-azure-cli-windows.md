---
title: "Instalación de la CLI de Azure para Windows"
description: "Instalación de la CLI de Azure 2.0 en Windows"
keywords: CLI de Azure, instalar la CLI de Azure, instalar azure windows, azure cli windows, azure windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="047aa-104">Instalación de la CLI de Azure 2.0 en Windows</span><span class="sxs-lookup"><span data-stu-id="047aa-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="047aa-105">En Windows, puede instalar un archivo binario nativo desde un archivo MSI, que se puede usar mediante el símbolo del sistema de Windows o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="047aa-105">On Windows, you can install a native binary from an MSI, which you can use through the Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="047aa-106">Si está ejecutando el subsistema de Windows para Linux (WSL), hay paquetes disponibles para la distribución que se está ejecutando.</span><span class="sxs-lookup"><span data-stu-id="047aa-106">If you are running Windows Subsystem for Linux (WSL) there are packages available for the distribution you are running.</span></span> <span data-ttu-id="047aa-107">Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.</span><span class="sxs-lookup"><span data-stu-id="047aa-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update-with-msi"></a><span data-ttu-id="047aa-108">Instalación o actualización con MSI</span><span class="sxs-lookup"><span data-stu-id="047aa-108">Install or update with MSI</span></span>

<span data-ttu-id="047aa-109">El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows.</span><span class="sxs-lookup"><span data-stu-id="047aa-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span> <span data-ttu-id="047aa-110">También puede [descargar el instalador MSI](https://aka.ms/InstallAzureCliWindows) y, a continuación, ejecutarlo para instalar o actualizar.</span><span class="sxs-lookup"><span data-stu-id="047aa-110">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) and then run it to install or update.</span></span>

<span data-ttu-id="047aa-111">Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".</span><span class="sxs-lookup"><span data-stu-id="047aa-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="047aa-112">Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="047aa-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span>

## <a name="uninstall-with-msi"></a><span data-ttu-id="047aa-113">Desinstalación con MSI</span><span class="sxs-lookup"><span data-stu-id="047aa-113">Uninstall with MSI</span></span>

<span data-ttu-id="047aa-114">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="047aa-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="047aa-115">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="047aa-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="047aa-116">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="047aa-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="047aa-117">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="047aa-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="047aa-118">Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="047aa-118">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> <span data-ttu-id="047aa-119">También puede [descargar el instalador MSI](https://aka.ms/InstallAzureCliWindows) si no lo tiene disponible.</span><span class="sxs-lookup"><span data-stu-id="047aa-119">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) if you no longer have it available.</span></span>
