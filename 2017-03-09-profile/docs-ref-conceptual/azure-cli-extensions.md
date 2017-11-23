---
title: Extensiones de la CLI de Azure 2.0
description: Uso de extensiones con la CLI de Azure 2.0
keywords: CLI de Azure, extensiones
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 930073324d68f9719ce5035388120e7b6ac41a98
ms.sourcegitcommit: 0149f195a0d9f0ea9b7ff5c6e00ad4242223a1a8
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/18/2017
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="44e96-104">Uso de extensiones con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="44e96-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="44e96-105">Las extensiones son módulos individuales que no se distribuyen con la propia CLI de Azure y que permiten agregar funcionalidad mediante nuevos comandos.</span><span class="sxs-lookup"><span data-stu-id="44e96-105">Extensions are individual modules not shipped with the Azure CLI itself that allow you to add functionality through new commands.</span></span> <span data-ttu-id="44e96-106">Podría tratarse de ofertas experimentales o en versión preliminar, herramientas especializadas que Microsoft tiene para sus necesidades o incluso extensiones que usted haya escrito.</span><span class="sxs-lookup"><span data-stu-id="44e96-106">These might be experimental or pre-release offerings, specialized tools that Microsoft has for your needs, or even extensions that you yourself have written.</span></span> <span data-ttu-id="44e96-107">Las extensiones aportan a la CLI un grado de flexibilidad que le permite modificarla según sus propias necesidades, sin tener que enviar una gran cantidad de paquetes adicionales que no se consideran parte del conjunto de características principales.</span><span class="sxs-lookup"><span data-stu-id="44e96-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="44e96-108">Este artículo le ayudará a aprender a instalar, actualizar y eliminar extensiones de la CLI.</span><span class="sxs-lookup"><span data-stu-id="44e96-108">This article will help you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="44e96-109">También responde a preguntas comunes sobre el comportamiento de las extensiones.</span><span class="sxs-lookup"><span data-stu-id="44e96-109">It should also answer common questions about extension behavior.</span></span>

## <a name="finding-extensions"></a><span data-ttu-id="44e96-110">Búsqueda de extensiones</span><span class="sxs-lookup"><span data-stu-id="44e96-110">Finding extensions</span></span>

<span data-ttu-id="44e96-111">Para saber qué extensiones están disponibles, puede utilizar `az extension list-available`.</span><span class="sxs-lookup"><span data-stu-id="44e96-111">In order to know what extensions are available, you can use `az extension list-available`.</span></span> <span data-ttu-id="44e96-112">Este comando enumera las extensiones disponibles oficiales proporcionadas por Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44e96-112">This command lists the available, official extensions which are provided and supported by Microsoft.</span></span>

## <a name="installing-extensions"></a><span data-ttu-id="44e96-113">Instalación de extensiones</span><span class="sxs-lookup"><span data-stu-id="44e96-113">Installing extensions</span></span>

<span data-ttu-id="44e96-114">Una vez que haya encontrado una extensión para instalar, use `az extension add` para obtenerla.</span><span class="sxs-lookup"><span data-stu-id="44e96-114">Once you have found an extension to install, use `az extension add` to get it.</span></span> <span data-ttu-id="44e96-115">Si se trata de una extensión de Microsoft oficial enumerada en `az extension list-available`, puede instalarla por nombre.</span><span class="sxs-lookup"><span data-stu-id="44e96-115">If the extension is an official Microsoft extension listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="44e96-116">Si la extensión es de un recurso externo o dispone de un vínculo directo a ella, puede proporcionar la dirección URL de origen o la ruta de acceso local.</span><span class="sxs-lookup"><span data-stu-id="44e96-116">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="44e96-117">Esto _debe_ ser un archivo wheel de Python compilado.</span><span class="sxs-lookup"><span data-stu-id="44e96-117">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="44e96-118">Cuando se instala una extensión, se puede encontrar en el valor de la variable del shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="44e96-118">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="44e96-119">Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.</span><span class="sxs-lookup"><span data-stu-id="44e96-119">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="updating-extensions"></a><span data-ttu-id="44e96-120">Actualización de extensiones</span><span class="sxs-lookup"><span data-stu-id="44e96-120">Updating extensions</span></span>

<span data-ttu-id="44e96-121">Solo se pueden actualizar las extensiones por nombre:</span><span class="sxs-lookup"><span data-stu-id="44e96-121">Extensions can only be updated by name:</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="44e96-122">Si no se puede resolver un nombre de extensión mediante la CLI por cualquier motivo, vuelva a instalar la extensión para actualizarla.</span><span class="sxs-lookup"><span data-stu-id="44e96-122">If an extension name cannot be resolved by the CLI for whatever reason, reinstall the extension to update it.</span></span> <span data-ttu-id="44e96-123">También es posible que la extensión haya dejado de estar en versión preliminar y se haya convertido en un comando integrado de la CLI.</span><span class="sxs-lookup"><span data-stu-id="44e96-123">There is also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="44e96-124">En ese caso, actualice la CLI y desinstale la extensión.</span><span class="sxs-lookup"><span data-stu-id="44e96-124">In that case, update the CLI and uninstall the extension.</span></span>

## <a name="uninstalling-extensions"></a><span data-ttu-id="44e96-125">Desinstalación de extensiones</span><span class="sxs-lookup"><span data-stu-id="44e96-125">Uninstalling extensions</span></span>

<span data-ttu-id="44e96-126">Si ya no necesita una extensión, se puede eliminar con `az extension remove`,</span><span class="sxs-lookup"><span data-stu-id="44e96-126">If you no longer need an extension, it can be removed with `az extension remove`,</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="44e96-127">También puede eliminar una extensión de forma manual mediante su eliminación de la ubicación donde se instaló.</span><span class="sxs-lookup"><span data-stu-id="44e96-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="44e96-128">Este será el valor de la variable del shell `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="44e96-128">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="44e96-129">Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.</span><span class="sxs-lookup"><span data-stu-id="44e96-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="44e96-130">Se recomienda realizar la desinstalación con `az extension remove`.</span><span class="sxs-lookup"><span data-stu-id="44e96-130">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="44e96-131">P+F</span><span class="sxs-lookup"><span data-stu-id="44e96-131">FAQ</span></span>

<span data-ttu-id="44e96-132">A continuación encontrará respuestas a otras preguntas comunes acerca de las extensiones de la CLI.</span><span class="sxs-lookup"><span data-stu-id="44e96-132">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="44e96-133">¿Qué formatos de archivo se permiten para la instalación?</span><span class="sxs-lookup"><span data-stu-id="44e96-133">What file formats are allowed for installation?</span></span>

<span data-ttu-id="44e96-134">Actualmente, solo pueden instalarse archivos wheel de Python compilados como extensiones.</span><span class="sxs-lookup"><span data-stu-id="44e96-134">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="44e96-135">¿Pueden reemplazar las extensiones a comandos existentes?</span><span class="sxs-lookup"><span data-stu-id="44e96-135">Can extensions replace existing commands?</span></span>

<span data-ttu-id="44e96-136">Sí.</span><span class="sxs-lookup"><span data-stu-id="44e96-136">Yes.</span></span> <span data-ttu-id="44e96-137">Las extensiones pueden reemplazar comandos existentes pero, antes de ejecutar un comando que se ha reemplazado, la CLI emitirá una advertencia.</span><span class="sxs-lookup"><span data-stu-id="44e96-137">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="44e96-138">¿Cómo se puede saber si una extensión está en versión preliminar?</span><span class="sxs-lookup"><span data-stu-id="44e96-138">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="44e96-139">Una extensión debe indicar si se encuentra en versión preliminar en su propia documentación y en el control de versiones.</span><span class="sxs-lookup"><span data-stu-id="44e96-139">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="44e96-140">También es común que Microsoft publique comandos de la CLI en versión preliminar como extensiones, con intención de moverlos a la interfaz principal de la CLI una vez que el producto haya dejado de estar en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="44e96-140">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="44e96-141">¿Las extensiones pueden depender entre sí?</span><span class="sxs-lookup"><span data-stu-id="44e96-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="44e96-142">No.</span><span class="sxs-lookup"><span data-stu-id="44e96-142">No.</span></span> <span data-ttu-id="44e96-143">Las extensiones deben ser paquetes individuales que no confían entre sí.</span><span class="sxs-lookup"><span data-stu-id="44e96-143">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="44e96-144">Esto es porque la CLI no ofrece ninguna garantía sobre cuándo se cargan las extensiones, por lo que no se puede garantizar que las dependencias se cumplan.</span><span class="sxs-lookup"><span data-stu-id="44e96-144">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="44e96-145">La instalación de una extensión instala solo esa extensión y debe continuar funcionando aunque elimine otras extensiones.</span><span class="sxs-lookup"><span data-stu-id="44e96-145">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="44e96-146">¿Las extensiones se actualizan junto con la CLI?</span><span class="sxs-lookup"><span data-stu-id="44e96-146">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="44e96-147">No.</span><span class="sxs-lookup"><span data-stu-id="44e96-147">No.</span></span> <span data-ttu-id="44e96-148">Las extensiones deben actualizarse por separado, tal y como se describe en la sección [Actualización de extensiones](#updating-extensions).</span><span class="sxs-lookup"><span data-stu-id="44e96-148">Extensions must be updated separately, as described in the [Updating extensions](#updating-extensions) section.</span></span>
