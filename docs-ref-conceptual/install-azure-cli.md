---
title: "Instalación de la CLI de Azure 2.0"
description: "Documentos de referencia para la instalación de la CLI de Azure 2.0"
keywords: "CLI de Azure 2.0, Referencia de la CLI de Azure 2.0, Instalación de la CLI de Azure 2.0, CLI de CLI de Python de Azure, Desinstalación de la CLI de Azure 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 08/17/2017
ms.topic: "articleå"
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 432edac070e238a6f1be0ccd76b9b3582b082219
ms.sourcegitcommit: 2ec80224c6b831e31038b710d912c0dbb1ddfef6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/17/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="bdbda-104">Instalación de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="bdbda-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="bdbda-105">Instale hoy mismo la nueva versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="bdbda-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="bdbda-106">La hemos mejorado y actualizado para facilitar la administración nativa de los recursos de Azure desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="bdbda-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="bdbda-107">Se puede usar en macOS, Linux y Windows.</span><span class="sxs-lookup"><span data-stu-id="bdbda-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="bdbda-108">Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bdbda-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="bdbda-109">Si necesita la versión anterior de la CLI de Azure, vea aquí cómo [instalar la CLI de Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="bdbda-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="bdbda-110">macOS</span><span class="sxs-lookup"><span data-stu-id="bdbda-110">macOS</span></span>

> [!WARNING]
> <span data-ttu-id="bdbda-111">La fórmula de Homebrew para la CLI de Azure, `azure-cli`, actualmente no está actualizada e instalará una versión anterior.</span><span class="sxs-lookup"><span data-stu-id="bdbda-111">The Homebrew formula for the Azure CLI, `azure-cli`, is currently out of date and will install a previous version.</span></span>

1. <span data-ttu-id="bdbda-112">Instale la CLI de Azure 2.0 con un comando `curl`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-112">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="bdbda-113">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell de comandos.</span><span class="sxs-lookup"><span data-stu-id="bdbda-113">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="bdbda-114">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-114">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="bdbda-115">Cuando la instalación se realiza con InstallAzureCli, no se admite [`az component update`](/cli/azure/component#update).</span><span class="sxs-lookup"><span data-stu-id="bdbda-115">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="bdbda-116">Para actualizar a la CLI más reciente, vuelva a ejecutar `curl -L https://aka.ms/InstallAzureCli | bash`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-116">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="bdbda-117">Para desinstalarla, consulte las [instrucciones de desinstalación del manual](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="bdbda-117">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="bdbda-118">Windows</span><span class="sxs-lookup"><span data-stu-id="bdbda-118">Windows</span></span>

<span data-ttu-id="bdbda-119">Puede instalar la CLI de Azure 2.0 con el archivo MSI y utilizarla en la línea de comandos de Windows, o puede instalar la CLI con apt-get en Bash en Ubuntu o Windows.</span><span class="sxs-lookup"><span data-stu-id="bdbda-119">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="bdbda-120">MSI para la línea de comandos de Windows</span><span class="sxs-lookup"><span data-stu-id="bdbda-120">MSI for the Windows command-line</span></span> 

<span data-ttu-id="bdbda-121">Para instalar la CLI en Windows y usarla en la línea de comandos de Windows, descargue y ejecute el archivo [msi](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="bdbda-121">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="bdbda-122">Si la instalación se realiza con el archivo msi, no se admite [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="bdbda-122">When you install with the msi, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="bdbda-123">Para actualizar a la última CLI, ejecute [msi](https://aka.ms/InstallAzureCliWindows) de nuevo.</span><span class="sxs-lookup"><span data-stu-id="bdbda-123">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="bdbda-124">Para desinstalar la CLI, ejecute [msi](https://aka.ms/InstallAzureCliWindows) de nuevo y elija la opción de desinstalación.</span><span class="sxs-lookup"><span data-stu-id="bdbda-124">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="bdbda-125">apt-get para Bash en Ubuntu en Windows</span><span class="sxs-lookup"><span data-stu-id="bdbda-125">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="bdbda-126">Si no dispone de Bash en Windows, [instálelo](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="bdbda-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="bdbda-127">Abra el shell de Bash.</span><span class="sxs-lookup"><span data-stu-id="bdbda-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="bdbda-128">Modifique la lista de orígenes.</span><span class="sxs-lookup"><span data-stu-id="bdbda-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="bdbda-129">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="bdbda-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="bdbda-130">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-130">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="bdbda-131">Si la instalación se realiza con apt-get, no se admite [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="bdbda-131">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="bdbda-132">Para actualizar la CLI, vuelva a ejecutar `sudo apt-get update && sudo apt-get install azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-132">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="bdbda-133">Para desinstalarla, ejecute `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-133">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="apt-get-for-debianubuntu"></a><span data-ttu-id="bdbda-134">apt-get para Debian y Ubuntu</span><span class="sxs-lookup"><span data-stu-id="bdbda-134">apt-get for Debian/Ubuntu</span></span>

<span data-ttu-id="bdbda-135">En los sistemas con Debian y Ubuntu, la CLI de Azure 2.0 se puede instalar a través de `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-135">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="bdbda-136">Modifique la lista de orígenes.</span><span class="sxs-lookup"><span data-stu-id="bdbda-136">Modify your sources list.</span></span>
 
   - <span data-ttu-id="bdbda-137">Sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="bdbda-137">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="bdbda-138">Sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="bdbda-138">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="bdbda-139">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="bdbda-139">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="bdbda-140">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-140">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="bdbda-141">Si la instalación se realiza con apt-get, no se admite [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="bdbda-141">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="bdbda-142">Para actualizar la CLI, vuelva a ejecutar `sudo apt-get update && sudo apt-get install azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-142">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="bdbda-143">Para desinstalarla, ejecute `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-143">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="docker"></a><span data-ttu-id="bdbda-144">Docker</span><span class="sxs-lookup"><span data-stu-id="bdbda-144">Docker</span></span>

<span data-ttu-id="bdbda-145">Mantenemos una imagen de Docker preconfigurada con la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="bdbda-145">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="bdbda-146">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-146">Install the CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="bdbda-147">Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="bdbda-147">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="bdbda-148">Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-148">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

>> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

<span data-ttu-id="bdbda-149">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-149">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="bdbda-150">La imagen de Docker no admite la característica [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="bdbda-150">The Docker image does not support the [`az component`](/cli/azure/component) feature.</span></span>
> <span data-ttu-id="bdbda-151">Para actualizar la CLI de Azure 2.0, utilice `docker run` para instalar la imagen más reciente, o la imagen específica que desee.</span><span class="sxs-lookup"><span data-stu-id="bdbda-151">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="linux"></a><span data-ttu-id="bdbda-152">Linux</span><span class="sxs-lookup"><span data-stu-id="bdbda-152">Linux</span></span>

1. <span data-ttu-id="bdbda-153">Si no lo tiene, instale [Python](https://www.python.org/downloads).</span><span class="sxs-lookup"><span data-stu-id="bdbda-153">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="bdbda-154">En función de la distribución de Linux, instale los requisitos previos.</span><span class="sxs-lookup"><span data-stu-id="bdbda-154">Depending on your Linux distribution, install the prerequisites.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

3. <span data-ttu-id="bdbda-155">Instalación de la CLI con un comando `curl`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-155">Install the CLI with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

4. <span data-ttu-id="bdbda-156">Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell de comandos.</span><span class="sxs-lookup"><span data-stu-id="bdbda-156">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

5. <span data-ttu-id="bdbda-157">Ejecute la CLI desde el símbolo del sistema con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-157">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="bdbda-158">Cuando la instalación se realiza con InstallAzureCli, no se admite [`az component update`](/cli/azure/component#update).</span><span class="sxs-lookup"><span data-stu-id="bdbda-158">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="bdbda-159">Para actualizar a la CLI más reciente, vuelva a ejecutar `curl -L https://aka.ms/InstallAzureCli | bash`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-159">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="bdbda-160">Para desinstalarla, consulte las [instrucciones de desinstalación del manual](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="bdbda-160">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="bdbda-161">Solución de problemas</span><span class="sxs-lookup"><span data-stu-id="bdbda-161">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="bdbda-162">Errores en el redireccionamiento de curl</span><span class="sxs-lookup"><span data-stu-id="bdbda-162">Errors with curl redirection</span></span>

<span data-ttu-id="bdbda-163">Si aparece un error en el comando `curl` relacionado con el parámetro `-L` o el error "Objeto movido", pruebe a usar la dirección URL completa, en lugar de la URL aka.ms:</span><span class="sxs-lookup"><span data-stu-id="bdbda-163">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a><span data-ttu-id="bdbda-164">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="bdbda-164">Uninstall</span></span>

<span data-ttu-id="bdbda-165">Si usó el script de https://aka.ms/InstallAzureCli para instalar la CLI, siga estos pasos para desinstalarla.</span><span class="sxs-lookup"><span data-stu-id="bdbda-165">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="bdbda-166">Quite los archivos instalados.</span><span class="sxs-lookup"><span data-stu-id="bdbda-166">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="bdbda-167">Elimine la línea `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-167">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="bdbda-168">La ubicación de instalación predeterminada es `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-168">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="bdbda-169">Si ha usado apt-get, Docker o el msi para instalar la CLI, utilice la misma herramienta para desinstalarla.</span><span class="sxs-lookup"><span data-stu-id="bdbda-169">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="bdbda-170">Notificación de problemas y comentarios</span><span class="sxs-lookup"><span data-stu-id="bdbda-170">Reporting issues and feedback</span></span>

<span data-ttu-id="bdbda-171">Si aparecen errores al usar la herramienta, envíe un problema en la sección [Issues](https://github.com/Azure/azure-cli/issues) (Problemas) del repositorio de GitHub.</span><span class="sxs-lookup"><span data-stu-id="bdbda-171">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="bdbda-172">Para enviar comentarios desde la línea de comandos, pruebe a hacerlo con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="bdbda-172">To provide feedback from the command line, try the `az feedback` command.</span></span>
