---
title: Instalación de la CLI de Azure para macOS
description: Instalación de la CLI de Azure 2.0 en macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: e8190ba91006bd6d83eb0ef90b492ee7df4dda4c
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439914"
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="643e5-103">Instalación de la CLI de Azure 2.0 en macOS</span><span class="sxs-lookup"><span data-stu-id="643e5-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="643e5-104">Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](http://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="643e5-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="643e5-105">Homebrew facilita mantener actualizada la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="643e5-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="643e5-106">El paquete de la CLI se ha probado en las versiones de Mac OS 10.9 y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="643e5-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="643e5-107">Instalación</span><span class="sxs-lookup"><span data-stu-id="643e5-107">Install</span></span>

<span data-ttu-id="643e5-108">Homebrew es la manera más fácil de administrar la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="643e5-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="643e5-109">Ofrece formas cómodas de instalar, actualizar y desinstalar.</span><span class="sxs-lookup"><span data-stu-id="643e5-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="643e5-110">Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="643e5-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="643e5-111">Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:</span><span class="sxs-lookup"><span data-stu-id="643e5-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="643e5-112">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="643e5-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="643e5-113">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="643e5-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="643e5-114">Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="643e5-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="643e5-115">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="643e5-115">Troubleshooting</span></span>

<span data-ttu-id="643e5-116">Si se produce un problema al instalar la CLI a través de Homebrew, aquí se muestran algunos errores comunes.</span><span class="sxs-lookup"><span data-stu-id="643e5-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="643e5-117">Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="643e5-117">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="643e5-118">No se puede encontrar Python o los paquetes instalados</span><span class="sxs-lookup"><span data-stu-id="643e5-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="643e5-119">Si la instalación no puede encontrar Python o los paquetes instalados, podría deberse a una diferencia de versión secundaria o a otro problema que se produjo durante la instalación de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="643e5-119">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="643e5-120">Como la CLI no usa un entorno virtual de Python, depende de que pueda encontrar la versión correcta de Python.</span><span class="sxs-lookup"><span data-stu-id="643e5-120">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="643e5-121">Para corregir estos problemas, puede volver a vincular la instalación de Python.</span><span class="sxs-lookup"><span data-stu-id="643e5-121">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="643e5-122">Versión de la CLI 1.x instalada</span><span class="sxs-lookup"><span data-stu-id="643e5-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="643e5-123">Si se instaló una versión no actualizada, podría deberse a una memoria caché de Homebrew obsoleta.</span><span class="sxs-lookup"><span data-stu-id="643e5-123">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="643e5-124">Siga las instrucciones de [actualización](#Update).</span><span class="sxs-lookup"><span data-stu-id="643e5-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="643e5-125">Actualizar</span><span class="sxs-lookup"><span data-stu-id="643e5-125">Update</span></span>

<span data-ttu-id="643e5-126">La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="643e5-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="643e5-127">Hay una nueva versión disponible aproximadamente cada dos semanas.</span><span class="sxs-lookup"><span data-stu-id="643e5-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="643e5-128">Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="643e5-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="643e5-129">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="643e5-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="643e5-130">Use Homebrew para desinstalar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="643e5-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
