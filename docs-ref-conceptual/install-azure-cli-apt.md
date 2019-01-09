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
ms.openlocfilehash: 1973c933cbffa494cbe9c0749346450251feefcb
ms.sourcegitcommit: 9bd90875a324908ec7195fc4c4f63ebf124760f9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982593"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="e6b07-103">Instalación de la CLI de Azure con apt</span><span class="sxs-lookup"><span data-stu-id="e6b07-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="e6b07-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="e6b07-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="e6b07-105">Este paquete se ha probado con:</span><span class="sxs-lookup"><span data-stu-id="e6b07-105">This package has been tested with:</span></span>

* <span data-ttu-id="e6b07-106">Ubuntu trusty, xenial, artful y bionic</span><span class="sxs-lookup"><span data-stu-id="e6b07-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="e6b07-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="e6b07-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="e6b07-108">Instalación</span><span class="sxs-lookup"><span data-stu-id="e6b07-108">Install</span></span>

1. <span data-ttu-id="e6b07-109">Instale los paquetes de requisitos previos:</span><span class="sxs-lookup"><span data-stu-id="e6b07-109">Install prerequisite packages:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/><span data-ttu-id="e6b07-110">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="e6b07-110">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/><span data-ttu-id="e6b07-111">Obtenga la clave de firma de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="e6b07-111">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. <span data-ttu-id="e6b07-112">Instale la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="e6b07-112">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="e6b07-113">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="e6b07-113">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="e6b07-114">Si recibe errores de firmas, asegúrese de tener [la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="e6b07-114">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="e6b07-115">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="e6b07-115">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="e6b07-116">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="e6b07-116">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="e6b07-117">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e6b07-117">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e6b07-118">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="e6b07-118">Troubleshooting</span></span>

<span data-ttu-id="e6b07-119">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="e6b07-119">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="e6b07-120">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e6b07-120">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="e6b07-121">lsb_release no devuelve la versión de distribución de base correcta</span><span class="sxs-lookup"><span data-stu-id="e6b07-121">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="e6b07-122">Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="e6b07-122">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="e6b07-123">Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar.</span><span class="sxs-lookup"><span data-stu-id="e6b07-123">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="e6b07-124">Si conoce el nombre de la versión de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente en el [paso 2 de la instalación](#set-release).</span><span class="sxs-lookup"><span data-stu-id="e6b07-124">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 2](#set-release).</span></span> <span data-ttu-id="e6b07-125">En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre de la distribución base y establezca `AZ_REPO` en el valor correcto.</span><span class="sxs-lookup"><span data-stu-id="e6b07-125">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="e6b07-126">No hay ningún paquete para su distribución</span><span class="sxs-lookup"><span data-stu-id="e6b07-126">No package for your distribution</span></span>

<span data-ttu-id="e6b07-127">A veces hace falta un tiempo desde el lanzamiento de una distribución Ubuntu para que haya un paquete de la CLI de Azure disponible.</span><span class="sxs-lookup"><span data-stu-id="e6b07-127">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="e6b07-128">La CLI de Azure se ha diseñado para ser resistente con respecto a versiones futuras de las dependencias, y a usar las menos posibles.</span><span class="sxs-lookup"><span data-stu-id="e6b07-128">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="e6b07-129">Si no hay ningún paquete disponible para su distribución de base, pruebe un paquete de una distribución anterior.</span><span class="sxs-lookup"><span data-stu-id="e6b07-129">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="e6b07-130">Para ello, establezca el valor de `AZ_REPO` manualmente en [install step 1](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="e6b07-130">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="e6b07-131">Para las distribuciones de Ubuntu, use el repositorio `bionic` y, para las distribuciones de Debian, use `stretch`.</span><span class="sxs-lookup"><span data-stu-id="e6b07-131">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="e6b07-132">Las distribuciones lanzadas antes de Ubuntu Trusty y Debian Wheezy no se admiten.</span><span class="sxs-lookup"><span data-stu-id="e6b07-132">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="e6b07-133">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="e6b07-133">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="e6b07-134">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="e6b07-134">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="e6b07-135">El error es debido a que falta un componente que `apt-key` necesita.</span><span class="sxs-lookup"><span data-stu-id="e6b07-135">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="e6b07-136">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="e6b07-136">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

<span data-ttu-id="e6b07-137">Si está en el subsistema de Windows para Linux (WSL), este error también aparece en las versiones de Windows anteriores a Windows 10 1809.</span><span class="sxs-lookup"><span data-stu-id="e6b07-137">If you are on Windows Subsystem for Linux (WSL), this error also appears on versions of Windows prior to Windows 10 1809.</span></span> <span data-ttu-id="e6b07-138">Para resolver el problema, actualice su versión de Windows.</span><span class="sxs-lookup"><span data-stu-id="e6b07-138">To resolve the issue, update your version of Windows.</span></span>

### <a name="apt-key-hangs"></a><span data-ttu-id="e6b07-139">bloqueos de apt-key</span><span class="sxs-lookup"><span data-stu-id="e6b07-139">apt-key hangs</span></span>

<span data-ttu-id="e6b07-140">Si está detrás de un firewall que bloquea las conexiones salientes al puerto 11371, el comando `apt-key` podría producir errores indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="e6b07-140">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="e6b07-141">El firewall puede requerir un servidor proxy HTTP para las conexiones salientes:</span><span class="sxs-lookup"><span data-stu-id="e6b07-141">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="e6b07-142">Para determinar si tiene un servidor proxy, póngase en contacto con el administrador del sistema.</span><span class="sxs-lookup"><span data-stu-id="e6b07-142">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="e6b07-143">Si el proxy no requiere un inicio de sesión, no indique el usuario ni la contraseña.</span><span class="sxs-lookup"><span data-stu-id="e6b07-143">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="e6b07-144">Actualizar</span><span class="sxs-lookup"><span data-stu-id="e6b07-144">Update</span></span>

<span data-ttu-id="e6b07-145">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="e6b07-145">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="e6b07-146">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="e6b07-146">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="e6b07-147">Si recibe errores de firmas, asegúrese de tener [la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="e6b07-147">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="e6b07-148">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="e6b07-148">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="e6b07-149">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="e6b07-149">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="e6b07-150">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="e6b07-150">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="e6b07-151">Desinstale con `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="e6b07-151">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="e6b07-152">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="e6b07-152">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="e6b07-153">Quite la clave de firma:</span><span class="sxs-lookup"><span data-stu-id="e6b07-153">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="e6b07-154">Quite los paquetes que no necesite:</span><span class="sxs-lookup"><span data-stu-id="e6b07-154">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="e6b07-155">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="e6b07-155">Next Steps</span></span>

<span data-ttu-id="e6b07-156">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="e6b07-156">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="e6b07-157">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="e6b07-157">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
