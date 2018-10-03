---
title: Instalación manual de la CLI de Azure para Linux
description: Cómo instalar manualmente la CLI de Azure en Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 221e8904fdb938b15b28cb369085dcacb08e4091
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177953"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="0eb58-103">Instalación manual de la CLI de Azure en Linux</span><span class="sxs-lookup"><span data-stu-id="0eb58-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="0eb58-104">Si no hay ningún paquete de la CLI de Azure para su distribución, ejecute un script para instalar la CLI manualmente.</span><span class="sxs-lookup"><span data-stu-id="0eb58-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

> [!NOTE]
> <span data-ttu-id="0eb58-105">Se recomienda utilizar un administrador de paquetes para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="0eb58-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="0eb58-106">Con un administrador de paquetes se asegura de que siempre tendrá las últimas actualizaciones y garantiza la estabilidad de los componentes de la CLI.</span><span class="sxs-lookup"><span data-stu-id="0eb58-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="0eb58-107">Compruebe si existe un paquete para su distribución antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="0eb58-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eb58-108">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="0eb58-108">Prerequisites</span></span>

<span data-ttu-id="0eb58-109">La CLI requiere el software siguiente:</span><span class="sxs-lookup"><span data-stu-id="0eb58-109">The CLI requires the following software:</span></span>

* [<span data-ttu-id="0eb58-110">Python 2.7 o Python 3.x</span><span class="sxs-lookup"><span data-stu-id="0eb58-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="0eb58-111">libffi</span><span class="sxs-lookup"><span data-stu-id="0eb58-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="0eb58-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="0eb58-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="0eb58-113">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="0eb58-113">Install or update</span></span>

<span data-ttu-id="0eb58-114">Para instalar y actualizar la CLI es necesario volver a ejecutar el script de instalación.</span><span class="sxs-lookup"><span data-stu-id="0eb58-114">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="0eb58-115">Ejecute `curl` para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="0eb58-115">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="0eb58-116">El script también se puede descargar y ejecutar localmente.</span><span class="sxs-lookup"><span data-stu-id="0eb58-116">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="0eb58-117">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="0eb58-117">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="0eb58-118">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="0eb58-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="0eb58-119">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="0eb58-119">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="0eb58-120">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0eb58-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0eb58-121">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="0eb58-121">Troubleshooting</span></span>

<span data-ttu-id="0eb58-122">Estos son algunos problemas comunes que se han observado durante la instalación manual.</span><span class="sxs-lookup"><span data-stu-id="0eb58-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="0eb58-123">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="0eb58-123">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="0eb58-124">Error de curl "Object Moved" (objeto movido)</span><span class="sxs-lookup"><span data-stu-id="0eb58-124">curl "Object Moved" error</span></span>

<span data-ttu-id="0eb58-125">Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="0eb58-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="0eb58-126">Comando `az` no encontrado</span><span class="sxs-lookup"><span data-stu-id="0eb58-126">`az` command not found</span></span>

<span data-ttu-id="0eb58-127">Si después de la instalación no se puede ejecutar el comando y utiliza `bash` o `zsh`, debe borrar la memoria caché del hash de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="0eb58-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="0eb58-128">Ejecute</span><span class="sxs-lookup"><span data-stu-id="0eb58-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="0eb58-129">y compruebe si el problema se resuelve.</span><span class="sxs-lookup"><span data-stu-id="0eb58-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="0eb58-130">Este problema también puede ocurrir si no reinició el shell después de la instalación.</span><span class="sxs-lookup"><span data-stu-id="0eb58-130">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="0eb58-131">Asegúrese de que la ubicación del comando `az` esté en `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="0eb58-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="0eb58-132">La ubicación del comando `az` es</span><span class="sxs-lookup"><span data-stu-id="0eb58-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="0eb58-133">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="0eb58-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="0eb58-134">Para desinstalar la CLI, puede eliminar los archivos directamente de la ubicación elegida en el momento de la instalación.</span><span class="sxs-lookup"><span data-stu-id="0eb58-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="0eb58-135">La ubicación de instalación predeterminada es `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="0eb58-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="0eb58-136">Elimine los archivos de la CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="0eb58-136">Remove the installed CLI files.</span></span>

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```

2. <span data-ttu-id="0eb58-137">Modifique el archivo `$HOME/.bash_profile` para eliminar la línea siguiente:</span><span class="sxs-lookup"><span data-stu-id="0eb58-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="0eb58-138">Si usa `bash` o `zsh`, vuelva a cargar la memoria caché de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="0eb58-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

  ```bash
  hash -r
  ```

## <a name="next-steps"></a><span data-ttu-id="0eb58-139">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="0eb58-139">Next Steps</span></span>

<span data-ttu-id="0eb58-140">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="0eb58-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0eb58-141">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="0eb58-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
