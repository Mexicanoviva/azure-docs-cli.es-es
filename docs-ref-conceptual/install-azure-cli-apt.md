---
title: Instalación de la CLI de Azure en Linux con apt
description: Instalación de la CLI de Azure con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0d4311e88fec9903c1aab1410cc71328f896dc65
ms.sourcegitcommit: 728a050f13d3682122be4a8993596cc4185a45ce
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/15/2018
ms.locfileid: "51680941"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="09c27-103">Instalación de la CLI de Azure con apt</span><span class="sxs-lookup"><span data-stu-id="09c27-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="09c27-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="09c27-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="09c27-105">Este paquete se ha probado con:</span><span class="sxs-lookup"><span data-stu-id="09c27-105">This package has been tested with:</span></span>

* <span data-ttu-id="09c27-106">Ubuntu trusty, xenial, artful y bionic</span><span class="sxs-lookup"><span data-stu-id="09c27-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="09c27-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="09c27-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="09c27-108">Instalación</span><span class="sxs-lookup"><span data-stu-id="09c27-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="09c27-109">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="09c27-109">Modify your sources list:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="09c27-110">Obtenga la clave de firma de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="09c27-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. <span data-ttu-id="09c27-111">Instale la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="09c27-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="09c27-112">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="09c27-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="09c27-113">Si recibe errores de firmas, asegúrese de tener [la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="09c27-113">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="09c27-114">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="09c27-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="09c27-115">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="09c27-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="09c27-116">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="09c27-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="09c27-117">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="09c27-117">Troubleshooting</span></span>

<span data-ttu-id="09c27-118">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="09c27-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="09c27-119">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="09c27-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="09c27-120">lsb_release no devuelve la versión de distribución de base</span><span class="sxs-lookup"><span data-stu-id="09c27-120">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="09c27-121">Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="09c27-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="09c27-122">Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar.</span><span class="sxs-lookup"><span data-stu-id="09c27-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="09c27-123">Si conoce el nombre de la versión de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente en el [paso 1 de la instalación](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="09c27-123">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="09c27-124">En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre de la distribución base y establezca `AZ_REPO` en el valor correcto.</span><span class="sxs-lookup"><span data-stu-id="09c27-124">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="09c27-125">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="09c27-125">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="09c27-126">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="09c27-126">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="09c27-127">El error es debido a que falta un componente que `apt-key` necesita.</span><span class="sxs-lookup"><span data-stu-id="09c27-127">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="09c27-128">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="09c27-128">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="09c27-129">bloqueos de apt-key</span><span class="sxs-lookup"><span data-stu-id="09c27-129">apt-key hangs</span></span>

<span data-ttu-id="09c27-130">Si está detrás de un firewall que bloquea las conexiones salientes al puerto 11371, el comando `apt-key` podría producir errores indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="09c27-130">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="09c27-131">El firewall puede requerir un servidor proxy HTTP para las conexiones salientes:</span><span class="sxs-lookup"><span data-stu-id="09c27-131">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="09c27-132">Para determinar si tiene un servidor proxy, póngase en contacto con el administrador del sistema.</span><span class="sxs-lookup"><span data-stu-id="09c27-132">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="09c27-133">Si el proxy no requiere un inicio de sesión, no indique el usuario ni la contraseña.</span><span class="sxs-lookup"><span data-stu-id="09c27-133">If your proxy does not require a login, then leave out the user and password information.</span></span>

## <a name="update"></a><span data-ttu-id="09c27-134">Actualizar</span><span class="sxs-lookup"><span data-stu-id="09c27-134">Update</span></span>

<span data-ttu-id="09c27-135">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="09c27-135">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="09c27-136">La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada.</span><span class="sxs-lookup"><span data-stu-id="09c27-136">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="09c27-137">Si recibe errores de firmas, asegúrese de tener [la clave de firma más reciente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="09c27-137">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="09c27-138">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="09c27-138">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="09c27-139">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="09c27-139">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="09c27-140">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="09c27-140">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="09c27-141">Desinstale con `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="09c27-141">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="09c27-142">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="09c27-142">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="09c27-143">Quite la clave de firma:</span><span class="sxs-lookup"><span data-stu-id="09c27-143">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="09c27-144">Quite los paquetes que no necesite:</span><span class="sxs-lookup"><span data-stu-id="09c27-144">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="09c27-145">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="09c27-145">Next Steps</span></span>

<span data-ttu-id="09c27-146">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="09c27-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="09c27-147">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="09c27-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)