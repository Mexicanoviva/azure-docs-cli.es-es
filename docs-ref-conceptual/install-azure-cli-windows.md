---
title: Instalación de la CLI de Azure para Windows
description: Cómo instalar la CLI de Azure en Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240549"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="d17f8-103">Instalación de la CLI de Azure en Windows</span><span class="sxs-lookup"><span data-stu-id="d17f8-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="d17f8-104">En Windows, la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d17f8-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="d17f8-105">Si se va a instalar el subsistema de Windows para Linux (WSL), hay paquetes disponibles para su distribución de Linux.</span><span class="sxs-lookup"><span data-stu-id="d17f8-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="d17f8-106">Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.</span><span class="sxs-lookup"><span data-stu-id="d17f8-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="d17f8-107">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="d17f8-107">Install or update</span></span>

<span data-ttu-id="d17f8-108">El archivo MSI distribuible se usa para instalar o actualizar la CLI de Azure en Windows.</span><span class="sxs-lookup"><span data-stu-id="d17f8-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="d17f8-109">No es necesario desinstalar las versiones actuales antes de usar el instalador MSI.</span><span class="sxs-lookup"><span data-stu-id="d17f8-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d17f8-110">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="d17f8-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="d17f8-111">Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".</span><span class="sxs-lookup"><span data-stu-id="d17f8-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="d17f8-112">Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d17f8-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="d17f8-113">PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows.</span><span class="sxs-lookup"><span data-stu-id="d17f8-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="d17f8-114">Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="d17f8-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d17f8-115">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d17f8-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="d17f8-116">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="d17f8-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="d17f8-117">La CLI de Azure se desinstala desde la lista "Aplicaciones y características" de Windows.</span><span class="sxs-lookup"><span data-stu-id="d17f8-117">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="d17f8-118">Para desinstalar:</span><span class="sxs-lookup"><span data-stu-id="d17f8-118">To uninstall:</span></span>

| <span data-ttu-id="d17f8-119">Plataforma</span><span class="sxs-lookup"><span data-stu-id="d17f8-119">Platform</span></span> | <span data-ttu-id="d17f8-120">Instrucciones</span><span class="sxs-lookup"><span data-stu-id="d17f8-120">Instructions</span></span> |
|---|---|
| <span data-ttu-id="d17f8-121">Windows 10</span><span class="sxs-lookup"><span data-stu-id="d17f8-121">Windows 10</span></span> | <span data-ttu-id="d17f8-122">Inicio > Configuración > Aplicaciones</span><span class="sxs-lookup"><span data-stu-id="d17f8-122">Start > Settings > Apps</span></span> |
| <span data-ttu-id="d17f8-123">Windows 8</span><span class="sxs-lookup"><span data-stu-id="d17f8-123">Windows 8</span></span><br/><span data-ttu-id="d17f8-124">Windows 7</span><span class="sxs-lookup"><span data-stu-id="d17f8-124">Windows 7</span></span> | <span data-ttu-id="d17f8-125">Inicio > Panel de Control > Programas > Desinstalar un programa</span><span class="sxs-lookup"><span data-stu-id="d17f8-125">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="d17f8-126">En esta pantalla, escriba __CLI de Azure__ en la barra de búsqueda de programas.</span><span class="sxs-lookup"><span data-stu-id="d17f8-126">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="d17f8-127">El programa para desinstalar aparece como __Microsoft CLI 2.0 para Azure__.</span><span class="sxs-lookup"><span data-stu-id="d17f8-127">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="d17f8-128">Seleccione esta aplicación y haga clic en el botón `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="d17f8-128">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d17f8-129">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d17f8-129">Next Steps</span></span>

<span data-ttu-id="d17f8-130">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="d17f8-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d17f8-131">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="d17f8-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
