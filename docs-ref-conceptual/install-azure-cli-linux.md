---
title: "Instalación manual de la CLI de Azure 2.0 para Linux"
description: "Instalación manual de la CLI de Azure 2.0 para Linux"
keywords: CLI de Azure, instalar la CLI de Azure, azure linux, azure instalar linux
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: d8c88d111c50a3cbb6b643a14dcd2a9773699657
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="4efdd-104">Instalación manual de la CLI de Azure 2.0 en Linux</span><span class="sxs-lookup"><span data-stu-id="4efdd-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="4efdd-105">Si no tiene un paquete de la CLI de Azure disponible en la distribución, siempre puede ejecutar manualmente un script de instalación para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="4efdd-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="4efdd-106">Se recomienda utilizar un administrador de paquetes para la CLI.</span><span class="sxs-lookup"><span data-stu-id="4efdd-106">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="4efdd-107">Con un administrador de paquetes se asegura de que siempre tendrá las últimas actualizaciones y garantiza la estabilidad de los componentes de la CLI.</span><span class="sxs-lookup"><span data-stu-id="4efdd-107">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="4efdd-108">Compruebe si existe un paquete para su distribución antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="4efdd-108">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4efdd-109">requisitos previos</span><span class="sxs-lookup"><span data-stu-id="4efdd-109">Prerequisites</span></span>

<span data-ttu-id="4efdd-110">Para instalar la CLI, necesita el siguiente software disponible en el sistema:</span><span class="sxs-lookup"><span data-stu-id="4efdd-110">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="4efdd-111">Python 2.7 o Python 3.x</span><span class="sxs-lookup"><span data-stu-id="4efdd-111">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="4efdd-112">libffi</span><span class="sxs-lookup"><span data-stu-id="4efdd-112">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="4efdd-113">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="4efdd-113">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="4efdd-114">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="4efdd-114">Install or update</span></span> 

<span data-ttu-id="4efdd-115">Tanto si va a instalar como si va a actualizar la CLI, debe realizar una instalación completa.</span><span class="sxs-lookup"><span data-stu-id="4efdd-115">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="4efdd-116">Una vez que tenga los requisitos previos, puede instalar la CLI ejecutando `curl`.</span><span class="sxs-lookup"><span data-stu-id="4efdd-116">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="4efdd-117">También puede descargar el script y ejecutarlo localmente.</span><span class="sxs-lookup"><span data-stu-id="4efdd-117">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="4efdd-118">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="4efdd-118">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="4efdd-119">Después de la instalación, ejecute la CLI con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="4efdd-119">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="4efdd-120">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="4efdd-120">Troubleshooting</span></span>

<span data-ttu-id="4efdd-121">Estos son algunos problemas comunes que se han observado durante la instalación manual.</span><span class="sxs-lookup"><span data-stu-id="4efdd-121">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="4efdd-122">Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="4efdd-122">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>
### <a name="curl-object-moved-error"></a><span data-ttu-id="4efdd-123">Error de curl "Object Moved" (objeto movido)</span><span class="sxs-lookup"><span data-stu-id="4efdd-123">curl "Object Moved" error</span></span>

<span data-ttu-id="4efdd-124">Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="4efdd-124">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="4efdd-125">Comando `az` no encontrado</span><span class="sxs-lookup"><span data-stu-id="4efdd-125">`az` command not found</span></span>

<span data-ttu-id="4efdd-126">Si después de la instalación no se puede ejecutar el comando y utiliza `bash` o `zsh`, debe borrar la memoria caché del hash de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="4efdd-126">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="4efdd-127">Ejecute</span><span class="sxs-lookup"><span data-stu-id="4efdd-127">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="4efdd-128">y compruebe si el problema se resuelve.</span><span class="sxs-lookup"><span data-stu-id="4efdd-128">and check if the problem is resolved.</span></span>

<span data-ttu-id="4efdd-129">Este problema también puede ocurrir si no se reinició el shell después de la instalación.</span><span class="sxs-lookup"><span data-stu-id="4efdd-129">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="4efdd-130">Asegúrese de que la ubicación del comando `az` esté en `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="4efdd-130">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="4efdd-131">La ubicación del comando `az` es</span><span class="sxs-lookup"><span data-stu-id="4efdd-131">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="4efdd-132">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="4efdd-132">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="4efdd-133">Para desinstalar la CLI, puede eliminar los archivos directamente de la ubicación elegida en el momento de la instalación.</span><span class="sxs-lookup"><span data-stu-id="4efdd-133">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="4efdd-134">La ubicación de instalación predeterminada es `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="4efdd-134">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="4efdd-135">Elimine los archivos de la CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="4efdd-135">Remove the installed CLI files.</span></span>
  
  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. <span data-ttu-id="4efdd-136">Modifique el archivo `$HOME/.bash_profile` para eliminar la línea siguiente:</span><span class="sxs-lookup"><span data-stu-id="4efdd-136">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>
  
  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="4efdd-137">Si usa `bash` o `zsh`, vuelva a cargar la memoria caché de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="4efdd-137">If using `bash` or `zsh`, reload your shell's command cache.</span></span>
  
  ```bash
  hash -r
  ```
