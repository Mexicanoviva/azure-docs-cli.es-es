---
title: Instalación de la CLI de Azure para macOS
description: Cómo instalar la CLI de Azure en macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9eb816ef68d24d1dbbaaeb5fd4877580edbe87ad
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177664"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="ff72e-103">Instalación de la CLI de Azure en macOS</span><span class="sxs-lookup"><span data-stu-id="ff72e-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="ff72e-104">Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="ff72e-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="ff72e-105">Homebrew facilita mantener actualizada la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="ff72e-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="ff72e-106">El paquete de la CLI se ha probado en las versiones de Mac OS 10.9 y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="ff72e-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="ff72e-107">Instalación</span><span class="sxs-lookup"><span data-stu-id="ff72e-107">Install</span></span>

<span data-ttu-id="ff72e-108">Homebrew es la manera más fácil de administrar la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="ff72e-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="ff72e-109">Ofrece formas cómodas de instalar, actualizar y desinstalar.</span><span class="sxs-lookup"><span data-stu-id="ff72e-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="ff72e-110">Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="ff72e-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="ff72e-111">Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:</span><span class="sxs-lookup"><span data-stu-id="ff72e-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="ff72e-112">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="ff72e-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ff72e-113">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="ff72e-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ff72e-114">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ff72e-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ff72e-115">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="ff72e-115">Troubleshooting</span></span>

<span data-ttu-id="ff72e-116">Si se produce un problema al instalar la CLI a través de Homebrew, aquí se muestran algunos errores comunes.</span><span class="sxs-lookup"><span data-stu-id="ff72e-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="ff72e-117">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ff72e-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="ff72e-118">No se puede encontrar Python o los paquetes instalados</span><span class="sxs-lookup"><span data-stu-id="ff72e-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="ff72e-119">Puede haber una discrepancia con la versión secundaria u otros problemas durante la instalación de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="ff72e-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="ff72e-120">La CLI no usa un entorno virtual de Python y debe buscar la versión de Python instalada.</span><span class="sxs-lookup"><span data-stu-id="ff72e-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="ff72e-121">Una posible solución consiste en instalar y volver a vincular la dependencia de `python3` desde Homebrew.</span><span class="sxs-lookup"><span data-stu-id="ff72e-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="ff72e-122">Versión de la CLI 1.x instalada</span><span class="sxs-lookup"><span data-stu-id="ff72e-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="ff72e-123">Si se instaló una versión no actualizada, podría deberse a que la memoria caché de Homebrew estaba obsoleta.</span><span class="sxs-lookup"><span data-stu-id="ff72e-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="ff72e-124">Siga las instrucciones de [actualización](#Update).</span><span class="sxs-lookup"><span data-stu-id="ff72e-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="ff72e-125">Actualizar</span><span class="sxs-lookup"><span data-stu-id="ff72e-125">Update</span></span>

<span data-ttu-id="ff72e-126">La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="ff72e-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="ff72e-127">Hay una nueva versión disponible aproximadamente cada dos semanas.</span><span class="sxs-lookup"><span data-stu-id="ff72e-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="ff72e-128">Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="ff72e-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="ff72e-129">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="ff72e-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="ff72e-130">Use Homebrew para desinstalar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="ff72e-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="ff72e-131">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="ff72e-131">Next Steps</span></span>

<span data-ttu-id="ff72e-132">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="ff72e-132">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ff72e-133">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="ff72e-133">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
