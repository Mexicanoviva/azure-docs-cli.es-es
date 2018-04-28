---
title: Instalación de la CLI de Azure 1.0
description: Instalación de la CLI de Azure 1.0 para Mac, Linux y Windows con el objetivo de comenzar a utilizar los servicios de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/20/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 92714f32736e0a1a0ea7c8dd4a615b158c955931
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2018
---
# <a name="install-the-azure-cli-10"></a><span data-ttu-id="9e545-103">Instalación de la CLI de Azure 1.0</span><span class="sxs-lookup"><span data-stu-id="9e545-103">Install the Azure CLI 1.0</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9e545-104">En este tema se describe cómo instalar la CLI de Azure 1.0.</span><span class="sxs-lookup"><span data-stu-id="9e545-104">This topic describes how to install the Azure CLI 1.0.</span></span> <span data-ttu-id="9e545-105">Esta CLI está en desuso y solo debe usarse para la compatibilidad del modelo Azure Service Management (ASM) con recursos "clásicos".</span><span class="sxs-lookup"><span data-stu-id="9e545-105">This CLI is deprecated and should only be used for support with the Azure Service Management (ASM) model with "classic" resources.</span></span>
> <span data-ttu-id="9e545-106">Para las implementaciones de Azure Resource Manager, use la [CLI de Azure 2.0](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="9e545-106">For Azure Resource Manager deployments, use [Azure CLI 2.0](/cli/azure).</span></span>

<span data-ttu-id="9e545-107">Instale rápidamente la interfaz de la línea de comandos de Azure (CLI de Azure 1.0) para utilizar un conjunto de comandos de código abierto basados en shell para crear y administrar recursos en Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="9e545-107">Quickly install the Azure Command-Line Interface (Azure CLI 1.0) to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="9e545-108">Tiene varias opciones para instalar estas herramientas multiplataforma en su equipo:</span><span class="sxs-lookup"><span data-stu-id="9e545-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="9e545-109">**Paquete de npm** : ejecute npm (el administrador de paquetes de JavaScript) para instalar el paquete de la CLI de Azure 1.0 más reciente en su distribución de Linux o sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="9e545-109">**npm package** - Run npm (the package manager for JavaScript) to install the latest Azure CLI 1.0 package on your Linux distribution or OS.</span></span> <span data-ttu-id="9e545-110">Se requiere que node.js y npm estén instalados en su equipo.</span><span class="sxs-lookup"><span data-stu-id="9e545-110">Requires node.js and npm on your computer.</span></span>
* <span data-ttu-id="9e545-111">**Instalador** : descargue un instalador para facilitar la instalación en Mac o Windows.</span><span class="sxs-lookup"><span data-stu-id="9e545-111">**Installer** - Download an installer for easy installation on Mac or Windows.</span></span>
* <span data-ttu-id="9e545-112">**Contenedor de Docker** : empiece usando la CLI más reciente en un contenedor de Docker listos para ejecutarse.</span><span class="sxs-lookup"><span data-stu-id="9e545-112">**Docker container** - Start using the latest CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="9e545-113">Se requiere el host de Docker en su equipo.</span><span class="sxs-lookup"><span data-stu-id="9e545-113">Requires Docker host on your computer.</span></span>

<span data-ttu-id="9e545-114">Si desea obtener más opciones y los antecedentes, consulte el repositorio del proyecto en [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="9e545-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="9e545-115">Una vez que instale la CLI de Azure 1.0, [conéctela con su suscripción a Azure](/cli/azure/authenticate-azure-cli) y ejecute los comandos **azure** desde la interfaz de la línea de comandos (Bash, Terminal, símbolo del sistema, etc.) para trabajar con sus recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="9e545-115">Once the Azure CLI 1.0 is installed, [connect it with your Azure subscription](/cli/azure/authenticate-azure-cli) and run the **azure** commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="9e545-116">Opción 1: Instalación de un paquete de NPM</span><span class="sxs-lookup"><span data-stu-id="9e545-116">Option 1: Install an npm package</span></span>
<span data-ttu-id="9e545-117">Para instalar la CLI desde un paquete de npm, necesita la versión [más reciente de Node.js y npm instalada en su sistema](https://nodejs.org/en/download/package-manager/).</span><span class="sxs-lookup"><span data-stu-id="9e545-117">To install the CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="9e545-118">A continuación, ejecute **instalar npm** para instalar el paquete azure-cli:</span><span class="sxs-lookup"><span data-stu-id="9e545-118">Then, run **npm install** to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="9e545-119">En distribuciones de Linux, es posible que tenga que usar **sudo** para ejecutar correctamente el comando **npm**, tal como se muestra a continuación:</span><span class="sxs-lookup"><span data-stu-id="9e545-119">On Linux distributions, you might need to use **sudo** to successfully run the **npm** command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="9e545-120">Si necesita instalar o actualizar Node.js y npm en la distribución de Linux o el SO, recomendamos instalar la versión LTS de Node.js más reciente (4.x).</span><span class="sxs-lookup"><span data-stu-id="9e545-120">If you need to install or update Node.js and npm on your Linux distribution or OS, we recommend that you install the most recent Node.js LTS version (4.x).</span></span> <span data-ttu-id="9e545-121">Si utiliza una versión anterior, podrían producirse errores de instalación.</span><span class="sxs-lookup"><span data-stu-id="9e545-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="9e545-122">Si lo prefiere, descargue el [archivo .tar][linux-installer] de Linux más reciente para el paquete de npm localmente.</span><span class="sxs-lookup"><span data-stu-id="9e545-122">If you prefer, download the latest Linux [tar file][linux-installer] for the npm package locally.</span></span> <span data-ttu-id="9e545-123">Después, instale el paquete de npm descargado de la siguiente manera (en las distribuciones de Linux podría tener que usar **sudo**):</span><span class="sxs-lookup"><span data-stu-id="9e545-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use **sudo**):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="9e545-124">Opción 2: Uso de un instalador</span><span class="sxs-lookup"><span data-stu-id="9e545-124">Option 2: Use an installer</span></span>
<span data-ttu-id="9e545-125">Si utiliza un equipo Mac o Windows, los instaladores de la CLI siguientes están disponibles para descargarse:</span><span class="sxs-lookup"><span data-stu-id="9e545-125">If you use a Mac or Windows computer, the following CLI installers are available for download:</span></span>

* <span data-ttu-id="9e545-126">[Instalador de Mac OS X][mac-installer]</span><span class="sxs-lookup"><span data-stu-id="9e545-126">[Mac OS X installer][mac-installer]</span></span>
* <span data-ttu-id="9e545-127">[MSI de Windows][windows-installer]</span><span class="sxs-lookup"><span data-stu-id="9e545-127">[Windows MSI][windows-installer]</span></span>

> [!TIP]
> <span data-ttu-id="9e545-128">En Windows, también puede descargar el [Instalador de plataforma web](https://go.microsoft.com/?linkid=9828653) para instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="9e545-128">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the CLI.</span></span> <span data-ttu-id="9e545-129">Este instalador ofrece la opción de instalar otros Azure SDK y herramientas de línea de comandos después de instalar la CLI.</span><span class="sxs-lookup"><span data-stu-id="9e545-129">This installer gives you the option to install additional Azure SDK and command-line tools after installing the CLI.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="9e545-130">Opción 3: Uso de un contenedor Docker</span><span class="sxs-lookup"><span data-stu-id="9e545-130">Option 3: Use a Docker container</span></span>
<span data-ttu-id="9e545-131">Si ha configurado un host de [Docker](https://docs.docker.com/engine/understanding-docker/), puede ejecutar la CLI de Azure 1.0 más reciente en un contenedor de Docker.</span><span class="sxs-lookup"><span data-stu-id="9e545-131">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the latest Azure CLI 1.0 in a Docker container.</span></span> <span data-ttu-id="9e545-132">Ejecute el comando siguiente (en las distribuciones de Linux, es posible que tenga que usar **sudo**):</span><span class="sxs-lookup"><span data-stu-id="9e545-132">Run the following command (on Linux distributions you might need to use **sudo**):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-cli-10-commands"></a><span data-ttu-id="9e545-133">Ejecución de los comandos de la CLI de Azure 1.0</span><span class="sxs-lookup"><span data-stu-id="9e545-133">Run Azure CLI 1.0 commands</span></span>
<span data-ttu-id="9e545-134">Una vez instalada la CLI de Azure 1.0, ejecute el comando **azure** desde su interfaz de usuario de la línea de comandos (Bash, Terminal, símbolo del sistema, etc.).</span><span class="sxs-lookup"><span data-stu-id="9e545-134">After the Azure CLI 1.0 is installed, run the **azure** command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="9e545-135">Por ejemplo, si desea ejecutar el comando help, escriba lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="9e545-135">For example, to run the help command, type the following:</span></span>

```azurecli
azure help
```

> [!NOTE]
> <span data-ttu-id="9e545-136">En algunas distribuciones de Linux, puede recibir un error similar al `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="9e545-136">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="9e545-137">Este error procede de las instalaciones recientes de Node.js que se instala en /usr/bin/nodejs.</span><span class="sxs-lookup"><span data-stu-id="9e545-137">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="9e545-138">Para corregirlo, cree un vínculo simbólico a /usr/bin/node, para lo que debe ejecutar este comando:</span><span class="sxs-lookup"><span data-stu-id="9e545-138">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="9e545-139">Para saber qué versión de la CLI de Azure 1.0 instaló, escriba lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="9e545-139">To see the version of the Azure CLI 1.0 you installed, type the following:</span></span>

```azurecli
azure --version
```

<span data-ttu-id="9e545-140">De este modo, ya está listo.</span><span class="sxs-lookup"><span data-stu-id="9e545-140">Now you are ready!</span></span> <span data-ttu-id="9e545-141">Para obtener acceso a todos los comandos de la CLI para trabajar con sus propios recursos, [conéctese a su suscripción a Azure desde la CLI de Azure](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="9e545-141">To access all the CLI commands to work with your own resources, [connect to your Azure subscription from the Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="9e545-142">La primera vez que usa la CLI de Azure, ve un mensaje en el que se le pregunta si quiere permitir que Microsoft recopile información.</span><span class="sxs-lookup"><span data-stu-id="9e545-142">When you first use Azure CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="9e545-143">La participación es voluntaria.</span><span class="sxs-lookup"><span data-stu-id="9e545-143">Participation is voluntary.</span></span> <span data-ttu-id="9e545-144">Si elige participar, puede dejar de hacerlo cuando desee mediante la ejecución de `azure telemetry --disable`.</span><span class="sxs-lookup"><span data-stu-id="9e545-144">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="9e545-145">Para habilitar la participación en cualquier momento, ejecute `azure telemetry --enable`.</span><span class="sxs-lookup"><span data-stu-id="9e545-145">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-cli"></a><span data-ttu-id="9e545-146">Actualización de la CLI</span><span class="sxs-lookup"><span data-stu-id="9e545-146">Update the CLI</span></span>
<span data-ttu-id="9e545-147">Microsoft publica con frecuencia versiones actualizadas de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="9e545-147">Microsoft frequently releases updated versions of the Azure CLI.</span></span> <span data-ttu-id="9e545-148">Vuelva a instalar la CLI mediante el programa de instalación para su sistema operativo o ejecute el contenedor de Docker más reciente.</span><span class="sxs-lookup"><span data-stu-id="9e545-148">Reinstall the CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="9e545-149">Si tiene Node.js y npm más recientes instalados, escriba lo siguiente para efectuar la actualización (en las distribuciones de Linux, es posible que necesite utilizar **sudo**).</span><span class="sxs-lookup"><span data-stu-id="9e545-149">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use **sudo**).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="9e545-150">Habilitación de la función de autocompletar</span><span class="sxs-lookup"><span data-stu-id="9e545-150">Enable tab completion</span></span>
<span data-ttu-id="9e545-151">La función de autocompletar de los comandos de la CLI es compatible con Mac y Linux.</span><span class="sxs-lookup"><span data-stu-id="9e545-151">Tab completion of CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="9e545-152">Para habilitarla en zsh, ejecute el siguiente código:</span><span class="sxs-lookup"><span data-stu-id="9e545-152">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="9e545-153">Para habilitarla en Bash, ejecute el siguiente código:</span><span class="sxs-lookup"><span data-stu-id="9e545-153">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```


## <a name="next-steps"></a><span data-ttu-id="9e545-154">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="9e545-154">Next steps</span></span>
* <span data-ttu-id="9e545-155">[Conexión a una suscripción de Azure desde la interfaz de la línea de comandos de Azure (CLI de Azure)](/cli/azure/authenticate-azure-cli) para crear y administrar recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="9e545-155">[Connect from the CLI to your Azure subscription](/cli/azure/authenticate-azure-cli) to create and manage Azure resources.</span></span>
* <span data-ttu-id="9e545-156">Si desea obtener más información acerca de la CLI de Azure, descargar el código fuente, informar sobre problemas o colaborar con el proyecto, visite el [Repositorio de GitHub para la CLI de Azure](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="9e545-156">To learn more about the Azure CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure CLI](https://github.com/azure/azure-xplat-cli).</span></span>
* <span data-ttu-id="9e545-157">Si tiene preguntas acerca de cómo usar la CLI de Azure o sobre Azure, visite los [foros de Azure](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span><span class="sxs-lookup"><span data-stu-id="9e545-157">If you have questions about using the Azure CLI, or Azure, visit the [Azure Forums](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span></span>


[mac-installer]: http://aka.ms/mac-azure-cli
[windows-installer]: http://aka.ms/webpi-azure-cli
[linux-installer]: http://aka.ms/linux-azure-cli
[cliasm]: /cli/azure/get-started-with-az-cli2
[cliarm]: ./virtual-machines/azure-cli-arm-commands.md
