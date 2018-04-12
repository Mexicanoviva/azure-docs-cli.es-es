---
title: Extensiones de la CLI de Azure 2.0
description: Uso de extensiones con la CLI de Azure 2.0
keywords: CLI de Azure, extensiones
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a150edbc174ff77f4320a2cb60e031dc3c6ad1cc
ms.sourcegitcommit: c9da729f4a42a839f13106f7589deaa0ca19cc4e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/06/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="bf85e-104">Uso de extensiones con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="bf85e-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="bf85e-105">Las extensiones son módulos individuales que no se distribuyen con la propia CLI de Azure y que agregan funcionalidad mediante nuevos comandos.</span><span class="sxs-lookup"><span data-stu-id="bf85e-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="bf85e-106">Podría tratarse de ofertas experimentales o de una versión preliminar, herramientas especializadas de Microsoft o características personalizadas escritas por usted.</span><span class="sxs-lookup"><span data-stu-id="bf85e-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="bf85e-107">Las extensiones aportan a la CLI un grado de flexibilidad que le permite modificarla según sus propias necesidades, sin tener que enviar una gran cantidad de paquetes adicionales que no se consideran parte del conjunto de características principales.</span><span class="sxs-lookup"><span data-stu-id="bf85e-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="bf85e-108">Este artículo le ayuda a aprender a instalar, actualizar y eliminar extensiones de la CLI.</span><span class="sxs-lookup"><span data-stu-id="bf85e-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="bf85e-109">También responde a preguntas comunes sobre el comportamiento de las extensiones.</span><span class="sxs-lookup"><span data-stu-id="bf85e-109">It also answers common questions about extension behavior.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="bf85e-110">Buscar extensiones</span><span class="sxs-lookup"><span data-stu-id="bf85e-110">Find extensions</span></span>

<span data-ttu-id="bf85e-111">Para saber qué extensiones están disponibles, puede usar [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="bf85e-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension#az-extension-list-available).</span></span> <span data-ttu-id="bf85e-112">Este comando muestra las extensiones oficiales proporcionadas y mantenidas por Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bf85e-112">This command lists the official extensions provided and maintained by Microsoft.</span></span>

```azurecli
az extension list-available --output table
```

<span data-ttu-id="bf85e-113">También hospedamos una [lista de las extensiones de Microsoft](azure-cli-extensions-list.md) en el sitio de documentación.</span><span class="sxs-lookup"><span data-stu-id="bf85e-113">We also host a [list of Microsoft extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="bf85e-114">Instalar extensiones</span><span class="sxs-lookup"><span data-stu-id="bf85e-114">Install extensions</span></span>

<span data-ttu-id="bf85e-115">Una vez que haya encontrado una extensión para instalar, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-add) para obtenerla.</span><span class="sxs-lookup"><span data-stu-id="bf85e-115">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="bf85e-116">Si la extensión aparece enumerada en `az extension list-available`, puede instalarla por nombre.</span><span class="sxs-lookup"><span data-stu-id="bf85e-116">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="bf85e-117">Si la extensión es de un recurso externo o dispone de un vínculo directo a ella, puede proporcionar la dirección URL de origen o la ruta de acceso local.</span><span class="sxs-lookup"><span data-stu-id="bf85e-117">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="bf85e-118">Esto _debe_ ser un archivo wheel de Python compilado.</span><span class="sxs-lookup"><span data-stu-id="bf85e-118">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="bf85e-119">Cuando se instala una extensión, se puede encontrar en el valor de la variable del shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="bf85e-119">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="bf85e-120">Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.</span><span class="sxs-lookup"><span data-stu-id="bf85e-120">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="bf85e-121">Actualizar extensiones</span><span class="sxs-lookup"><span data-stu-id="bf85e-121">Update extensions</span></span>

<span data-ttu-id="bf85e-122">Si se instaló una extensión por nombre, se puede actualizar con [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="bf85e-122">If an extension was installed by name, it can be updated using [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="bf85e-123">En caso contrario, una extensión se puede actualizar desde el origen siguiendo las instrucciones de [Instalar extensiones](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="bf85e-123">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="bf85e-124">Si un nombre de extensión no se puede resolver mediante la CLI, desinstálela e intente volver a instalarla.</span><span class="sxs-lookup"><span data-stu-id="bf85e-124">If an extension name cannot be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="bf85e-125">También es posible que la extensión haya dejado de estar en versión preliminar y se haya convertido en un comando integrado de la CLI.</span><span class="sxs-lookup"><span data-stu-id="bf85e-125">There's also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="bf85e-126">Intente actualizar la CLI, tal y como se describe en [Instalación de la CLI de Azure 2.0](install-azure-cli.md) y vea si se agregaron los comandos de la extensión.</span><span class="sxs-lookup"><span data-stu-id="bf85e-126">Try updating the CLI as described in [Install the Azure CLI 2.0](install-azure-cli.md) and see if the extension's commands were added.</span></span> 

## <a name="uninstall-extensions"></a><span data-ttu-id="bf85e-127">Desinstalar extensiones</span><span class="sxs-lookup"><span data-stu-id="bf85e-127">Uninstall extensions</span></span>

<span data-ttu-id="bf85e-128">Si ya no necesita una extensión, se puede eliminar con [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="bf85e-128">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-remove).</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="bf85e-129">También puede eliminar una extensión de forma manual mediante su eliminación de la ubicación donde se instaló.</span><span class="sxs-lookup"><span data-stu-id="bf85e-129">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="bf85e-130">Este será el valor de la variable del shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="bf85e-130">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="bf85e-131">Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.</span><span class="sxs-lookup"><span data-stu-id="bf85e-131">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="bf85e-132">Se recomienda realizar la desinstalación con `az extension remove`.</span><span class="sxs-lookup"><span data-stu-id="bf85e-132">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="bf85e-133">Preguntas más frecuentes</span><span class="sxs-lookup"><span data-stu-id="bf85e-133">FAQ</span></span>

<span data-ttu-id="bf85e-134">A continuación encontrará respuestas a otras preguntas comunes acerca de las extensiones de la CLI.</span><span class="sxs-lookup"><span data-stu-id="bf85e-134">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="bf85e-135">¿Qué formatos de archivo se permiten para la instalación?</span><span class="sxs-lookup"><span data-stu-id="bf85e-135">What file formats are allowed for installation?</span></span>

<span data-ttu-id="bf85e-136">Actualmente, solo pueden instalarse archivos wheel de Python compilados como extensiones.</span><span class="sxs-lookup"><span data-stu-id="bf85e-136">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="bf85e-137">¿Pueden reemplazar las extensiones a comandos existentes?</span><span class="sxs-lookup"><span data-stu-id="bf85e-137">Can extensions replace existing commands?</span></span>

<span data-ttu-id="bf85e-138">Sí.</span><span class="sxs-lookup"><span data-stu-id="bf85e-138">Yes.</span></span> <span data-ttu-id="bf85e-139">Las extensiones pueden reemplazar comandos existentes pero, antes de ejecutar un comando que se ha reemplazado, la CLI emitirá una advertencia.</span><span class="sxs-lookup"><span data-stu-id="bf85e-139">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="bf85e-140">¿Cómo se puede saber si una extensión está en versión preliminar?</span><span class="sxs-lookup"><span data-stu-id="bf85e-140">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="bf85e-141">Una extensión debe indicar si se encuentra en versión preliminar en su propia documentación y en el control de versiones.</span><span class="sxs-lookup"><span data-stu-id="bf85e-141">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="bf85e-142">También es común que Microsoft publique comandos de la CLI en versión preliminar como extensiones, con intención de moverlos a la interfaz principal de la CLI una vez que el producto haya dejado de estar en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="bf85e-142">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="bf85e-143">¿Las extensiones pueden depender entre sí?</span><span class="sxs-lookup"><span data-stu-id="bf85e-143">Can extensions depend upon each other?</span></span>

<span data-ttu-id="bf85e-144">Nº</span><span class="sxs-lookup"><span data-stu-id="bf85e-144">No.</span></span> <span data-ttu-id="bf85e-145">Las extensiones deben ser paquetes individuales que no confían entre sí.</span><span class="sxs-lookup"><span data-stu-id="bf85e-145">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="bf85e-146">Esto es porque la CLI no ofrece ninguna garantía sobre cuándo se cargan las extensiones, por lo que no se puede garantizar que las dependencias se cumplan.</span><span class="sxs-lookup"><span data-stu-id="bf85e-146">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="bf85e-147">La instalación de una extensión instala solo esa extensión y debe continuar funcionando aunque elimine otras extensiones.</span><span class="sxs-lookup"><span data-stu-id="bf85e-147">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="bf85e-148">¿Las extensiones se actualizan junto con la CLI?</span><span class="sxs-lookup"><span data-stu-id="bf85e-148">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="bf85e-149">Nº</span><span class="sxs-lookup"><span data-stu-id="bf85e-149">No.</span></span> <span data-ttu-id="bf85e-150">Las extensiones deben actualizarse por separado, tal y como se describe en la sección [Actualizar extensiones](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="bf85e-150">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>
