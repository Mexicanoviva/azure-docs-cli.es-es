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
ms.openlocfilehash: 6c972ba69344f9e8bcd14a96a90e9dadb6cd8132
ms.sourcegitcommit: 61965f5d95d0dae3752ad6a0e5a93db27a623c28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2019
ms.locfileid: "68830963"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="a723e-103">Instalación de la CLI de Azure en Windows</span><span class="sxs-lookup"><span data-stu-id="a723e-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="a723e-104">En Windows, la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a723e-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="a723e-105">Si se va a instalar el subsistema de Windows para Linux (WSL), hay paquetes disponibles para su distribución de Linux.</span><span class="sxs-lookup"><span data-stu-id="a723e-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="a723e-106">Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.</span><span class="sxs-lookup"><span data-stu-id="a723e-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="a723e-107">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="a723e-107">Install or update</span></span>

<span data-ttu-id="a723e-108">El archivo MSI distribuible se usa para instalar o actualizar la CLI de Azure en Windows.</span><span class="sxs-lookup"><span data-stu-id="a723e-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="a723e-109">No es necesario desinstalar las versiones actuales antes de usar el instalador MSI.</span><span class="sxs-lookup"><span data-stu-id="a723e-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a723e-110">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="a723e-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="a723e-111">Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".</span><span class="sxs-lookup"><span data-stu-id="a723e-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="a723e-112">También puede instalar la CLI de Azure mediante PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a723e-112">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="a723e-113">Abra PowerShell como administrador y ejecute el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="a723e-113">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'
   ```
<span data-ttu-id="a723e-114">Esto descargará e instalará la versión más reciente de la CLI de Azure para Windows.</span><span class="sxs-lookup"><span data-stu-id="a723e-114">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="a723e-115">Si ya tiene instalada una versión, se actualizará la versión existente.</span><span class="sxs-lookup"><span data-stu-id="a723e-115">If you already have a version installed, it will update the existing version.</span></span> <span data-ttu-id="a723e-116">Una vez completada la instalación, tendrá que volver a abrir PowerShell para usar la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="a723e-116">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

<span data-ttu-id="a723e-117">Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a723e-117">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="a723e-118">PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows.</span><span class="sxs-lookup"><span data-stu-id="a723e-118">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="a723e-119">Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="a723e-119">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="a723e-120">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a723e-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="a723e-121">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="a723e-121">Troubleshooting</span></span>

<span data-ttu-id="a723e-122">Estos son algunos problemas comunes que se han observado cuando se instala con Windows.</span><span class="sxs-lookup"><span data-stu-id="a723e-122">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="a723e-123">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="a723e-123">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="a723e-124">Conexión de bloques proxy</span><span class="sxs-lookup"><span data-stu-id="a723e-124">Proxy blocks connection</span></span>

<span data-ttu-id="a723e-125">Si no puede descargar al instalador MSI porque el proxy está bloqueando la conexión, asegúrese de que el servidor proxy esté configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="a723e-125">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="a723e-126">En Windows 10, esta configuración se administra en el panel `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="a723e-126">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="a723e-127">Póngase en contacto con el administrador del sistema para más información sobre la configuración necesaria, o si su máquina se puede administrar mediante configuración o si requiere configuración avanzada.</span><span class="sxs-lookup"><span data-stu-id="a723e-127">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a723e-128">Esta configuración también es necesaria para poder tener acceso a los servicios de Azure con la CLI, PowerShell o la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="a723e-128">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="a723e-129">En PowerShell, se hace con el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="a723e-129">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="a723e-130">Para obtener el MSI, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:</span><span class="sxs-lookup"><span data-stu-id="a723e-130">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="a723e-131">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="a723e-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="a723e-132">La CLI de Azure se desinstala desde la lista "Aplicaciones y características" de Windows.</span><span class="sxs-lookup"><span data-stu-id="a723e-132">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="a723e-133">Para desinstalar:</span><span class="sxs-lookup"><span data-stu-id="a723e-133">To uninstall:</span></span>

| <span data-ttu-id="a723e-134">Plataforma</span><span class="sxs-lookup"><span data-stu-id="a723e-134">Platform</span></span> | <span data-ttu-id="a723e-135">Instrucciones</span><span class="sxs-lookup"><span data-stu-id="a723e-135">Instructions</span></span> |
|---|---|
| <span data-ttu-id="a723e-136">Windows 10</span><span class="sxs-lookup"><span data-stu-id="a723e-136">Windows 10</span></span> | <span data-ttu-id="a723e-137">Inicio > Configuración > Aplicaciones</span><span class="sxs-lookup"><span data-stu-id="a723e-137">Start > Settings > Apps</span></span> |
| <span data-ttu-id="a723e-138">Windows 8</span><span class="sxs-lookup"><span data-stu-id="a723e-138">Windows 8</span></span><br/><span data-ttu-id="a723e-139">Windows 7</span><span class="sxs-lookup"><span data-stu-id="a723e-139">Windows 7</span></span> | <span data-ttu-id="a723e-140">Inicio > Panel de Control > Programas > Desinstalar un programa</span><span class="sxs-lookup"><span data-stu-id="a723e-140">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="a723e-141">En esta pantalla, escriba __CLI de Azure__ en la barra de búsqueda de programas.</span><span class="sxs-lookup"><span data-stu-id="a723e-141">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="a723e-142">El programa para desinstalar aparece como __Microsoft CLI 2.0 para Azure__.</span><span class="sxs-lookup"><span data-stu-id="a723e-142">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="a723e-143">Seleccione esta aplicación y haga clic en el botón `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="a723e-143">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a723e-144">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="a723e-144">Next Steps</span></span>

<span data-ttu-id="a723e-145">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="a723e-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a723e-146">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="a723e-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
