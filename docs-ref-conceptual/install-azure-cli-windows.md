---
title: "Instalación de la CLI de Azure para Windows"
description: "Instalación de la CLI de Azure 2.0 en Windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: df1c2b33589c160525710845cc81d076082a9ecc
ms.sourcegitcommit: def1a07bfccf26a4178ba6dd836764a1df205929
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="9cf3f-103">Instalación de la CLI de Azure 2.0 en Windows</span><span class="sxs-lookup"><span data-stu-id="9cf3f-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="9cf3f-104">En Windows, el archivo binario de la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9cf3f-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="9cf3f-105">Si está ejecutando el subsistema de Windows para Linux (WSL), hay paquetes disponibles para la distribución de Linux.</span><span class="sxs-lookup"><span data-stu-id="9cf3f-105">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="9cf3f-106">Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.</span><span class="sxs-lookup"><span data-stu-id="9cf3f-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="9cf3f-107">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="9cf3f-107">Install or update</span></span>

<span data-ttu-id="9cf3f-108">El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows.</span><span class="sxs-lookup"><span data-stu-id="9cf3f-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9cf3f-109">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="9cf3f-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="9cf3f-110">Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".</span><span class="sxs-lookup"><span data-stu-id="9cf3f-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="9cf3f-111">Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9cf3f-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="9cf3f-112">PowerShell ofrece algunas características de la función de autocompletar que no están disponibles desde CMD.</span><span class="sxs-lookup"><span data-stu-id="9cf3f-112">PowerShell offers some tab completion features not available from CMD.</span></span>

## <a name="uninstall"></a><span data-ttu-id="9cf3f-113">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="9cf3f-113">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="9cf3f-114">Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="9cf3f-114">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9cf3f-115">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="9cf3f-115">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
