---
title: Instalación de la CLI de Azure 2.0 en Linux con apt
description: Instalación de la CLI de Azure 2.0 con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/24/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: abbffb1c474d752130dfffa8e60937b3d632fa14
ms.sourcegitcommit: c6c3058254974b3a1d5d2fa2cd231a900c53d321
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/29/2018
ms.locfileid: "37126589"
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="49b4d-103">Instalación de la CLI de Azure 2.0 con apt</span><span class="sxs-lookup"><span data-stu-id="49b4d-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="49b4d-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="49b4d-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="49b4d-105">Este paquete se ha probado con:</span><span class="sxs-lookup"><span data-stu-id="49b4d-105">This package has been tested with:</span></span>

* <span data-ttu-id="49b4d-106">Ubuntu trusty, xenial, artful y bionic</span><span class="sxs-lookup"><span data-stu-id="49b4d-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="49b4d-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="49b4d-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="49b4d-108">Instalación</span><span class="sxs-lookup"><span data-stu-id="49b4d-108">Install</span></span>

1. <span data-ttu-id="49b4d-109"><a name="install-step-1"/> Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="49b4d-109"><a name="install-step-1"/> Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <a name="signingKey"></a><span data-ttu-id="49b4d-110">Obtenga la clave de firma de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="49b4d-110">Get the Microsoft signing key:</span></span>

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. <span data-ttu-id="49b4d-111">Instale la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="49b4d-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="49b4d-112">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="49b4d-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="49b4d-113">Si recibe errores de clave de firma, asegúrese de que ha [adquirido la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="49b4d-113">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>

<span data-ttu-id="49b4d-114">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="49b4d-115">Para iniciar sesión, ejecute el comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="49b4d-116">Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="49b4d-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="49b4d-117">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="49b4d-117">Troubleshooting</span></span>

<span data-ttu-id="49b4d-118">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="49b4d-119">Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="49b4d-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="49b4d-120">Se produce un error en lsb_release con el mensaje "No se encontró el comando"</span><span class="sxs-lookup"><span data-stu-id="49b4d-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="49b4d-121">Cuando se ejecuta el comando `lsb_release`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="49b4d-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="49b4d-122">El error se debe a que lsb_release no está instalado.</span><span class="sxs-lookup"><span data-stu-id="49b4d-122">The error is due to lsb_release not being installed.</span></span> <span data-ttu-id="49b4d-123">Puede resolver este problema mediante la instalación del paquete `lsb-release`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="49b4d-124">lsb_release no devuelve la versión de distribución de base</span><span class="sxs-lookup"><span data-stu-id="49b4d-124">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="49b4d-125">Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-125">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="49b4d-126">Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar.</span><span class="sxs-lookup"><span data-stu-id="49b4d-126">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="49b4d-127">Si conoce el nombre de la versión de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente en el [paso 1 de la instalación](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="49b4d-127">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="49b4d-128">En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre de la distribución base y establezca `AZ_REPO` en el valor correcto.</span><span class="sxs-lookup"><span data-stu-id="49b4d-128">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="49b4d-129">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="49b4d-129">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="49b4d-130">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="49b4d-130">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="49b4d-131">El error es debido a que falta un componente que `apt-key` necesita.</span><span class="sxs-lookup"><span data-stu-id="49b4d-131">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="49b4d-132">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-132">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="49b4d-133">bloqueos de apt-key</span><span class="sxs-lookup"><span data-stu-id="49b4d-133">apt-key hangs</span></span>

<span data-ttu-id="49b4d-134">Si está detrás de un firewall que bloquea las conexiones salientes al puerto 11371, el comando `apt-key` podría producir errores indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="49b4d-134">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="49b4d-135">El firewall puede requerir el uso de un servidor proxy HTTP para las conexiones salientes:</span><span class="sxs-lookup"><span data-stu-id="49b4d-135">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="49b4d-136">Si no sabe si tiene un servidor proxy, póngase en contacto con el administrador del sistema.</span><span class="sxs-lookup"><span data-stu-id="49b4d-136">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="49b4d-137">Si el proxy no requiere un inicio de sesión, omita el usuario, la contraseña y el token `@`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-137">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="49b4d-138">Actualizar</span><span class="sxs-lookup"><span data-stu-id="49b4d-138">Update</span></span>

<span data-ttu-id="49b4d-139">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-139">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="49b4d-140">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="49b4d-140">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="49b4d-141">Si recibe errores de clave de firma, asegúrese de que ha [adquirido la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="49b4d-141">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>
   
> [!NOTE]
> <span data-ttu-id="49b4d-142">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="49b4d-142">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="49b4d-143">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-143">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="49b4d-144">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="49b4d-144">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="49b4d-145">Desinstale con `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="49b4d-145">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="49b4d-146">Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="49b4d-146">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="49b4d-147">Quite los paquetes que no necesite.</span><span class="sxs-lookup"><span data-stu-id="49b4d-147">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
