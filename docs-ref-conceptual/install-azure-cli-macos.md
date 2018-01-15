---
title: "Instalación de la CLI de Azure para macOS"
description: "Instalación de la CLI de Azure 2.0 en macOS"
keywords: CLI de Azure, instalar la CLI de Azure, azure linux, azure instalar macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="38081-104">Instalación de la CLI de Azure 2.0 en macOS</span><span class="sxs-lookup"><span data-stu-id="38081-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="38081-105">Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](http://brew.sh), o manualmente.</span><span class="sxs-lookup"><span data-stu-id="38081-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh) or manually.</span></span> <span data-ttu-id="38081-106">El método de instalación recomendado es con Homebrew, para que sea más fácil instalarlo, obtener actualizaciones y desinstalarlo, si lo necesita.</span><span class="sxs-lookup"><span data-stu-id="38081-106">The preferred installation method is through homebrew, so that it's easier to install, get updates, and uninstall if you need to.</span></span>

## <a name="use-homebrew-to-install"></a><span data-ttu-id="38081-107">Utilice Homebrew para la instalación</span><span class="sxs-lookup"><span data-stu-id="38081-107">Use homebrew to install</span></span>

<span data-ttu-id="38081-108">Homebrew es la manera más fácil de administrar la instalación de la CLI.</span><span class="sxs-lookup"><span data-stu-id="38081-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="38081-109">Ofrece formas cómodas de instalar, actualizar y desinstalar.</span><span class="sxs-lookup"><span data-stu-id="38081-109">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="38081-110">Es similar a otros administradores de paquetes como `apt` o `yum`.</span><span class="sxs-lookup"><span data-stu-id="38081-110">It's similar to other package managers such as `apt` or `yum`.</span></span>
<span data-ttu-id="38081-111">Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="38081-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="38081-112">Instalación con Homebrew</span><span class="sxs-lookup"><span data-stu-id="38081-112">Install with homebrew</span></span>

<span data-ttu-id="38081-113">Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:</span><span class="sxs-lookup"><span data-stu-id="38081-113">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="38081-114">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="38081-114">You can then run the Azure CLI with the `az` command.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="38081-115">Actualización con Homebrew</span><span class="sxs-lookup"><span data-stu-id="38081-115">Update with homebrew</span></span>

<span data-ttu-id="38081-116">La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="38081-116">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="38081-117">Hay una nueva versión disponible aproximadamente cada dos semanas.</span><span class="sxs-lookup"><span data-stu-id="38081-117">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="38081-118">Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete de la CLI.</span><span class="sxs-lookup"><span data-stu-id="38081-118">You will need to update your local repository information, and then update the CLI package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a><span data-ttu-id="38081-119">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="38081-119">Troubleshooting</span></span>

<span data-ttu-id="38081-120">¿Se encontró un problema al instalar o actualizar la CLI con Homebrew?</span><span class="sxs-lookup"><span data-stu-id="38081-120">Did you encounter a problem when installing or updating the CLI with homebrew?</span></span> <span data-ttu-id="38081-121">Estos son algunos errores comunes que pueden producirse y métodos para diagnosticar y solucionarlos.</span><span class="sxs-lookup"><span data-stu-id="38081-121">Here are some common errors that might occur, and ways to diagnose and resolve them.</span></span>

#### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="38081-122">No se puede encontrar Python o los paquetes instalados</span><span class="sxs-lookup"><span data-stu-id="38081-122">Unable to find Python or installed packages</span></span>

<span data-ttu-id="38081-123">Si la instalación no puede encontrar Python o los paquetes instalados, podría deberse a una diferencia de versión secundaria o a otro problema que se produjo durante la instalación de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="38081-123">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue which occurred during homebrew installation.</span></span> <span data-ttu-id="38081-124">Como la CLI no usa un entorno virtual, depende de que pueda encontrar las versiones correctas de Python instaladas por Homebrew.</span><span class="sxs-lookup"><span data-stu-id="38081-124">Since the CLI does not use a virtualenv, it relies on being able to find correct versions of Python installed by homebrew.</span></span> <span data-ttu-id="38081-125">Para corregir estos problemas, puede volver a vincular la instalación de Python:</span><span class="sxs-lookup"><span data-stu-id="38081-125">You may be able to fix these issues by re-linking your Python installation:</span></span>

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a><span data-ttu-id="38081-126">La versión de la CLI no está actualizada</span><span class="sxs-lookup"><span data-stu-id="38081-126">The CLI version is out of date</span></span>

<span data-ttu-id="38081-127">Si cree que la versión de la CLI que hay instalada podría estar obsoleta, debe ejecutar un comando `brew update`, seguido de `brew upgrade azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="38081-127">If you think that your installed CLI version might be out of date, you will need to run a `brew update` command, followed by `brew upgrade azure-cli`.</span></span> <span data-ttu-id="38081-128">Si la CLI no se actualiza, tenga en cuenta que los paquetes de Homebrew se lanzan más lentamente que las versiones generales.</span><span class="sxs-lookup"><span data-stu-id="38081-128">If this does not update the CLI, be aware that homebrew packages may roll out more slowly than general releases.</span></span> <span data-ttu-id="38081-129">Si necesita las instalaciones más recientes de la CLI, debe [instalar manualmente](#manage-the-cli-manually).</span><span class="sxs-lookup"><span data-stu-id="38081-129">If you require bleeding-edge installs of the CLI, then you should [install manually](#manage-the-cli-manually).</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="38081-130">Desinstalación con Homebrew</span><span class="sxs-lookup"><span data-stu-id="38081-130">Uninstall with homebrew</span></span>

<span data-ttu-id="38081-131">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="38081-131">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="38081-132">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="38081-132">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="38081-133">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="38081-133">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="38081-134">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="38081-134">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="38081-135">Si instaló con Homebrew, debe usarlo también para desinstalar.</span><span class="sxs-lookup"><span data-stu-id="38081-135">If you installed with homebrew, you should also use it to uninstall.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a><span data-ttu-id="38081-136">Instalación manual de la CLI</span><span class="sxs-lookup"><span data-stu-id="38081-136">Install the CLI manually</span></span>

<span data-ttu-id="38081-137">Si no puede o no desea que Homebrew administre la instalación de la CLI automáticamente, puede instalarla manualmente.</span><span class="sxs-lookup"><span data-stu-id="38081-137">If you can't or don't want to rely on homebrew to manage the CLI install for you, then you can manually install.</span></span>

<span data-ttu-id="38081-138">Siga las [instrucciones de instalación manual de Linux](install-azure-cli-linux.md) para instalar manualmente en macOS.</span><span class="sxs-lookup"><span data-stu-id="38081-138">Follow the [manual Linux installation instructions](install-azure-cli-linux.md) to install manually on macOS.</span></span> <span data-ttu-id="38081-139">macOS 10.9 y las versiones posteriores deben incluir todas las dependencias necesarias.</span><span class="sxs-lookup"><span data-stu-id="38081-139">macOS versions 10.9 and later should include all of the required dependencies.</span></span>
