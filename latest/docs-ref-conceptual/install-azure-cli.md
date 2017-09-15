---
title: "Instalación de la CLI de Azure 2.0"
description: "Consulte los documentos para la instalación de la CLI de Azure 2.0"
keywords: CLI de Azure, instalar la CLI de Azure, CLI de Azure para Python, referencia de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: a61f47076854d0ff0a7056f82240794b7533fe3e
ms.sourcegitcommit: 3db5fb207db551a0d3fe0a88fe09e8f5e2ec184d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="97d27-104">Instalación de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="97d27-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="97d27-105">Instale hoy mismo la nueva versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="97d27-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="97d27-106">La hemos mejorado y actualizado para facilitar la administración nativa de los recursos de Azure desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="97d27-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="97d27-107">Se puede usar en macOS, Linux y Windows.</span><span class="sxs-lookup"><span data-stu-id="97d27-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="97d27-108">Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="97d27-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="97d27-109">Si necesita la versión anterior de la CLI de Azure, vea aquí cómo [instalar la CLI de Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="97d27-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="97d27-110"><a name="macOS"/>Instalación en macOS</span><span class="sxs-lookup"><span data-stu-id="97d27-110"><a name="macOS"/>Install on macOS</span></span>

1. <span data-ttu-id="97d27-111">Instalación de la CLI de Azure 2.0 con `curl`.</span><span class="sxs-lookup"><span data-stu-id="97d27-111">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="97d27-112">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="97d27-112">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="97d27-113">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="97d27-113">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="97d27-114">Instalación en Windows</span><span class="sxs-lookup"><span data-stu-id="97d27-114">Install on Windows</span></span>

<span data-ttu-id="97d27-115">Puede instalar la CLI de Azure 2.0 con el archivo MSI y utilizarla en la línea de comandos de Windows, o puede instalar la CLI con `apt-get` en Bash en Ubuntu en Windows.</span><span class="sxs-lookup"><span data-stu-id="97d27-115">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="97d27-116">Instalación con MSI para la línea de comandos de Windows</span><span class="sxs-lookup"><span data-stu-id="97d27-116">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="97d27-117">Para instalar la CLI en Windows y usarla en la línea de comandos de Windows, descargue y ejecute el archivo [MSI](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="97d27-117">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="97d27-118">Instalación con apt-get para Bash en Ubuntu en Windows</span><span class="sxs-lookup"><span data-stu-id="97d27-118">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="97d27-119">Si no dispone de Bash en Windows, [instálelo](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="97d27-119">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="97d27-120">Abra el shell de Bash.</span><span class="sxs-lookup"><span data-stu-id="97d27-120">Open the Bash shell.</span></span>

3. <span data-ttu-id="97d27-121">Modifique la lista de orígenes.</span><span class="sxs-lookup"><span data-stu-id="97d27-121">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="97d27-122">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="97d27-122">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="97d27-123">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="97d27-123">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="97d27-124">Instalación en Debian/Ubuntu con apt-get</span><span class="sxs-lookup"><span data-stu-id="97d27-124">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="97d27-125">En los sistemas con Debian y Ubuntu, la CLI de Azure 2.0 se puede instalar a través de `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="97d27-125">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="97d27-126">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="97d27-126">Modify your sources list:</span></span>
 
   - <span data-ttu-id="97d27-127">Sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="97d27-127">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="97d27-128">Sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="97d27-128">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="97d27-129">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="97d27-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="97d27-130">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="97d27-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="97d27-131">Instalación en RHEL, Fedora y CentOS con yum</span><span class="sxs-lookup"><span data-stu-id="97d27-131">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="97d27-132">Para las distribuciones basadas en RedHat que contengan el administrador de paquetes de `yum`, puede instalar la CLI de Azure 2.0 mediante `yum`.</span><span class="sxs-lookup"><span data-stu-id="97d27-132">For any distribution which is based off of RedHat and contains the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

1. <span data-ttu-id="97d27-133">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="97d27-133">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="97d27-134">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="97d27-134">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="97d27-135">Actualice el índice del paquete `yum` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="97d27-135">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="97d27-136">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="97d27-136">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="97d27-137">Instalación en openSUSE y SLE con zypper</span><span class="sxs-lookup"><span data-stu-id="97d27-137">Install on openSUSE and SLE with zypper</span></span>

1. <span data-ttu-id="97d27-138">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="97d27-138">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="97d27-139">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="97d27-139">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="97d27-140">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="97d27-140">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="97d27-141">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="97d27-141">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="97d27-142">Instalación con Docker</span><span class="sxs-lookup"><span data-stu-id="97d27-142">Install with Docker</span></span>

<span data-ttu-id="97d27-143">Mantenemos una imagen de Docker preconfigurada con la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="97d27-143">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="97d27-144">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="97d27-144">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="97d27-145">Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="97d27-145">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="97d27-146">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="97d27-146">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="97d27-147">Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="97d27-147">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="97d27-148"><a name="Linux"/>Instalación en Linux sin apt-get</span><span class="sxs-lookup"><span data-stu-id="97d27-148"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="97d27-149">Se recomienda instalar la CLI con un administrador de paquetes si es posible.</span><span class="sxs-lookup"><span data-stu-id="97d27-149">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="97d27-150">En el caso de las distribuciones que no tienen un administrador de paquetes, puede instalarla manualmente.</span><span class="sxs-lookup"><span data-stu-id="97d27-150">For distributions which do not have a package provided for them, you can manually install.</span></span>

1. <span data-ttu-id="97d27-151">Instale los requisitos previos en función de la distribución de Linux.</span><span class="sxs-lookup"><span data-stu-id="97d27-151">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="97d27-152">Si la distribución no está indicada anteriormente, debe instalar [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) y [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="97d27-152">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="97d27-153">Instalación de la CLI con `curl`.</span><span class="sxs-lookup"><span data-stu-id="97d27-153">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="97d27-154">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.</span><span class="sxs-lookup"><span data-stu-id="97d27-154">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="97d27-155">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="97d27-155">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="97d27-156">Solución de problemas</span><span class="sxs-lookup"><span data-stu-id="97d27-156">Troubleshooting</span></span>

<span data-ttu-id="97d27-157">Si encuentra algún problema durante la instalación de la CLI, consulte esta sección para ver si su caso particular ya está descrito.</span><span class="sxs-lookup"><span data-stu-id="97d27-157">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="97d27-158">Si su problema no está aquí, [notifique un problema de Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="97d27-158">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="97d27-159">Error de curl "Object Moved" (objeto movido)</span><span class="sxs-lookup"><span data-stu-id="97d27-159">curl "Object Moved" error</span></span>

<span data-ttu-id="97d27-160">Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="97d27-160">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a><span data-ttu-id="97d27-161">Homebrew en macOS instala versiones anteriores</span><span class="sxs-lookup"><span data-stu-id="97d27-161">Homebrew on macOS installing older version</span></span>

<span data-ttu-id="97d27-162">La fórmula `azure-cli` de Homebrew disponible para macOS no está actualizada e instalará una versión 1.x de la CLI.</span><span class="sxs-lookup"><span data-stu-id="97d27-162">The Homebrew `azure-cli` formula available for macOS is currently out of date, and will install a 1.x version of the CLI.</span></span> <span data-ttu-id="97d27-163">Para ver cuándo se actualiza, consulte `brew info azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="97d27-163">You can see when it is updated by checking `brew info azure-cli`.</span></span>

<span data-ttu-id="97d27-164">Hasta entonces, [desinstale la versión anterior](#uninstall_brew) y siga las [instrucciones de instalación de macOS](#macOS).</span><span class="sxs-lookup"><span data-stu-id="97d27-164">Until then, [uninstall the older version](#uninstall_brew) and follow the [macOS install instructions](#macOS).</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="97d27-165">Desinstalación de las versiones 1.x de la CLI</span><span class="sxs-lookup"><span data-stu-id="97d27-165">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="97d27-166">Si tiene una versión de la CLI 1.x anterior en el sistema, puede desinstalarla según el tipo de instalación que se usó.</span><span class="sxs-lookup"><span data-stu-id="97d27-166">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="97d27-167">Desinstalación con npm</span><span class="sxs-lookup"><span data-stu-id="97d27-167">Uninstall with npm</span></span>

<span data-ttu-id="97d27-168">Quite la CLI anterior con `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="97d27-168">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><span data-ttu-id="97d27-169"><a name="uninstall_brew"/>Desinstalación con Homebrew en macOS</span><span class="sxs-lookup"><span data-stu-id="97d27-169"><a name="uninstall_brew"/>Uninstall with Homebrew on macOS</span></span>

<span data-ttu-id="97d27-170">Quite la CLI anterior con `brew uninstall`.</span><span class="sxs-lookup"><span data-stu-id="97d27-170">Remove the older CLI with `brew uninstall`.</span></span>

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="97d27-171">Desinstalación con código distribuible</span><span class="sxs-lookup"><span data-stu-id="97d27-171">Uninstall with distributable</span></span>

<span data-ttu-id="97d27-172">Si instaló mediante [MSI](http://aka.ms/webpi-azure-cli) o un [paquete de macOS](http://aka.ms/mac-azure-cli), use la misma herramienta para quitar la instalación.</span><span class="sxs-lookup"><span data-stu-id="97d27-172">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="97d27-173">Desinstalación con Docker</span><span class="sxs-lookup"><span data-stu-id="97d27-173">Uninstall with Docker</span></span>

<span data-ttu-id="97d27-174">Si ha instalado una imagen de Docker para usar la versión anterior de la CLI, quite dicha imagen y los contenedores asociados.</span><span class="sxs-lookup"><span data-stu-id="97d27-174">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="97d27-175">Después, puede volver a crear los contenedores después de instalar la nueva imagen de Docker, tal y como se describe en las instrucciones de instalación.</span><span class="sxs-lookup"><span data-stu-id="97d27-175">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="97d27-176">Actualización de la CLI</span><span class="sxs-lookup"><span data-stu-id="97d27-176">Update the CLI</span></span>

<span data-ttu-id="97d27-177">Para actualizar la CLI de Azure, use el mismo método que usó para su instalación.</span><span class="sxs-lookup"><span data-stu-id="97d27-177">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-msi"></a><span data-ttu-id="97d27-178">Actualización con MSI</span><span class="sxs-lookup"><span data-stu-id="97d27-178">Update with MSI</span></span>

<span data-ttu-id="97d27-179">Ejecute de nuevo el [MSI](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="97d27-179">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="97d27-180">Actualización con apt-get</span><span class="sxs-lookup"><span data-stu-id="97d27-180">Update with apt-get</span></span>

<span data-ttu-id="97d27-181">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="97d27-181">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="97d27-182">Esto actualizará todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="97d27-182">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="97d27-183">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="97d27-183">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="97d27-184">Actualización con Docker</span><span class="sxs-lookup"><span data-stu-id="97d27-184">Update with Docker</span></span>

1. <span data-ttu-id="97d27-185">Actualización de la imagen local con `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="97d27-185">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="97d27-186">Obtenga los contenedores que está usando con la imagen de la CLI.</span><span class="sxs-lookup"><span data-stu-id="97d27-186">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="97d27-187">Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.</span><span class="sxs-lookup"><span data-stu-id="97d27-187">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="97d27-188">Detenga y vuelva a crear los contenedores.</span><span class="sxs-lookup"><span data-stu-id="97d27-188">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="97d27-189">Actualización manual</span><span class="sxs-lookup"><span data-stu-id="97d27-189">Update manually</span></span>

<span data-ttu-id="97d27-190">Para actualizar, siga las instrucciones de instalación manual en [macOS](#macOS) o [Linux](#Linux).</span><span class="sxs-lookup"><span data-stu-id="97d27-190">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="97d27-191">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="97d27-191">Uninstall</span></span>

<span data-ttu-id="97d27-192">Si decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="97d27-192">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="97d27-193">Debe desinstalar con el mismo método que utilizó para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="97d27-193">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-msi"></a><span data-ttu-id="97d27-194">Desinstalación con MSI</span><span class="sxs-lookup"><span data-stu-id="97d27-194">Uninstall with MSI</span></span>

<span data-ttu-id="97d27-195">Ejecute [MSI](https://aka.ms/InstallAzureCliWindows) de nuevo y elija la opción de desinstalación.</span><span class="sxs-lookup"><span data-stu-id="97d27-195">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="97d27-196">Desinstalación con apt-get</span><span class="sxs-lookup"><span data-stu-id="97d27-196">Uninstall with apt-get</span></span>

<span data-ttu-id="97d27-197">Desinstalación mediante `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="97d27-197">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="97d27-198">Desinstalación con Docker</span><span class="sxs-lookup"><span data-stu-id="97d27-198">Uninstall with Docker</span></span>

<span data-ttu-id="97d27-199">Si ha instalado una imagen de Docker, debe quitar los contenedores que la ejecutan y, a continuación, eliminar la imagen local.</span><span class="sxs-lookup"><span data-stu-id="97d27-199">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="97d27-200">Obtenga los contenedores que están ejecutando la imagen azure-cli.</span><span class="sxs-lookup"><span data-stu-id="97d27-200">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="97d27-201">Elimine los contenedores con la imagen de la CLI.</span><span class="sxs-lookup"><span data-stu-id="97d27-201">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="97d27-202">Quite la imagen de la CLI instalada localmente.</span><span class="sxs-lookup"><span data-stu-id="97d27-202">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="97d27-203">Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.</span><span class="sxs-lookup"><span data-stu-id="97d27-203">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="97d27-204">Desinstalación manual</span><span class="sxs-lookup"><span data-stu-id="97d27-204">Uninstall manually</span></span>

<span data-ttu-id="97d27-205">Si usó el script de https://aka.ms/InstallAzureCli para instalar la CLI, siga estos pasos para desinstalarla.</span><span class="sxs-lookup"><span data-stu-id="97d27-205">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="97d27-206">Quite los archivos instalados.</span><span class="sxs-lookup"><span data-stu-id="97d27-206">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="97d27-207">Elimine la línea `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="97d27-207">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="97d27-208">La ubicación de instalación predeterminada es `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="97d27-208">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="97d27-209">Notificación de problemas y comentarios sobre la CLI</span><span class="sxs-lookup"><span data-stu-id="97d27-209">Report CLI issues and feedback</span></span>

<span data-ttu-id="97d27-210">Si aparecen errores al usar la herramienta, envíe un problema en la sección [Issues](https://github.com/Azure/azure-cli/issues) (Problemas) del repositorio de GitHub.</span><span class="sxs-lookup"><span data-stu-id="97d27-210">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="97d27-211">Para proporcionar comentarios desde la línea de comandos, use el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="97d27-211">To provide feedback from the command line, use the `az feedback` command.</span></span>
