---
title: Extensiones de la CLI de Azure
description: Uso de extensiones con la CLI de Azure
keywords: CLI de Azure, extensiones
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0ba204063c00bf706f6af5a14dc59ba317385f95
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178123"
---
# <a name="use-extensions-with-azure-cli"></a><span data-ttu-id="3b6d3-104">Uso de extensiones con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="3b6d3-104">Use extensions with Azure CLI</span></span> 

<span data-ttu-id="3b6d3-105">La CLI de Azure ofrece la posibilidad de cargar extensiones.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-105">The Azure CLI offers the capability to load extensions.</span></span> <span data-ttu-id="3b6d3-106">Las extensiones son archivos wheel de Python que no se distribuyen como parte de la CLI, pero se ejecutan como comandos de la CLI.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-106">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="3b6d3-107">Con las extensiones, obtendrá acceso a comandos experimentales y en versión preliminar, además de poder escribir sus propias interfaces de la CLI.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-107">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="3b6d3-108">En este artículo se explica cómo administrar las extensiones y se da respuesta a preguntas comunes sobre su uso.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-108">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="3b6d3-109">Buscar extensiones</span><span class="sxs-lookup"><span data-stu-id="3b6d3-109">Find extensions</span></span>

<span data-ttu-id="3b6d3-110">Para ver las extensiones que Microsoft proporciona y mantiene, use el comando [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="3b6d3-110">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="3b6d3-111">También hospedamos una [lista de las extensiones](azure-cli-extensions-list.md) en el sitio de documentación.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-111">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="3b6d3-112">Instalar extensiones</span><span class="sxs-lookup"><span data-stu-id="3b6d3-112">Install extensions</span></span>

<span data-ttu-id="3b6d3-113">Una vez que haya encontrado una extensión para instalar, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) para obtenerla.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-113">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="3b6d3-114">Si la extensión aparece enumerada en `az extension list-available`, puede instalarla por nombre.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-114">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="3b6d3-115">Si la extensión es de un recurso externo o dispone de un vínculo directo a ella, proporcione la dirección URL de origen o la ruta de acceso local.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-115">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="3b6d3-116">La extensión _debe_ ser un archivo wheel de Python compilado.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-116">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="3b6d3-117">Cuando se instala una extensión, se encuentra en el valor de la variable `$AZURE_EXTENSION_DIR` del shell.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-117">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="3b6d3-118">Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-118">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="3b6d3-119">Actualizar extensiones</span><span class="sxs-lookup"><span data-stu-id="3b6d3-119">Update extensions</span></span>

<span data-ttu-id="3b6d3-120">Si se instaló una extensión por nombre, actualícela con [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="3b6d3-120">If an extension was installed by name, update it using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="3b6d3-121">En caso contrario, una extensión se puede actualizar desde el origen siguiendo las instrucciones de [Instalar extensiones](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="3b6d3-121">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="3b6d3-122">Si un nombre de extensión no se puede resolver mediante la CLI, desinstálela e intente volver a instalarla.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-122">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="3b6d3-123">La extensión también podría haberse vuelto parte de la CLI de base.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-123">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="3b6d3-124">Intente actualizar la CLI, tal y como se describe en [Instalación de la CLI de Azure](install-azure-cli.md) y compruebe si se agregaron los comandos de la extensión.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-124">Try updating the CLI as described in [Install the Azure CLI](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="3b6d3-125">Desinstalar extensiones</span><span class="sxs-lookup"><span data-stu-id="3b6d3-125">Uninstall extensions</span></span>

<span data-ttu-id="3b6d3-126">Si ya no necesita una extensión, quítela con [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="3b6d3-126">If you no longer need an extension, remove it with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="3b6d3-127">También puede eliminar una extensión de forma manual mediante su eliminación de la ubicación donde se instaló.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="3b6d3-128">La variable `$AZURE_EXTENSION_DIR` del shell define donde están instalados los módulos.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-128">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="3b6d3-129">Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="3b6d3-130">Preguntas más frecuentes</span><span class="sxs-lookup"><span data-stu-id="3b6d3-130">FAQ</span></span>

<span data-ttu-id="3b6d3-131">A continuación encontrará respuestas a otras preguntas comunes acerca de las extensiones de la CLI.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-131">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="3b6d3-132">¿Qué formatos de archivo se permiten para la instalación?</span><span class="sxs-lookup"><span data-stu-id="3b6d3-132">What file formats are allowed for installation?</span></span>

<span data-ttu-id="3b6d3-133">Actualmente, solo pueden instalarse archivos wheel de Python compilados como extensiones.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-133">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="3b6d3-134">¿Pueden reemplazar las extensiones a comandos existentes?</span><span class="sxs-lookup"><span data-stu-id="3b6d3-134">Can extensions replace existing commands?</span></span>

<span data-ttu-id="3b6d3-135">Sí.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-135">Yes.</span></span> <span data-ttu-id="3b6d3-136">Las extensiones pueden reemplazar comandos existentes pero, antes de ejecutar un comando que se ha reemplazado, la CLI emitirá una advertencia.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-136">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="3b6d3-137">¿Cómo se puede saber si una extensión está en versión preliminar?</span><span class="sxs-lookup"><span data-stu-id="3b6d3-137">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="3b6d3-138">La documentación y el control de versiones de una extensión mostrarán si se encuentra en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-138">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="3b6d3-139">Microsoft publica periódicamente comandos en versión preliminar como extensiones de la CLI, con la opción de trasladarlos más adelante al producto de CLI principal.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-139">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="3b6d3-140">Cuando se retiran comandos de las extensiones, se debe desinstalar la extensión anterior.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-140">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="3b6d3-141">¿Las extensiones pueden depender entre sí?</span><span class="sxs-lookup"><span data-stu-id="3b6d3-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="3b6d3-142">No.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-142">No.</span></span> <span data-ttu-id="3b6d3-143">Como la CLI no garantiza un orden de carga, puede que las dependencias no se cumplan.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-143">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="3b6d3-144">La retirada de una extensión no afectará a las demás.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-144">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="3b6d3-145">¿Las extensiones se actualizan junto con la CLI?</span><span class="sxs-lookup"><span data-stu-id="3b6d3-145">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="3b6d3-146">No.</span><span class="sxs-lookup"><span data-stu-id="3b6d3-146">No.</span></span> <span data-ttu-id="3b6d3-147">Las extensiones deben actualizarse por separado, tal y como se describe en la sección [Actualizar extensiones](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="3b6d3-147">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>
