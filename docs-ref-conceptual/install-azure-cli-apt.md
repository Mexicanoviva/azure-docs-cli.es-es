---
title: Instalación de la CLI de Azure en Linux con apt
description: Instalación de la CLI de Azure con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 45e1e7468e5817d0138c9b87da83c5a5228e4965
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421939"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="d85db-103">Instalación de la CLI de Azure con apt</span><span class="sxs-lookup"><span data-stu-id="d85db-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="d85db-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="d85db-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="d85db-105">Este paquete se ha probado con:</span><span class="sxs-lookup"><span data-stu-id="d85db-105">This package has been tested with:</span></span>

* <span data-ttu-id="d85db-106">Ubuntu trusty, xenial, artful y bionic</span><span class="sxs-lookup"><span data-stu-id="d85db-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="d85db-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="d85db-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="d85db-108">El paquete `.deb` para la CLI de Azure instala su propio intérprete de Python y no utiliza el entorno de Python del sistema, por lo que se necesita explícitamente una versión local de Python.</span><span class="sxs-lookup"><span data-stu-id="d85db-108">The `.deb` package for Azure CLI installs its own Python interpreter, and does not use the system Python, so there is no explicit requirement for a local Python version.</span></span>

## <a name="install"></a><span data-ttu-id="d85db-109">Instalación</span><span class="sxs-lookup"><span data-stu-id="d85db-109">Install</span></span>

1. <span data-ttu-id="d85db-110">Instale los paquetes de requisitos previos:</span><span class="sxs-lookup"><span data-stu-id="d85db-110">Install prerequisite packages:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/><span data-ttu-id="d85db-111">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="d85db-111">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/><span data-ttu-id="d85db-112">Obtenga la clave de firma de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="d85db-112">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. <span data-ttu-id="d85db-113">Instale la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="d85db-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="d85db-114">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="d85db-114">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="d85db-115">Si recibe errores de firmas, asegúrese de tener [la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="d85db-115">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="d85db-116">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="d85db-116">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="d85db-117">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="d85db-117">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d85db-118">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d85db-118">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d85db-119">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="d85db-119">Troubleshooting</span></span>

<span data-ttu-id="d85db-120">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="d85db-120">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="d85db-121">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="d85db-121">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="d85db-122">lsb_release no devuelve la versión de distribución de base correcta</span><span class="sxs-lookup"><span data-stu-id="d85db-122">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="d85db-123">Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="d85db-123">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="d85db-124">Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar.</span><span class="sxs-lookup"><span data-stu-id="d85db-124">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="d85db-125">Si conoce el nombre de la versión de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente en el [paso 2 de la instalación](#set-release).</span><span class="sxs-lookup"><span data-stu-id="d85db-125">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 2](#set-release).</span></span> <span data-ttu-id="d85db-126">En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre de la distribución base y establezca `AZ_REPO` en el valor correcto.</span><span class="sxs-lookup"><span data-stu-id="d85db-126">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="d85db-127">No hay ningún paquete para su distribución</span><span class="sxs-lookup"><span data-stu-id="d85db-127">No package for your distribution</span></span>

<span data-ttu-id="d85db-128">A veces hace falta un tiempo desde el lanzamiento de una distribución Ubuntu para que haya un paquete de la CLI de Azure disponible.</span><span class="sxs-lookup"><span data-stu-id="d85db-128">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="d85db-129">La CLI de Azure se ha diseñado para ser resistente con respecto a versiones futuras de las dependencias, y a usar las menos posibles.</span><span class="sxs-lookup"><span data-stu-id="d85db-129">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="d85db-130">Si no hay ningún paquete disponible para su distribución de base, pruebe un paquete de una distribución anterior.</span><span class="sxs-lookup"><span data-stu-id="d85db-130">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="d85db-131">Para ello, establezca el valor de `AZ_REPO` manualmente en [install step 1](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="d85db-131">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="d85db-132">Para las distribuciones de Ubuntu, use el repositorio `bionic` y, para las distribuciones de Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="d85db-132">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="d85db-133">Las distribuciones lanzadas antes de Ubuntu Trusty y Debian Wheezy no se admiten.</span><span class="sxs-lookup"><span data-stu-id="d85db-133">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="d85db-134">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="d85db-134">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="d85db-135">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="d85db-135">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="d85db-136">El error es debido a que falta un componente que `apt-key` necesita.</span><span class="sxs-lookup"><span data-stu-id="d85db-136">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="d85db-137">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="d85db-137">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

<span data-ttu-id="d85db-138">Si está en el subsistema de Windows para Linux (WSL), este error también aparece en las versiones de Windows anteriores a Windows 10 1809.</span><span class="sxs-lookup"><span data-stu-id="d85db-138">If you are on Windows Subsystem for Linux (WSL), this error also appears on versions of Windows prior to Windows 10 1809.</span></span> <span data-ttu-id="d85db-139">Para resolver el problema, actualice su versión de Windows.</span><span class="sxs-lookup"><span data-stu-id="d85db-139">To resolve the issue, update your version of Windows.</span></span>

### <a name="apt-key-hangs"></a><span data-ttu-id="d85db-140">bloqueos de apt-key</span><span class="sxs-lookup"><span data-stu-id="d85db-140">apt-key hangs</span></span>

<span data-ttu-id="d85db-141">Si está detrás de un firewall que bloquea las conexiones salientes al puerto 11371, el comando `apt-key` podría producir errores indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="d85db-141">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="d85db-142">El firewall puede requerir un servidor proxy HTTP para las conexiones salientes:</span><span class="sxs-lookup"><span data-stu-id="d85db-142">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="d85db-143">Para determinar si tiene un servidor proxy, póngase en contacto con el administrador del sistema.</span><span class="sxs-lookup"><span data-stu-id="d85db-143">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="d85db-144">Si el proxy no requiere un inicio de sesión, no indique el usuario ni la contraseña.</span><span class="sxs-lookup"><span data-stu-id="d85db-144">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="d85db-145">Actualizar</span><span class="sxs-lookup"><span data-stu-id="d85db-145">Update</span></span>

<span data-ttu-id="d85db-146">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="d85db-146">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="d85db-147">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="d85db-147">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="d85db-148">Si recibe errores de firmas, asegúrese de tener [la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="d85db-148">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="d85db-149">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="d85db-149">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="d85db-150">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="d85db-150">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="d85db-151">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="d85db-151">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="d85db-152">Desinstale con `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="d85db-152">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="d85db-153">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="d85db-153">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="d85db-154">Quite la clave de firma:</span><span class="sxs-lookup"><span data-stu-id="d85db-154">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="d85db-155">Quite los paquetes que no necesite:</span><span class="sxs-lookup"><span data-stu-id="d85db-155">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="d85db-156">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d85db-156">Next Steps</span></span>

<span data-ttu-id="d85db-157">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="d85db-157">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d85db-158">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="d85db-158">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
