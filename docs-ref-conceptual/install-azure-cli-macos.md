---
title: "Instalación de la CLI de Azure para macOS"
description: "Instalación de la CLI de Azure 2.0 en macOS"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0295846abc2fe6091940824c6efc47b8fd64ce9f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="33c1f-103">Instalación de la CLI de Azure 2.0 en macOS</span><span class="sxs-lookup"><span data-stu-id="33c1f-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="33c1f-104">Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](http://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="33c1f-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="33c1f-105">Homebrew facilita mantener actualizada la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="33c1f-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="33c1f-106">El paquete de la CLI se ha probado en las versiones de Mac OS 10.9 y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="33c1f-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="33c1f-107">Instalación</span><span class="sxs-lookup"><span data-stu-id="33c1f-107">Install</span></span>

<span data-ttu-id="33c1f-108">Homebrew es la manera más fácil de administrar la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="33c1f-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="33c1f-109">Ofrece formas cómodas de instalar, actualizar y desinstalar.</span><span class="sxs-lookup"><span data-stu-id="33c1f-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="33c1f-110">Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="33c1f-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="33c1f-111">Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:</span><span class="sxs-lookup"><span data-stu-id="33c1f-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="33c1f-112">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="33c1f-112">You can then run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="33c1f-113">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="33c1f-113">Troubleshooting</span></span>

<span data-ttu-id="33c1f-114">Si se produce un problema al instalar la CLI a través de Homebrew, aquí se muestran algunos errores comunes.</span><span class="sxs-lookup"><span data-stu-id="33c1f-114">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="33c1f-115">Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="33c1f-115">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="33c1f-116">No se puede encontrar Python o los paquetes instalados</span><span class="sxs-lookup"><span data-stu-id="33c1f-116">Unable to find Python or installed packages</span></span>

<span data-ttu-id="33c1f-117">Si la instalación no puede encontrar Python o los paquetes instalados, podría deberse a una diferencia de versión secundaria o a otro problema que se produjo durante la instalación de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="33c1f-117">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="33c1f-118">Como la CLI no usa un entorno virtual de Python, depende de que pueda encontrar la versión correcta de Python.</span><span class="sxs-lookup"><span data-stu-id="33c1f-118">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="33c1f-119">Para corregir estos problemas, puede volver a vincular la instalación de Python.</span><span class="sxs-lookup"><span data-stu-id="33c1f-119">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="33c1f-120">Versión de la CLI 1.x instalada</span><span class="sxs-lookup"><span data-stu-id="33c1f-120">CLI version 1.x is installed</span></span>

<span data-ttu-id="33c1f-121">Si se instaló una versión no actualizada, podría deberse a una memoria caché de Homebrew obsoleta.</span><span class="sxs-lookup"><span data-stu-id="33c1f-121">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="33c1f-122">Siga las instrucciones de [actualización](#Update).</span><span class="sxs-lookup"><span data-stu-id="33c1f-122">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="33c1f-123">Actualizar</span><span class="sxs-lookup"><span data-stu-id="33c1f-123">Update</span></span>

<span data-ttu-id="33c1f-124">La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="33c1f-124">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="33c1f-125">Hay una nueva versión disponible aproximadamente cada dos semanas.</span><span class="sxs-lookup"><span data-stu-id="33c1f-125">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="33c1f-126">Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="33c1f-126">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="33c1f-127">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="33c1f-127">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="33c1f-128">Use Homebrew para desinstalar el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="33c1f-128">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
