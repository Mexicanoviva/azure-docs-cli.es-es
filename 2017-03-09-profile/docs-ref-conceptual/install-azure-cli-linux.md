---
title: "Instalación manual de la CLI de Azure 2.0 para Linux"
description: "Instalación manual de la CLI de Azure 2.0 para Linux"
keywords: CLI de Azure, instalar la CLI de Azure, azure linux, azure instalar linux
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="4055a-104">Instalación manual de la CLI de Azure 2.0 en Linux</span><span class="sxs-lookup"><span data-stu-id="4055a-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="4055a-105">Si no tiene un paquete de la CLI de Azure disponible en la distribución, siempre puede ejecutar manualmente un script de instalación para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="4055a-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manualy by running an installation script.</span></span> <span data-ttu-id="4055a-106">Si dispone de un paquete, siempre es el método de instalación recomendado.</span><span class="sxs-lookup"><span data-stu-id="4055a-106">If you do have a package available, that is always the recommended installation method.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4055a-107">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="4055a-107">Prerequisites</span></span>

<span data-ttu-id="4055a-108">Para instalar la CLI, necesitará el siguiente software disponible en el sistema:</span><span class="sxs-lookup"><span data-stu-id="4055a-108">In order to install the CLI, you will need the following software available on your system:</span></span>

* [<span data-ttu-id="4055a-109">Python 2.7 o Python 3.x</span><span class="sxs-lookup"><span data-stu-id="4055a-109">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="4055a-110">libffi</span><span class="sxs-lookup"><span data-stu-id="4055a-110">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="4055a-111">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="4055a-111">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a><span data-ttu-id="4055a-112">Instalación o actualización manual</span><span class="sxs-lookup"><span data-stu-id="4055a-112">Install or update manually</span></span>

<span data-ttu-id="4055a-113">Tanto si va a instalar como si va a actualizar la CLI, debe realizar una instalación completa.</span><span class="sxs-lookup"><span data-stu-id="4055a-113">Whether you are installing or updating the CLI, you will need to perform a full installation.</span></span> <span data-ttu-id="4055a-114">Una vez que tenga los requisitos previos, puede instalar la CLI ejecutando `curl`.</span><span class="sxs-lookup"><span data-stu-id="4055a-114">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="4055a-115">Si no tiene `curl` en el sistema o prefiere ejecutar el script, puede descargarlo y ejecutarlo localmente.</span><span class="sxs-lookup"><span data-stu-id="4055a-115">If you would prefer, or do not have `curl` on your system, you can download the script and run it locally instead.</span></span> <span data-ttu-id="4055a-116">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="4055a-116">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="4055a-117">Después de la instalación, ejecute la CLI con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="4055a-117">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="4055a-118">Solución de problemas</span><span class="sxs-lookup"><span data-stu-id="4055a-118">Troubleshooting</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="4055a-119">Error de curl "Object Moved" (objeto movido)</span><span class="sxs-lookup"><span data-stu-id="4055a-119">curl "Object Moved" error</span></span>

<span data-ttu-id="4055a-120">Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="4055a-120">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="4055a-121">Comando `az` no encontrado</span><span class="sxs-lookup"><span data-stu-id="4055a-121">`az` command not found</span></span>

<span data-ttu-id="4055a-122">Si después de la instalación no se puede ejecutar el comando, debe borrar la memoria caché del hash de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="4055a-122">After installation if you can't run the command, you may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="4055a-123">Ejecute</span><span class="sxs-lookup"><span data-stu-id="4055a-123">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="4055a-124">y compruebe si el problema se resuelve.</span><span class="sxs-lookup"><span data-stu-id="4055a-124">and see if the problem is resolved.</span></span>

<span data-ttu-id="4055a-125">Esto también puede ocurrir si no se reinició el shell después de la instalación.</span><span class="sxs-lookup"><span data-stu-id="4055a-125">This can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="4055a-126">Asegúrese de que la ubicación del comando `az` esté en `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="4055a-126">Make sure that the location of the `az` command is in your `$PATH`.</span></span>

<span data-ttu-id="4055a-127">Si ha ejecutado el script de instalación, la ruta será:</span><span class="sxs-lookup"><span data-stu-id="4055a-127">If you ran the installation script, this will be:</span></span>

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a><span data-ttu-id="4055a-128">Desinstalación manual</span><span class="sxs-lookup"><span data-stu-id="4055a-128">Unstinall manually</span></span>

<span data-ttu-id="4055a-129">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="4055a-129">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="4055a-130">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="4055a-130">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="4055a-131">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="4055a-131">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="4055a-132">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="4055a-132">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="4055a-133">Para desinstalar la CLI, puede eliminar los archivos directamente de la ubicación de instalación.</span><span class="sxs-lookup"><span data-stu-id="4055a-133">You can uninstall the CLI by directly deleting the files from the install location.</span></span> <span data-ttu-id="4055a-134">La ubicación de instalación se elige en el momento de la instalación, si realizó la instalación mediante el script `https://aka.ms/InstallAzureCLI`.</span><span class="sxs-lookup"><span data-stu-id="4055a-134">Your install location should have been chosen at the time of install, if you installed via the `https://aka.ms/InstallAzureCLI` script.</span></span> <span data-ttu-id="4055a-135">La ubicación de instalación predeterminada es `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="4055a-135">The default installation location is `$HOME`.</span></span>

<span data-ttu-id="4055a-136">En primer lugar, quite los archivos de la CLI instalados:</span><span class="sxs-lookup"><span data-stu-id="4055a-136">First, remove the installed CLI files:</span></span>

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

<span data-ttu-id="4055a-137">A continuación, modifique su archivo `$HOME/.bash_profile` para quitar la línea:</span><span class="sxs-lookup"><span data-stu-id="4055a-137">Then modify your `$HOME/.bash_profile` file to remove the line:</span></span>

```
<install location>/lib/azure-cli/az.completion
```

<span data-ttu-id="4055a-138">Y, por último, vuelva a cargar la memoria caché de comandos del shell, si utiliza una.</span><span class="sxs-lookup"><span data-stu-id="4055a-138">And finally, reload your shell's command cache if it uses one.</span></span> <span data-ttu-id="4055a-139">Los usuarios de `bash` y `zsh` tendrán que realizar este paso:</span><span class="sxs-lookup"><span data-stu-id="4055a-139">`bash` and `zsh` users will need to perform this step:</span></span>

```bash
hash -r
```
