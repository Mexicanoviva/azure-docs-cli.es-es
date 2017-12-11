---
title: "Instalación de la CLI de Azure 2.0"
description: "Consulte los documentos para la instalación de la CLI de Azure 2.0"
keywords: CLI de Azure, instalar la CLI de Azure, CLI de Azure para Python, referencia de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 36429bb23f392ff6210a9c99885df83f53768386
ms.sourcegitcommit: 5fc7d8ccf2304c5a12fb99a80f0b00a0ad2c34e9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/01/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="1f008-104">Instalación de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="1f008-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="1f008-105">Instale hoy mismo la nueva versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="1f008-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="1f008-106">La hemos mejorado y actualizado para facilitar la administración nativa de los recursos de Azure desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="1f008-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="1f008-107">Se puede usar en macOS, Linux y Windows.</span><span class="sxs-lookup"><span data-stu-id="1f008-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="1f008-108">Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1f008-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="1f008-109">Si está usando el modelo de Azure Service Management (ASM), [instale la CLI de Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="1f008-109">If you are using the Azure Service Management (ASM) model, [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="1f008-110"><a name="macOS"/>Instalación en macOS</span><span class="sxs-lookup"><span data-stu-id="1f008-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="1f008-111">En macOS, es posible instalar con [Homebrew](https://brew.sh/) o de forma manual.</span><span class="sxs-lookup"><span data-stu-id="1f008-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="1f008-112">Instalación con Homebrew</span><span class="sxs-lookup"><span data-stu-id="1f008-112">Install with Homebrew</span></span>

1. <span data-ttu-id="1f008-113">Si no lo tiene todavía, instale Homebrew siguiendo las [instrucciones de instalación correspondientes](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="1f008-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="1f008-114">Si ha instalado manualmente la CLI, siga las instrucciones para la [desinstalación manual](#UninstallManually).</span><span class="sxs-lookup"><span data-stu-id="1f008-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="1f008-115">Actualice los repositorios locales de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="1f008-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="1f008-116">Instale el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="1f008-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="1f008-117">Si instaló anteriormente la CLI de Azure 1.0 con Homebrew, en lugar de instalar el paquete puede obtener la CLI 2.0 durante el proceso de actualización normal de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="1f008-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="1f008-118">Instalación manual</span><span class="sxs-lookup"><span data-stu-id="1f008-118">Install manually</span></span>

1. <span data-ttu-id="1f008-119">Instalación de la CLI de Azure 2.0 con `curl`.</span><span class="sxs-lookup"><span data-stu-id="1f008-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="1f008-120">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="1f008-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="1f008-121">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="1f008-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="1f008-122">Instalación en Windows</span><span class="sxs-lookup"><span data-stu-id="1f008-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="1f008-123">Instalación con MSI para la línea de comandos de Windows</span><span class="sxs-lookup"><span data-stu-id="1f008-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="1f008-124">Para instalar la CLI en Windows y usarla en la línea de comandos de Windows, descargue y ejecute el [instalador de la CLI de Azure (MSI)](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="1f008-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="1f008-125">Instalación con apt-get para Bash en Ubuntu en Windows</span><span class="sxs-lookup"><span data-stu-id="1f008-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="1f008-126">Si no dispone de Bash en Windows, [instálelo](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="1f008-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="1f008-127">Abra el shell de Bash.</span><span class="sxs-lookup"><span data-stu-id="1f008-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="1f008-128">Modifique la lista de orígenes.</span><span class="sxs-lookup"><span data-stu-id="1f008-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="1f008-129">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="1f008-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="1f008-130">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="1f008-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-apt-package-manager"></a><span data-ttu-id="1f008-131">Instalación con el administrador de paquetes apt</span><span class="sxs-lookup"><span data-stu-id="1f008-131">Install with apt package manager</span></span> 

<span data-ttu-id="1f008-132">Para distribuciones que usan el administrador de paquetes `apt` como Ubuntu o Debian, puede instalar la CLI de Azure 2.0 a través de `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="1f008-132">For distributions using the `apt` package manager such as Ubuntu or Debian, you can install Azure CLI 2.0 via `apt-get`.</span></span>

> [!NOTE]
> <span data-ttu-id="1f008-133">Debe tener Python 2.7.x o Python 3.x para poder usar la CLI.</span><span class="sxs-lookup"><span data-stu-id="1f008-133">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="1f008-134">Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="1f008-134">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

1. <span data-ttu-id="1f008-135">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="1f008-135">Modify your sources list:</span></span>
 
   - <span data-ttu-id="1f008-136">Sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="1f008-136">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="1f008-137">Sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="1f008-137">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="1f008-138">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="1f008-138">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="1f008-139">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="1f008-139">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-yum-package-manager"></a><span data-ttu-id="1f008-140">Instalación con el administrador de paquetes yum</span><span class="sxs-lookup"><span data-stu-id="1f008-140">Install with yum package manager</span></span>

<span data-ttu-id="1f008-141">Para las distribuciones que utilizan el administrador de paquetes `yum` como Red Hat Enterprise Linux (RHEL), Fedora o CentOS, puede instalar la CLI de Azure 2.0 a través de `yum`.</span><span class="sxs-lookup"><span data-stu-id="1f008-141">For distributions which use the `yum` package manager such as Red Hat Enterprise Linux (RHEL), Fedora, or CentOS, you can install Azure CLI 2.0 via `yum`.</span></span>

> [!NOTE]
> <span data-ttu-id="1f008-142">Debe tener Python 2.7.x o Python 3.x para poder usar la CLI.</span><span class="sxs-lookup"><span data-stu-id="1f008-142">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="1f008-143">Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="1f008-143">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

1. <span data-ttu-id="1f008-144">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="1f008-144">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="1f008-145">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="1f008-145">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="1f008-146">Actualice el índice del paquete `yum` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="1f008-146">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="1f008-147">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="1f008-147">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-zypper-package-manager"></a><span data-ttu-id="1f008-148">Instalación con el administrador de paquetes zypper</span><span class="sxs-lookup"><span data-stu-id="1f008-148">Install with zypper package manager</span></span>

<span data-ttu-id="1f008-149">Para distribuciones que usan el administrador de paquetes `zypper` como OpenSUSE o SLE, puede instalar la CLI de Azure 2.0 a través de `zypper`.</span><span class="sxs-lookup"><span data-stu-id="1f008-149">For distributions which use the `zypper` package manager such as OpenSUSE or SLE, you can install Azure CLI 2.0 via `zypper`.</span></span>

> [!NOTE]
> <span data-ttu-id="1f008-150">Debe tener Python 2.7.x o Python 3.x para poder usar la CLI.</span><span class="sxs-lookup"><span data-stu-id="1f008-150">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="1f008-151">Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="1f008-151">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

1. <span data-ttu-id="1f008-152">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="1f008-152">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="1f008-153">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="1f008-153">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="1f008-154">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="1f008-154">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="1f008-155">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="1f008-155">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="1f008-156">Instalación con Docker</span><span class="sxs-lookup"><span data-stu-id="1f008-156">Install with Docker</span></span>

<span data-ttu-id="1f008-157">Mantenemos una imagen de Docker preconfigurada con la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="1f008-157">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="1f008-158">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="1f008-158">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="1f008-159">Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="1f008-159">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="1f008-160">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="1f008-160">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="1f008-161">Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="1f008-161">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><span data-ttu-id="1f008-162"><a name="Linux"/>Instalación en Linux sin un administrador de paquetes</span><span class="sxs-lookup"><span data-stu-id="1f008-162"><a name="Linux"/>Install on Linux without a package manager</span></span>

<span data-ttu-id="1f008-163">Se recomienda instalar la CLI con un administrador de paquetes si es posible.</span><span class="sxs-lookup"><span data-stu-id="1f008-163">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="1f008-164">Si no desea agregar repositorios de Microsoft, o si está trabajando con una distribución para la que no se ha proporcionado ningún paquete, puede instalar manualmente la CLI.</span><span class="sxs-lookup"><span data-stu-id="1f008-164">If you do not want to add Microsoft's repositories, or are working with a distribution which does not have a provided package, you can manually install the CLI.</span></span>

1. <span data-ttu-id="1f008-165">Instale los requisitos previos en función de la distribución de Linux.</span><span class="sxs-lookup"><span data-stu-id="1f008-165">Install the prerequisites based on your Linux distribution.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

<span data-ttu-id="1f008-166">Si la distribución no está indicada anteriormente, debe instalar [Python 2.7 o posterior](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) y [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="1f008-166">If your distribution is not listed above, you will need to install [Python 2.7 or later](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="1f008-167">Instalación de la CLI con `curl`.</span><span class="sxs-lookup"><span data-stu-id="1f008-167">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="1f008-168">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="1f008-168">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="1f008-169">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="1f008-169">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1f008-170">Solución de problemas</span><span class="sxs-lookup"><span data-stu-id="1f008-170">Troubleshooting</span></span>

<span data-ttu-id="1f008-171">Si encuentra algún problema durante la instalación de la CLI, consulte esta sección para ver si su caso particular ya está descrito.</span><span class="sxs-lookup"><span data-stu-id="1f008-171">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="1f008-172">Si su problema no está aquí, [notifique un problema de Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1f008-172">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="1f008-173">Error de curl "Object Moved" (objeto movido)</span><span class="sxs-lookup"><span data-stu-id="1f008-173">curl "Object Moved" error</span></span>

<span data-ttu-id="1f008-174">Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="1f008-174">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="1f008-175">Comando `az` no encontrado</span><span class="sxs-lookup"><span data-stu-id="1f008-175">`az` command not found</span></span>

<span data-ttu-id="1f008-176">Debe borrar la caché de hash de comandos del shell.</span><span class="sxs-lookup"><span data-stu-id="1f008-176">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="1f008-177">Ejecute</span><span class="sxs-lookup"><span data-stu-id="1f008-177">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="1f008-178">y compruebe si el problema se resuelve.</span><span class="sxs-lookup"><span data-stu-id="1f008-178">and see if the problem is resolved.</span></span> <span data-ttu-id="1f008-179">El comando también podría no estar en su variable `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="1f008-179">The command may also not be in your `$PATH`.</span></span> <span data-ttu-id="1f008-180">Asegúrese de que `<install path>/bin` aparece en la variable `$PATH` y reinicie el shell si es necesario.</span><span class="sxs-lookup"><span data-stu-id="1f008-180">Make sure that `<install path>/bin` appears in your `$PATH`, and restart your shell if necessary.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="1f008-181">Desinstalación de las versiones 1.x de la CLI</span><span class="sxs-lookup"><span data-stu-id="1f008-181">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="1f008-182">Si tiene una versión de la CLI 1.x anterior en el sistema, puede desinstalarla según el tipo de instalación que se usó.</span><span class="sxs-lookup"><span data-stu-id="1f008-182">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="1f008-183">Desinstalación con npm</span><span class="sxs-lookup"><span data-stu-id="1f008-183">Uninstall with npm</span></span>

<span data-ttu-id="1f008-184">Quite la CLI anterior con `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="1f008-184">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="1f008-185">Desinstalación con código distribuible</span><span class="sxs-lookup"><span data-stu-id="1f008-185">Uninstall with distributable</span></span>

<span data-ttu-id="1f008-186">Si realizó la instalación mediante [el instalador de la CLI de Azure (MSI)](http://aka.ms/webpi-azure-cli) o un [paquete de macOS](http://aka.ms/mac-azure-cli), use la misma herramienta para quitar la instalación.</span><span class="sxs-lookup"><span data-stu-id="1f008-186">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="1f008-187">Desinstalación con Docker</span><span class="sxs-lookup"><span data-stu-id="1f008-187">Uninstall with Docker</span></span>

<span data-ttu-id="1f008-188">Si ha instalado una imagen de Docker para usar la versión anterior de la CLI, quite dicha imagen y los contenedores asociados.</span><span class="sxs-lookup"><span data-stu-id="1f008-188">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="1f008-189">Después, puede volver a crear los contenedores después de instalar la nueva imagen de Docker, tal y como se describe en las instrucciones de instalación.</span><span class="sxs-lookup"><span data-stu-id="1f008-189">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="1f008-190">Actualización de la CLI</span><span class="sxs-lookup"><span data-stu-id="1f008-190">Update the CLI</span></span>

<span data-ttu-id="1f008-191">Para actualizar la CLI de Azure, use el mismo método que usó para su instalación.</span><span class="sxs-lookup"><span data-stu-id="1f008-191">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="1f008-192">Actualización con Homebrew</span><span class="sxs-lookup"><span data-stu-id="1f008-192">Update with Homebrew</span></span>

1. <span data-ttu-id="1f008-193">Si anteriormente realizó la instalación de forma manual, siga las instrucciones de [instalación con Homebrew](#macOS).</span><span class="sxs-lookup"><span data-stu-id="1f008-193">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="1f008-194">Actualice la información del repositorio local de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="1f008-194">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="1f008-195">Actualice los paquetes instalados.</span><span class="sxs-lookup"><span data-stu-id="1f008-195">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="1f008-196">Actualización con MSI</span><span class="sxs-lookup"><span data-stu-id="1f008-196">Update with MSI</span></span>

<span data-ttu-id="1f008-197">Ejecute de nuevo el [instalador de la CLI de Azure (MSI)](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="1f008-197">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt"></a><span data-ttu-id="1f008-198">Actualización con apt</span><span class="sxs-lookup"><span data-stu-id="1f008-198">Update with apt</span></span>

<span data-ttu-id="1f008-199">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="1f008-199">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="1f008-200">Esto actualizará todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="1f008-200">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="1f008-201">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="1f008-201">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-yum"></a><span data-ttu-id="1f008-202">Actualización con yum</span><span class="sxs-lookup"><span data-stu-id="1f008-202">Update with yum</span></span>

<span data-ttu-id="1f008-203">Actualice la CLI de Azure con el comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="1f008-203">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

### <a name="update-with-zypper"></a><span data-ttu-id="1f008-204">Actualización con zypper</span><span class="sxs-lookup"><span data-stu-id="1f008-204">Update with zypper</span></span>

<span data-ttu-id="1f008-205">Puede actualizar el paquete con el comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="1f008-205">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

### <a name="update-with-docker"></a><span data-ttu-id="1f008-206">Actualización con Docker</span><span class="sxs-lookup"><span data-stu-id="1f008-206">Update with Docker</span></span>

1. <span data-ttu-id="1f008-207">Actualización de la imagen local con `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="1f008-207">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="1f008-208">Obtenga los contenedores que está usando con la imagen de la CLI.</span><span class="sxs-lookup"><span data-stu-id="1f008-208">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="1f008-209">Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.</span><span class="sxs-lookup"><span data-stu-id="1f008-209">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="1f008-210">Detenga y vuelva a crear los contenedores.</span><span class="sxs-lookup"><span data-stu-id="1f008-210">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="1f008-211">Actualización manual</span><span class="sxs-lookup"><span data-stu-id="1f008-211">Update manually</span></span>

<span data-ttu-id="1f008-212">Para actualizar, siga las instrucciones de instalación manual en [macOS](#macOS) o [Linux](#Linux).</span><span class="sxs-lookup"><span data-stu-id="1f008-212">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="1f008-213">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="1f008-213">Uninstall</span></span>

<span data-ttu-id="1f008-214">Si decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="1f008-214">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="1f008-215">Debe desinstalar con el mismo método que utilizó para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="1f008-215">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="1f008-216">Desinstalación con Homebrew</span><span class="sxs-lookup"><span data-stu-id="1f008-216">Uninstall with Homebrew</span></span>

<span data-ttu-id="1f008-217">Desinstale el paquete `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="1f008-217">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="1f008-218">Desinstalación con MSI</span><span class="sxs-lookup"><span data-stu-id="1f008-218">Uninstall with MSI</span></span>

<span data-ttu-id="1f008-219">Ejecute [MSI](https://aka.ms/InstallAzureCliWindows) de nuevo y elija la opción de desinstalación.</span><span class="sxs-lookup"><span data-stu-id="1f008-219">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt"></a><span data-ttu-id="1f008-220">Desinstalación con apt</span><span class="sxs-lookup"><span data-stu-id="1f008-220">Uninstall with apt</span></span>

<span data-ttu-id="1f008-221">Desinstalación mediante `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="1f008-221">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-yum"></a><span data-ttu-id="1f008-222">Desinstalación con yum</span><span class="sxs-lookup"><span data-stu-id="1f008-222">Uninstall with yum</span></span>

1. <span data-ttu-id="1f008-223">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="1f008-223">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="1f008-224">Si no piensa volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="1f008-224">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="1f008-225">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1f008-225">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-zypper"></a><span data-ttu-id="1f008-226">Desinstalación con zypper</span><span class="sxs-lookup"><span data-stu-id="1f008-226">Uninstall with zypper</span></span>

1. <span data-ttu-id="1f008-227">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="1f008-227">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="1f008-228">Si no piensa volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="1f008-228">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="1f008-229">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1f008-229">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="1f008-230">Desinstalación con Docker</span><span class="sxs-lookup"><span data-stu-id="1f008-230">Uninstall with Docker</span></span>

<span data-ttu-id="1f008-231">Si ha instalado una imagen de Docker, debe quitar los contenedores que la ejecutan y, a continuación, eliminar la imagen local.</span><span class="sxs-lookup"><span data-stu-id="1f008-231">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="1f008-232">Obtenga los contenedores que están ejecutando la imagen azure-cli.</span><span class="sxs-lookup"><span data-stu-id="1f008-232">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="1f008-233">Elimine los contenedores con la imagen de la CLI.</span><span class="sxs-lookup"><span data-stu-id="1f008-233">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="1f008-234">Quite la imagen de la CLI instalada localmente.</span><span class="sxs-lookup"><span data-stu-id="1f008-234">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="1f008-235">Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.</span><span class="sxs-lookup"><span data-stu-id="1f008-235">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="1f008-236"><a name="UninstallManually"/>Desinstalación manual</span><span class="sxs-lookup"><span data-stu-id="1f008-236"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="1f008-237">Si usó el script de https://aka.ms/InstallAzureCli para instalar la CLI, siga estos pasos para desinstalarla.</span><span class="sxs-lookup"><span data-stu-id="1f008-237">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="1f008-238">Quite los archivos instalados.</span><span class="sxs-lookup"><span data-stu-id="1f008-238">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="1f008-239">Elimine la línea `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="1f008-239">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

3. <span data-ttu-id="1f008-240">Si el shell utiliza una caché de comandos, vuelva a cargarlo.</span><span class="sxs-lookup"><span data-stu-id="1f008-240">If your shell uses a command cache, reload it.</span></span>

   ```bash
   hash -r
   ```

> [!Note]
> <span data-ttu-id="1f008-241">La ubicación de instalación predeterminada es `/Users/<username>` para macOS y `/home/<username>` para Linux.</span><span class="sxs-lookup"><span data-stu-id="1f008-241">The default install location is `/Users/<username>` for macOS and `/home/<username>` for Linux.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="1f008-242">Notificación de problemas y comentarios sobre la CLI</span><span class="sxs-lookup"><span data-stu-id="1f008-242">Report CLI issues and feedback</span></span>

<span data-ttu-id="1f008-243">Si aparecen errores al usar la herramienta, envíe un problema en la sección [Issues](https://github.com/Azure/azure-cli/issues) (Problemas) del repositorio de GitHub.</span><span class="sxs-lookup"><span data-stu-id="1f008-243">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="1f008-244">Para proporcionar comentarios desde la línea de comandos, use el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="1f008-244">To provide feedback from the command line, use the `az feedback` command.</span></span>
