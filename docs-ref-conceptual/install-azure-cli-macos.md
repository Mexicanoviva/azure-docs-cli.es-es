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
ms.openlocfilehash: 790c63a60a5d23863b48227dcc99462bbf950d80
ms.sourcegitcommit: b42ce26476b135bb2047c8d9d787580c858f8b6b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/09/2019
ms.locfileid: "72163850"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="47131-103">Instalación de la CLI de Azure en macOS</span><span class="sxs-lookup"><span data-stu-id="47131-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="47131-104">Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="47131-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="47131-105">Homebrew facilita mantener actualizada la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="47131-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="47131-106">El paquete de la CLI se ha probado en las versiones de Mac OS 10.9 y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="47131-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a><span data-ttu-id="47131-107">Instalación con Homebrew</span><span class="sxs-lookup"><span data-stu-id="47131-107">Install with Homebrew</span></span>

<span data-ttu-id="47131-108">Homebrew es la manera más fácil de administrar la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="47131-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="47131-109">Ofrece formas cómodas de instalar, actualizar y desinstalar.</span><span class="sxs-lookup"><span data-stu-id="47131-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="47131-110">Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="47131-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="47131-111">Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:</span><span class="sxs-lookup"><span data-stu-id="47131-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="47131-112">La CLI de Azure tiene una dependencia en el paquete `python3` de Homebrew, y lo instalará.</span><span class="sxs-lookup"><span data-stu-id="47131-112">The Azure CLI has a dependency on the Homebrew `python3` package, and will install it.</span></span>
> <span data-ttu-id="47131-113">Se garantiza que la CLI de Azure será compatible con la versión más reciente de `python3` publicada en Homebrew.</span><span class="sxs-lookup"><span data-stu-id="47131-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="47131-114">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="47131-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="47131-115">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="47131-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="47131-116">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="47131-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="47131-117">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="47131-117">Troubleshooting</span></span>

<span data-ttu-id="47131-118">Si se produce un problema al instalar la CLI a través de Homebrew, aquí se muestran algunos errores comunes.</span><span class="sxs-lookup"><span data-stu-id="47131-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="47131-119">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="47131-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="47131-120">No se puede encontrar Python o los paquetes instalados</span><span class="sxs-lookup"><span data-stu-id="47131-120">Unable to find Python or installed packages</span></span>

<span data-ttu-id="47131-121">Puede haber una discrepancia con la versión secundaria u otros problemas durante la instalación de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="47131-121">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="47131-122">La CLI no usa un entorno virtual de Python y debe buscar la versión de Python instalada.</span><span class="sxs-lookup"><span data-stu-id="47131-122">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="47131-123">Una posible solución consiste en instalar y volver a vincular la dependencia de `python3` desde Homebrew.</span><span class="sxs-lookup"><span data-stu-id="47131-123">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="47131-124">Versión de la CLI 1.x instalada</span><span class="sxs-lookup"><span data-stu-id="47131-124">CLI version 1.x is installed</span></span>

<span data-ttu-id="47131-125">Si se instaló una versión no actualizada, podría deberse a que la memoria caché de Homebrew estaba obsoleta.</span><span class="sxs-lookup"><span data-stu-id="47131-125">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="47131-126">Siga las instrucciones de [actualización](#update).</span><span class="sxs-lookup"><span data-stu-id="47131-126">Follow the [update](#update) instructions.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="47131-127">Conexión de bloques proxy</span><span class="sxs-lookup"><span data-stu-id="47131-127">Proxy blocks connection</span></span>

<span data-ttu-id="47131-128">No puede obtener recursos de Homebrew, a menos que lo haya configurado correctamente para usar el servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="47131-128">You may be unable to get resources from Homebrew unless you have correctly configured it to use your proxy.</span></span> <span data-ttu-id="47131-129">Siga las [instrucciones de configuración del servidor proxy de Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span><span class="sxs-lookup"><span data-stu-id="47131-129">Follow the [Homebrew proxy configuration instructions](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="47131-130">Si está detrás de un servidor proxy, `HTTP_PROXY` y `HTTPS_PROXY` deben establecerse para conectarse a los servicios de Azure con la CLI.</span><span class="sxs-lookup"><span data-stu-id="47131-130">If you are behind a proxy, `HTTP_PROXY` and `HTTPS_PROXY` must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="47131-131">Si no utiliza autenticación básica, se recomienda exportar estas variables en su archivo `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="47131-131">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="47131-132">Siga siempre las directivas de seguridad de su empresa y los requisitos del administrador del sistema.</span><span class="sxs-lookup"><span data-stu-id="47131-132">Always follow your business' security policies and the requirements of your system administrator.</span></span>

<span data-ttu-id="47131-133">Para obtener los recursos Bottle de Homebrew, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:</span><span class="sxs-lookup"><span data-stu-id="47131-133">In order to get the bottle resources from Homebrew, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a><span data-ttu-id="47131-134">Actualizar</span><span class="sxs-lookup"><span data-stu-id="47131-134">Update</span></span>

<span data-ttu-id="47131-135">La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="47131-135">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="47131-136">Hay una nueva versión disponible aproximadamente cada dos semanas.</span><span class="sxs-lookup"><span data-stu-id="47131-136">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="47131-137">Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="47131-137">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="47131-138">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="47131-138">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="47131-139">Use Homebrew para desinstalar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="47131-139">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="47131-140">Otros métodos de instalación</span><span class="sxs-lookup"><span data-stu-id="47131-140">Other installation methods</span></span>

<span data-ttu-id="47131-141">Si no puede usar Homebrew para instalar la CLI de Azure en su entorno, es posible usar las instrucciones manuales para Linux.</span><span class="sxs-lookup"><span data-stu-id="47131-141">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="47131-142">Tenga en cuenta que este proceso no se mantiene oficialmente para que sea compatible con macOS.</span><span class="sxs-lookup"><span data-stu-id="47131-142">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="47131-143">Siempre se recomienda usar un administrador de paquetes como Homebrew.</span><span class="sxs-lookup"><span data-stu-id="47131-143">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="47131-144">Solo debe usar el método de instalación manual si no dispone de ninguna otra opción.</span><span class="sxs-lookup"><span data-stu-id="47131-144">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="47131-145">Para las instrucciones de instalación manual, consulte [Instalación de la CLI de Azure en Linux manualmente](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="47131-145">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="47131-146">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="47131-146">Next Steps</span></span>

<span data-ttu-id="47131-147">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="47131-147">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="47131-148">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="47131-148">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
