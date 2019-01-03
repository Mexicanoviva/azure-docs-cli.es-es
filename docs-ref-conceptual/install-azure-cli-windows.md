---
title: Instalación de la CLI de Azure para Windows
description: Cómo instalar la CLI de Azure en Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ff4ed838351167410c75c046dc8f615faa0930f5
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593224"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="faed8-103">Instalación de la CLI de Azure en Windows</span><span class="sxs-lookup"><span data-stu-id="faed8-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="faed8-104">En Windows, la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="faed8-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="faed8-105">Si se va a instalar el subsistema de Windows para Linux (WSL), hay paquetes disponibles para su distribución de Linux.</span><span class="sxs-lookup"><span data-stu-id="faed8-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="faed8-106">Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.</span><span class="sxs-lookup"><span data-stu-id="faed8-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="faed8-107">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="faed8-107">Install or update</span></span>

<span data-ttu-id="faed8-108">El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows.</span><span class="sxs-lookup"><span data-stu-id="faed8-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="faed8-109">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="faed8-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="faed8-110">Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".</span><span class="sxs-lookup"><span data-stu-id="faed8-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="faed8-111">Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="faed8-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="faed8-112">PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows.</span><span class="sxs-lookup"><span data-stu-id="faed8-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="faed8-113">Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="faed8-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="faed8-114">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="faed8-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="faed8-115">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="faed8-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="faed8-116">Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="faed8-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="faed8-117">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="faed8-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

## <a name="next-steps"></a><span data-ttu-id="faed8-118">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="faed8-118">Next Steps</span></span>

<span data-ttu-id="faed8-119">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="faed8-119">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="faed8-120">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="faed8-120">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
