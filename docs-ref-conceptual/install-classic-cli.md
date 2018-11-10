---
title: Instalación de la CLI clásica de Azure
description: Instalación de la CLI clásica de Azure para Mac, Linux y Windows con el objetivo de comenzar a utilizar los servicios de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 78043f9c070626545030971dea2a8fd155ac76c2
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222470"
---
# <a name="install-the-azure-classic-cli"></a><span data-ttu-id="b301f-103">Instalación de la CLI clásica de Azure</span><span class="sxs-lookup"><span data-stu-id="b301f-103">Install the Azure classic CLI</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b301f-104">Este tema describe cómo instalar la CLI clásica de Azure.</span><span class="sxs-lookup"><span data-stu-id="b301f-104">This topic describes how to install the Azure classic CLI.</span></span> <span data-ttu-id="b301f-105">La CLI clásica está en desuso y solo debe usarse con el modelo de implementación clásico.</span><span class="sxs-lookup"><span data-stu-id="b301f-105">The classic CLI is deprecated and should only be used with the classic deployment model.</span></span>
> <span data-ttu-id="b301f-106">Para todas las demás implementaciones, utilice [la CLI de Azure](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="b301f-106">For all other deployments, use [the Azure CLI](/cli/azure).</span></span>

<span data-ttu-id="b301f-107">Instale rápidamente la CLI clásica de Azure para utilizar un conjunto de comandos de código abierto basados en shell para crear y administrar recursos en Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="b301f-107">Quickly install the Azure classic CLI to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="b301f-108">Tiene varias opciones para instalar estas herramientas multiplataforma en su equipo:</span><span class="sxs-lookup"><span data-stu-id="b301f-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="b301f-109">**Paquete de npm**: ejecute npm (el administrador de paquetes para JavaScript) para instalar el paquete de la CLI clásica de Azure en su distribución de Linux o sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="b301f-109">**npm package** - Run npm (the package manager for JavaScript) to install the Azure classic CLI package on your Linux distribution or OS.</span></span> <span data-ttu-id="b301f-110">Se requieren node.js y npm.</span><span class="sxs-lookup"><span data-stu-id="b301f-110">Requires node.js and npm.</span></span>
* <span data-ttu-id="b301f-111">**Instalador**: descargue un instalador para facilitar la instalación en Mac o Windows.</span><span class="sxs-lookup"><span data-stu-id="b301f-111">**Installer** - Download an installer for easy installation on macOS or Windows.</span></span>
* <span data-ttu-id="b301f-112">**Contenedor de Docker**: empiece a usar la CLI clásica en un contenedor de Docker listo para ejecutarse.</span><span class="sxs-lookup"><span data-stu-id="b301f-112">**Docker container** - Start using the classic CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="b301f-113">Requiere un host de Docker.</span><span class="sxs-lookup"><span data-stu-id="b301f-113">Requires a Docker host.</span></span>

<span data-ttu-id="b301f-114">Si desea obtener más opciones y los antecedentes, consulte el repositorio del proyecto en [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="b301f-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="b301f-115">Una vez que instale la CLI clásica de Azure, conéctese con `azure login` y ejecute los comandos `azure` desde la interfaz de la línea de comandos (Bash, Terminal, símbolo del sistema, etc.) para trabajar con los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="b301f-115">Once the Azure classic CLI is installed, connect with `azure login` and run the `azure` commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="b301f-116">Opción 1: Instalación de un paquete de NPM</span><span class="sxs-lookup"><span data-stu-id="b301f-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="b301f-117">Para instalar la CLI clásica desde un paquete de npm, asegúrese de que ha descargado e instalado la versión [más reciente de Node.js y npm](https://nodejs.org/en/download/package-manager/).</span><span class="sxs-lookup"><span data-stu-id="b301f-117">To install the classic CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="b301f-118">A continuación, ejecute `npm install` para instalar el paquete azure-cli:</span><span class="sxs-lookup"><span data-stu-id="b301f-118">Then, run `npm install` to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="b301f-119">En distribuciones de Linux, es posible que tenga que usar `sudo` para ejecutar correctamente el comando `npm`, tal como se muestra a continuación:</span><span class="sxs-lookup"><span data-stu-id="b301f-119">On Linux distributions, you might need to use `sudo` to successfully run the `npm` command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="b301f-120">Si necesita instalar o actualizar Node.js y npm en el sistema operativo, se recomienda instalar Node.js LTS versión 4.x o posterior.</span><span class="sxs-lookup"><span data-stu-id="b301f-120">If you need to install or update Node.js and npm on your OS, we recommend that you install Node.js LTS version 4.x or later.</span></span> <span data-ttu-id="b301f-121">Si utiliza una versión anterior, podrían producirse errores de instalación.</span><span class="sxs-lookup"><span data-stu-id="b301f-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="b301f-122">Si lo prefiere, también puede descargar un archivo tar desde las [versiones de GitHub](https://github.com/Azure/azure-xplat-cli/releases).</span><span class="sxs-lookup"><span data-stu-id="b301f-122">If you prefer, you may also download a tar file from the [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span> <span data-ttu-id="b301f-123">Después, instale el paquete de npm descargado de la siguiente manera (en las distribuciones de Linux podría tener que usar `sudo`):</span><span class="sxs-lookup"><span data-stu-id="b301f-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use `sudo`):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="b301f-124">Opción 2: Uso de un instalador</span><span class="sxs-lookup"><span data-stu-id="b301f-124">Option 2: Use an installer</span></span>

<span data-ttu-id="b301f-125">Si usa un equipo Mac o Windows, los instaladores DMG y MSI están disponibles en [versiones de GitHub](https://github.com/Azure/azure-xplat-cli/releases).</span><span class="sxs-lookup"><span data-stu-id="b301f-125">If you use a Mac or Windows computer, DMG and MSI installers are available from [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span>

> [!TIP]
> <span data-ttu-id="b301f-126">En Windows, también puede descargar el [Instalador de plataforma web](https://go.microsoft.com/?linkid=9828653) para instalar la CLI clásica.</span><span class="sxs-lookup"><span data-stu-id="b301f-126">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the classic CLI.</span></span> <span data-ttu-id="b301f-127">Este instalador ofrece la opción de instalar SDK de Azure adicionales y herramientas de la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="b301f-127">This installer gives you the option to install additional Azure SDK and command-line tools.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="b301f-128">Opción 3: Uso de un contenedor Docker</span><span class="sxs-lookup"><span data-stu-id="b301f-128">Option 3: Use a Docker container</span></span>

<span data-ttu-id="b301f-129">Si ha configurado el equipo como un host de [Docker](https://docs.docker.com/engine/understanding-docker/), puede ejecutar la CLI clásica de Azure en un contenedor de Docker.</span><span class="sxs-lookup"><span data-stu-id="b301f-129">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the Azure classic CLI in a Docker container.</span></span> <span data-ttu-id="b301f-130">Ejecute el comando siguiente (en las distribuciones de Linux, es posible que tenga que usar `sudo`):</span><span class="sxs-lookup"><span data-stu-id="b301f-130">Run the following command (on Linux distributions you might need to use `sudo`):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a><span data-ttu-id="b301f-131">Ejecución de los comandos de la CLI clásica de Azure</span><span class="sxs-lookup"><span data-stu-id="b301f-131">Run Azure classic CLI commands</span></span>

<span data-ttu-id="b301f-132">Una vez instalada la CLI clásica de Azure, ejecute el comando `azure` desde la interfaz de usuario de la línea de comandos (Bash, Terminal, símbolo del sistema, etc.).</span><span class="sxs-lookup"><span data-stu-id="b301f-132">After the classic CLI is installed, run the `azure` command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="b301f-133">Por ejemplo, si desea ejecutar el comando help, escriba lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="b301f-133">For example, to run the help command, type the following:</span></span>

```azurecli-interactive
azure help
```

> [!NOTE]
> <span data-ttu-id="b301f-134">En algunas distribuciones de Linux, puede recibir un error similar al `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="b301f-134">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="b301f-135">Este error procede de las instalaciones recientes de Node.js que se instala en /usr/bin/nodejs.</span><span class="sxs-lookup"><span data-stu-id="b301f-135">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="b301f-136">Para corregirlo, cree un vínculo simbólico a /usr/bin/node, para lo que debe ejecutar este comando:</span><span class="sxs-lookup"><span data-stu-id="b301f-136">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="b301f-137">Para saber qué versión de la CLI clásica de Azure se ha instalado, escriba lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="b301f-137">To see the version of the Azure classic CLI installed, type the following:</span></span>

```azurecli-interactive
azure --version
```

> [!NOTE]
> <span data-ttu-id="b301f-138">La primera vez que usa la CLI clásica de Azure, verá un mensaje en el que se le pregunta si quiere permitir que Microsoft recopile información de uso.</span><span class="sxs-lookup"><span data-stu-id="b301f-138">When you first use Azure classic CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="b301f-139">La participación es voluntaria.</span><span class="sxs-lookup"><span data-stu-id="b301f-139">Participation is voluntary.</span></span> <span data-ttu-id="b301f-140">Si elige participar, puede dejar de hacerlo cuando desee mediante la ejecución de `azure telemetry --disable`.</span><span class="sxs-lookup"><span data-stu-id="b301f-140">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="b301f-141">Para habilitar la participación en cualquier momento, ejecute `azure telemetry --enable`.</span><span class="sxs-lookup"><span data-stu-id="b301f-141">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-classic-cli"></a><span data-ttu-id="b301f-142">Actualización de la CLI clásica</span><span class="sxs-lookup"><span data-stu-id="b301f-142">Update the classic CLI</span></span>

<span data-ttu-id="b301f-143">Microsoft puede liberar versiones actualizadas de la CLI clásica de Azure.</span><span class="sxs-lookup"><span data-stu-id="b301f-143">Microsoft may release updated versions of the Azure classic CLI.</span></span> <span data-ttu-id="b301f-144">Vuelva a instalar la CLI clásica mediante el programa de instalación para su sistema operativo o ejecute el contenedor de Docker más reciente.</span><span class="sxs-lookup"><span data-stu-id="b301f-144">Reinstall the classic CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="b301f-145">O bien, si tiene las versiones de Node.js y npm más recientes instaladas, escriba lo siguiente para efectuar la actualización (en las distribuciones de Linux, es posible que necesite utilizar `sudo`).</span><span class="sxs-lookup"><span data-stu-id="b301f-145">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use `sudo`).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="b301f-146">Habilitación de la función de autocompletar</span><span class="sxs-lookup"><span data-stu-id="b301f-146">Enable tab completion</span></span>

<span data-ttu-id="b301f-147">La función de autocompletar de los comandos de la CLI clásica es compatible con Mac y Linux.</span><span class="sxs-lookup"><span data-stu-id="b301f-147">Tab completion of classic CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="b301f-148">Para habilitarla en zsh, ejecute el siguiente código:</span><span class="sxs-lookup"><span data-stu-id="b301f-148">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="b301f-149">Para habilitarla en Bash, ejecute el siguiente código:</span><span class="sxs-lookup"><span data-stu-id="b301f-149">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="b301f-150">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="b301f-150">Next steps</span></span>

* <span data-ttu-id="b301f-151">Para más información acerca de la CLI clásica de Azure, descargar el código fuente, informar sobre problemas o colaborar con el proyecto, visite el [Repositorio de GitHub para la CLI clásica de Azure](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="b301f-151">To learn more about the Azure classic CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli).</span></span>
