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
ms.devlang: azurecli
ms.openlocfilehash: caca30ec186f302e47f2978b9bfe616d4b2a5c02
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543634"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="590f9-103">Instalación manual de la CLI de Azure en Linux</span><span class="sxs-lookup"><span data-stu-id="590f9-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="590f9-104">Si no hay ningún paquete de la CLI de Azure para su distribución, ejecute un script para instalar la CLI manualmente.</span><span class="sxs-lookup"><span data-stu-id="590f9-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="590f9-105">Se recomienda utilizar un administrador de paquetes para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="590f9-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="590f9-106">Con un administrador de paquetes se asegura de que siempre tendrá las últimas actualizaciones y garantiza la estabilidad de los componentes de la CLI.</span><span class="sxs-lookup"><span data-stu-id="590f9-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="590f9-107">Compruebe si existe un paquete para su distribución antes de instalar manualmente.</span><span class="sxs-lookup"><span data-stu-id="590f9-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="590f9-108">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="590f9-108">Prerequisites</span></span>

<span data-ttu-id="590f9-109">La CLI requiere el software siguiente:</span><span class="sxs-lookup"><span data-stu-id="590f9-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="590f9-110">[Python 3.6.x o 3.7.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="590f9-110">[Python 3.6.x or 3.7.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="590f9-111">libffi</span><span class="sxs-lookup"><span data-stu-id="590f9-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="590f9-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="590f9-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="590f9-113">La CLI también es compatible con Python 2.7. x, que terminará su ciclo de vida el 1 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="590f9-113">The CLI is also compatible with Python 2.7.x, which is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="590f9-114">Una versión futura de la CLI de Azure eliminará la compatibilidad con Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="590f9-114">A future version of Azure CLI will drop support for Python 2.7.</span></span> <span data-ttu-id="590f9-115">Por este motivo, se recomienda instalar Python 3 para ejecutar la CLI.</span><span class="sxs-lookup"><span data-stu-id="590f9-115">For this reason we recommend that you install Python 3 to run the CLI.</span></span> 

## <a name="install-or-update"></a><span data-ttu-id="590f9-116">Instalación o actualización</span><span class="sxs-lookup"><span data-stu-id="590f9-116">Install or update</span></span>

<span data-ttu-id="590f9-117">Para instalar y actualizar la CLI es necesario volver a ejecutar el script de instalación.</span><span class="sxs-lookup"><span data-stu-id="590f9-117">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="590f9-118">Ejecute `curl` para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="590f9-118">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="590f9-119">El script también se puede descargar y ejecutar localmente.</span><span class="sxs-lookup"><span data-stu-id="590f9-119">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="590f9-120">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="590f9-120">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="590f9-121">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="590f9-121">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="590f9-122">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="590f9-122">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="590f9-123">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="590f9-123">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="590f9-124">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="590f9-124">Troubleshooting</span></span>

<span data-ttu-id="590f9-125">Estos son algunos problemas comunes que se han observado durante la instalación manual.</span><span class="sxs-lookup"><span data-stu-id="590f9-125">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="590f9-126">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="590f9-126">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="590f9-127">Error de curl "Object Moved" (objeto movido)</span><span class="sxs-lookup"><span data-stu-id="590f9-127">curl "Object Moved" error</span></span>

<span data-ttu-id="590f9-128">Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="590f9-128">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="590f9-129">Comando `az` no encontrado</span><span class="sxs-lookup"><span data-stu-id="590f9-129">`az` command not found</span></span>

<span data-ttu-id="590f9-130">Si después de la instalación no se puede ejecutar el comando y utiliza `bash` o `zsh`, debe borrar la memoria caché del hash de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="590f9-130">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="590f9-131">Ejecute</span><span class="sxs-lookup"><span data-stu-id="590f9-131">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="590f9-132">y compruebe si el problema se resuelve.</span><span class="sxs-lookup"><span data-stu-id="590f9-132">and check if the problem is resolved.</span></span>

<span data-ttu-id="590f9-133">Este problema también puede ocurrir si no reinició el shell después de la instalación.</span><span class="sxs-lookup"><span data-stu-id="590f9-133">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="590f9-134">Asegúrese de que la ubicación del comando `az` esté en `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="590f9-134">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="590f9-135">La ubicación del comando `az` es</span><span class="sxs-lookup"><span data-stu-id="590f9-135">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="590f9-136">Conexión de bloques proxy</span><span class="sxs-lookup"><span data-stu-id="590f9-136">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="590f9-137">Para obtener los scripts de instalación, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:</span><span class="sxs-lookup"><span data-stu-id="590f9-137">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="590f9-138">Puntos de conexión usados por el administrador de paquetes de su distribución (si existe) para los paquetes principales.</span><span class="sxs-lookup"><span data-stu-id="590f9-138">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="590f9-139">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="590f9-139">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="590f9-140">Para desinstalar la CLI, puede eliminar los archivos directamente de la ubicación elegida en el momento de la instalación.</span><span class="sxs-lookup"><span data-stu-id="590f9-140">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="590f9-141">La ubicación de instalación predeterminada es `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="590f9-141">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="590f9-142">Elimine los archivos de la CLI instalados.</span><span class="sxs-lookup"><span data-stu-id="590f9-142">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="590f9-143">Modifique el archivo `$HOME/.bash_profile` para eliminar la línea siguiente:</span><span class="sxs-lookup"><span data-stu-id="590f9-143">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="590f9-144">Si usa `bash` o `zsh`, vuelva a cargar la memoria caché de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="590f9-144">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="590f9-145">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="590f9-145">Next Steps</span></span>

<span data-ttu-id="590f9-146">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="590f9-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="590f9-147">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="590f9-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
