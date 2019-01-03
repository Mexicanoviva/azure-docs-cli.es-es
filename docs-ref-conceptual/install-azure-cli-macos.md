---
title: Instalación de la CLI de Azure para macOS
description: Cómo instalar la CLI de Azure en macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 40415bc7bec056dc1564c58c8df3f7263bee348c
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593173"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="a2859-103">Instalación de la CLI de Azure en macOS</span><span class="sxs-lookup"><span data-stu-id="a2859-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="a2859-104">Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="a2859-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="a2859-105">Homebrew facilita mantener actualizada la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="a2859-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="a2859-106">El paquete de la CLI se ha probado en las versiones de Mac OS 10.9 y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="a2859-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="a2859-107">Instalación</span><span class="sxs-lookup"><span data-stu-id="a2859-107">Install</span></span>

<span data-ttu-id="a2859-108">Homebrew es la manera más fácil de administrar la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="a2859-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="a2859-109">Ofrece formas cómodas de instalar, actualizar y desinstalar.</span><span class="sxs-lookup"><span data-stu-id="a2859-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="a2859-110">Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="a2859-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="a2859-111">Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:</span><span class="sxs-lookup"><span data-stu-id="a2859-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="a2859-112">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="a2859-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="a2859-113">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="a2859-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="a2859-114">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a2859-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="a2859-115">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="a2859-115">Troubleshooting</span></span>

<span data-ttu-id="a2859-116">Si se produce un problema al instalar la CLI a través de Homebrew, aquí se muestran algunos errores comunes.</span><span class="sxs-lookup"><span data-stu-id="a2859-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="a2859-117">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="a2859-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="a2859-118">No se puede encontrar Python o los paquetes instalados</span><span class="sxs-lookup"><span data-stu-id="a2859-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="a2859-119">Puede haber una discrepancia con la versión secundaria u otros problemas durante la instalación de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="a2859-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="a2859-120">La CLI no usa un entorno virtual de Python y debe buscar la versión de Python instalada.</span><span class="sxs-lookup"><span data-stu-id="a2859-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="a2859-121">Una posible solución consiste en instalar y volver a vincular la dependencia de `python3` desde Homebrew.</span><span class="sxs-lookup"><span data-stu-id="a2859-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="a2859-122">Versión de la CLI 1.x instalada</span><span class="sxs-lookup"><span data-stu-id="a2859-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="a2859-123">Si se instaló una versión no actualizada, podría deberse a que la memoria caché de Homebrew estaba obsoleta.</span><span class="sxs-lookup"><span data-stu-id="a2859-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="a2859-124">Siga las instrucciones de [actualización](#Update).</span><span class="sxs-lookup"><span data-stu-id="a2859-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="a2859-125">Actualizar</span><span class="sxs-lookup"><span data-stu-id="a2859-125">Update</span></span>

<span data-ttu-id="a2859-126">La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="a2859-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="a2859-127">Hay una nueva versión disponible aproximadamente cada dos semanas.</span><span class="sxs-lookup"><span data-stu-id="a2859-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="a2859-128">Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="a2859-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="a2859-129">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="a2859-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="a2859-130">Use Homebrew para desinstalar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="a2859-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="a2859-131">Otros métodos de instalación</span><span class="sxs-lookup"><span data-stu-id="a2859-131">Other installation methods</span></span>

<span data-ttu-id="a2859-132">Si no puede usar Homebrew para instalar la CLI de Azure en su entorno, es posible usar las instrucciones manuales para Linux.</span><span class="sxs-lookup"><span data-stu-id="a2859-132">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="a2859-133">Tenga en cuenta que este proceso no se mantiene oficialmente para que sea compatible con macOS.</span><span class="sxs-lookup"><span data-stu-id="a2859-133">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="a2859-134">Siempre se recomienda usar un administrador de paquetes como Homebrew.</span><span class="sxs-lookup"><span data-stu-id="a2859-134">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="a2859-135">Solo debe usar el método de instalación manual si no dispone de ninguna otra opción.</span><span class="sxs-lookup"><span data-stu-id="a2859-135">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="a2859-136">Para las instrucciones de instalación manual, consulte [Instalación de la CLI de Azure en Linux manualmente](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="a2859-136">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a2859-137">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="a2859-137">Next Steps</span></span>

<span data-ttu-id="a2859-138">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="a2859-138">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a2859-139">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="a2859-139">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
