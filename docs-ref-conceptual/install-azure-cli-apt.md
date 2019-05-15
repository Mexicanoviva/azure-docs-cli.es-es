---
title: Instalación de la CLI de Azure en Linux con apt
description: Instalación de la CLI de Azure con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: af82eea3fd549cbca85699a3030a19bc82574b73
ms.sourcegitcommit: c65c69bd08fd6b7632ba60dc7c8e9f2b57a9d0b7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/09/2019
ms.locfileid: "65476259"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="db3b4-103">Instalación de la CLI de Azure con apt</span><span class="sxs-lookup"><span data-stu-id="db3b4-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="db3b4-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete x86_64 disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="db3b4-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="db3b4-105">Este paquete se ha probado y es compatible con:</span><span class="sxs-lookup"><span data-stu-id="db3b4-105">This package has been tested with and is supported for:</span></span>

* <span data-ttu-id="db3b4-106">Ubuntu trusty, xenial, artful, bionic y disco</span><span class="sxs-lookup"><span data-stu-id="db3b4-106">Ubuntu trusty, xenial, artful, bionic, and disco</span></span>
* <span data-ttu-id="db3b4-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="db3b4-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="db3b4-108">El paquete para la CLI de Azure instala su propio intérprete de Python y no utiliza el sistema Python.</span><span class="sxs-lookup"><span data-stu-id="db3b4-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="db3b4-109">Instalación</span><span class="sxs-lookup"><span data-stu-id="db3b4-109">Install</span></span>

<span data-ttu-id="db3b4-110">Ofrecemos dos formas de instalar la CLI de Azure con las distribuciones compatibles con `apt`: Como un script integral que ejecuta automáticamente los comandos de instalación, y con instrucciones que puede seguir paso a paso por su cuenta.</span><span class="sxs-lookup"><span data-stu-id="db3b4-110">We offer two ways to install the Azure CLI with distributions that support `apt`: As an all-in-one script that runs the install commands for you, and instructions that you can run as a step-by-step process on your own.</span></span>

### <a name="install-with-one-command"></a><span data-ttu-id="db3b4-111">Instalación con un comando</span><span class="sxs-lookup"><span data-stu-id="db3b4-111">Install with one command</span></span>

<span data-ttu-id="db3b4-112">Ofrecemos y mantenemos un script que ejecuta todos los comandos de instalación en un solo paso.</span><span class="sxs-lookup"><span data-stu-id="db3b4-112">We offer and maintain a script which runs all of the installation commands in one step.</span></span> <span data-ttu-id="db3b4-113">Ejecútelo con `curl` y canalícelo directamente a `bash`, o descargue el script en un archivo e inspecciónelo antes de ejecutarlo.</span><span class="sxs-lookup"><span data-stu-id="db3b4-113">Run it by using `curl` and pipe directly to `bash`, or download the script to a file and inspect it before running.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="db3b4-114">Este script solo se ha comprobado con Ubuntu 16.04 y Debian 8, y las versiones posteriores de ambos.</span><span class="sxs-lookup"><span data-stu-id="db3b4-114">This script is only verified for Ubuntu 16.04+ and Debian 8+.</span></span> <span data-ttu-id="db3b4-115">Puede que no funcione en otras distribuciones.</span><span class="sxs-lookup"><span data-stu-id="db3b4-115">It may not work on other distributions.</span></span>
> <span data-ttu-id="db3b4-116">Si usa una distribución derivada como Linux Mint, siga las instrucciones de instalación manual y solucione todos los posibles problemas.</span><span class="sxs-lookup"><span data-stu-id="db3b4-116">If you're using a derived distribution such as Linux Mint, follow the manual install instructions and perform any necessary troubleshooting.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a><span data-ttu-id="db3b4-117">Instrucciones de instalación manual</span><span class="sxs-lookup"><span data-stu-id="db3b4-117">Manual install instructions</span></span>

<span data-ttu-id="db3b4-118">Si no desea ejecutar un script como superusuario, siga estos pasos manuales para instalar la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="db3b4-118">If you don't want to run a script as superuser, follow these manual steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="db3b4-119">Obtenga los paquetes necesarios para el proceso de instalación:</span><span class="sxs-lookup"><span data-stu-id="db3b4-119">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="db3b4-120">Descargue e instale la clave de firma de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="db3b4-120">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="db3b4-121">Agregue el repositorio de software de la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="db3b4-121">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="db3b4-122">Actualice la información del repositorio e instale el paquete `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="db3b4-122">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="db3b4-123">Ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="db3b4-123">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="db3b4-124">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="db3b4-124">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="db3b4-125">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="db3b4-125">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="db3b4-126">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="db3b4-126">Troubleshooting</span></span>

<span data-ttu-id="db3b4-127">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="db3b4-127">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="db3b4-128">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="db3b4-128">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="db3b4-129">lsb_release no devuelve la versión de distribución de base correcta</span><span class="sxs-lookup"><span data-stu-id="db3b4-129">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="db3b4-130">Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="db3b4-130">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="db3b4-131">Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar.</span><span class="sxs-lookup"><span data-stu-id="db3b4-131">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="db3b4-132">Si conoce el nombre de código de la versión de Ubuntu o Debian de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente al [agregar el repositorio](#set-release).</span><span class="sxs-lookup"><span data-stu-id="db3b4-132">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="db3b4-133">En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre del código de distribución base y establezca `AZ_REPO` en el valor correcto.</span><span class="sxs-lookup"><span data-stu-id="db3b4-133">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="db3b4-134">No hay ningún paquete para su distribución</span><span class="sxs-lookup"><span data-stu-id="db3b4-134">No package for your distribution</span></span>

<span data-ttu-id="db3b4-135">A veces hace falta un tiempo desde el lanzamiento de una distribución para que haya un paquete de la CLI de Azure disponible.</span><span class="sxs-lookup"><span data-stu-id="db3b4-135">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="db3b4-136">La CLI de Azure se ha diseñado para ser resistente con respecto a versiones futuras de las dependencias, y a usar las menos posibles.</span><span class="sxs-lookup"><span data-stu-id="db3b4-136">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="db3b4-137">Si no hay ningún paquete disponible para su distribución de base, pruebe un paquete de una distribución anterior.</span><span class="sxs-lookup"><span data-stu-id="db3b4-137">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="db3b4-138">Para ello, establezca el valor de `AZ_REPO` manualmente al [agregar el repositorio](#set-release).</span><span class="sxs-lookup"><span data-stu-id="db3b4-138">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="db3b4-139">Para las distribuciones de Ubuntu, use el repositorio `disco` y, para las distribuciones de Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="db3b4-139">For Ubuntu distributions use the `disco` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="db3b4-140">Las distribuciones lanzadas antes de Ubuntu Trusty y Debian Wheezy no se admiten.</span><span class="sxs-lookup"><span data-stu-id="db3b4-140">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="db3b4-141">Actualizar</span><span class="sxs-lookup"><span data-stu-id="db3b4-141">Update</span></span>

<span data-ttu-id="db3b4-142">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="db3b4-142">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="db3b4-143">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="db3b4-143">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="db3b4-144">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="db3b4-144">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="db3b4-145">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="db3b4-145">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="db3b4-146">Desinstale con `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="db3b4-146">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="db3b4-147">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="db3b4-147">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="db3b4-148">Quite la clave de firma:</span><span class="sxs-lookup"><span data-stu-id="db3b4-148">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="db3b4-149">Quite los paquetes que no necesite:</span><span class="sxs-lookup"><span data-stu-id="db3b4-149">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="db3b4-150">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="db3b4-150">Next Steps</span></span>

<span data-ttu-id="db3b4-151">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="db3b4-151">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="db3b4-152">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="db3b4-152">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
