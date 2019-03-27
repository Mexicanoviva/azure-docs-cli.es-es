---
title: Instalación de la CLI de Azure en Linux con apt
description: Instalación de la CLI de Azure con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/19/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: fa2e1db439b4836d7506409b3abcce74fb6e6695
ms.sourcegitcommit: 5864f72b9a6fbf82a4d98bf805b3a16a7da18556
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/22/2019
ms.locfileid: "58343152"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="1cb20-103">Instalación de la CLI de Azure con apt</span><span class="sxs-lookup"><span data-stu-id="1cb20-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="1cb20-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete x86_64 disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="1cb20-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="1cb20-105">Este paquete se ha probado con:</span><span class="sxs-lookup"><span data-stu-id="1cb20-105">This package has been tested with:</span></span>

* <span data-ttu-id="1cb20-106">Ubuntu trusty, xenial, artful y bionic</span><span class="sxs-lookup"><span data-stu-id="1cb20-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="1cb20-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="1cb20-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="1cb20-108">El paquete para la CLI de Azure instala su propio intérprete de Python y no utiliza el sistema Python.</span><span class="sxs-lookup"><span data-stu-id="1cb20-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="1cb20-109">Instalación</span><span class="sxs-lookup"><span data-stu-id="1cb20-109">Install</span></span>

1. <span data-ttu-id="1cb20-110">Obtenga los paquetes necesarios para el proceso de instalación:</span><span class="sxs-lookup"><span data-stu-id="1cb20-110">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gpg
    ```

2. <span data-ttu-id="1cb20-111">Descargue e instale la clave de firma de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="1cb20-111">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="1cb20-112">Agregue el repositorio de software de la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="1cb20-112">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="1cb20-113">Actualice la información del repositorio e instale el paquete `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="1cb20-113">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="1cb20-114">Ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="1cb20-114">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="1cb20-115">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="1cb20-115">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1cb20-116">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1cb20-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1cb20-117">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="1cb20-117">Troubleshooting</span></span>

<span data-ttu-id="1cb20-118">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="1cb20-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="1cb20-119">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1cb20-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="1cb20-120">lsb_release no devuelve la versión de distribución de base correcta</span><span class="sxs-lookup"><span data-stu-id="1cb20-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="1cb20-121">Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="1cb20-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="1cb20-122">Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar.</span><span class="sxs-lookup"><span data-stu-id="1cb20-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="1cb20-123">Si conoce el nombre de código de la versión de Ubuntu o Debian de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente al [agregar el repositorio](#set-release).</span><span class="sxs-lookup"><span data-stu-id="1cb20-123">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="1cb20-124">En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre del código de distribución base y establezca `AZ_REPO` en el valor correcto.</span><span class="sxs-lookup"><span data-stu-id="1cb20-124">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="1cb20-125">No hay ningún paquete para su distribución</span><span class="sxs-lookup"><span data-stu-id="1cb20-125">No package for your distribution</span></span>

<span data-ttu-id="1cb20-126">A veces hace falta un tiempo desde el lanzamiento de una distribución para que haya un paquete de la CLI de Azure disponible.</span><span class="sxs-lookup"><span data-stu-id="1cb20-126">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="1cb20-127">La CLI de Azure se ha diseñado para ser resistente con respecto a versiones futuras de las dependencias, y a usar las menos posibles.</span><span class="sxs-lookup"><span data-stu-id="1cb20-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="1cb20-128">Si no hay ningún paquete disponible para su distribución de base, pruebe un paquete de una distribución anterior.</span><span class="sxs-lookup"><span data-stu-id="1cb20-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="1cb20-129">Para ello, establezca el valor de `AZ_REPO` manualmente al [agregar el repositorio](#set-release).</span><span class="sxs-lookup"><span data-stu-id="1cb20-129">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="1cb20-130">Para las distribuciones de Ubuntu, use el repositorio `bionic` y, para las distribuciones de Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="1cb20-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="1cb20-131">Las distribuciones lanzadas antes de Ubuntu Trusty y Debian Wheezy no se admiten.</span><span class="sxs-lookup"><span data-stu-id="1cb20-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="1cb20-132">Actualizar</span><span class="sxs-lookup"><span data-stu-id="1cb20-132">Update</span></span>

<span data-ttu-id="1cb20-133">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="1cb20-133">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="1cb20-134">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="1cb20-134">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="1cb20-135">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="1cb20-135">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="1cb20-136">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="1cb20-136">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="1cb20-137">Desinstale con `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="1cb20-137">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="1cb20-138">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="1cb20-138">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="1cb20-139">Quite la clave de firma:</span><span class="sxs-lookup"><span data-stu-id="1cb20-139">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="1cb20-140">Quite los paquetes que no necesite:</span><span class="sxs-lookup"><span data-stu-id="1cb20-140">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="1cb20-141">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="1cb20-141">Next Steps</span></span>

<span data-ttu-id="1cb20-142">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="1cb20-142">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1cb20-143">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="1cb20-143">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
