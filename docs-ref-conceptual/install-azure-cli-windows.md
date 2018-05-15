---
title: Instalación de la CLI de Azure para Windows
description: Instalación de la CLI de Azure 2.0 en Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c3ed3585b601ee55b267ea6cfc43ce41c54f084a
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="fc1d4-103">Instalación de la CLI de Azure 2.0 en Windows</span><span class="sxs-lookup"><span data-stu-id="fc1d4-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="fc1d4-104">En Windows, el archivo binario de la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="fc1d4-105">Si está ejecutando el subsistema de Windows para Linux (WSL), hay paquetes disponibles para la distribución de Linux.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-105">If you are running the Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="fc1d4-106">Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="fc1d4-107">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="fc1d4-107">Install or update</span></span>

<span data-ttu-id="fc1d4-108">El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="fc1d4-109">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="fc1d4-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="fc1d4-110">Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".</span><span class="sxs-lookup"><span data-stu-id="fc1d4-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="fc1d4-111">Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="fc1d4-112">PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="fc1d4-113">Para iniciar sesión, ejecute el comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-113">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="fc1d4-114">Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fc1d4-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="fc1d4-115">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="fc1d4-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="fc1d4-116">Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar".</span><span class="sxs-lookup"><span data-stu-id="fc1d4-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="fc1d4-117">Descargue el instalador MSI</span><span class="sxs-lookup"><span data-stu-id="fc1d4-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
