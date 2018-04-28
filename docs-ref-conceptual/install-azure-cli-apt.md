---
title: Instalación de la CLI de Azure 2.0 en Linux con apt
description: Instalación de la CLI de Azure 2.0 con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/06/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 86d601fdc375ec59c4f7cbf0881bc67a08e24b19
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="b030c-103">Instalación de la CLI de Azure 2.0 con apt</span><span class="sxs-lookup"><span data-stu-id="b030c-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="b030c-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="b030c-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="b030c-105">Este paquete se ha probado con:</span><span class="sxs-lookup"><span data-stu-id="b030c-105">This package has been tested with:</span></span>

* <span data-ttu-id="b030c-106">Ubuntu trusty, xenial y artful</span><span class="sxs-lookup"><span data-stu-id="b030c-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="b030c-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="b030c-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="b030c-108">Instalación</span><span class="sxs-lookup"><span data-stu-id="b030c-108">Install</span></span>

1. <span data-ttu-id="b030c-109">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="b030c-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="b030c-110">Obtenga la clave de firma de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="b030c-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > <span data-ttu-id="b030c-111">Esta clave de firma está en desuso y se reemplazará a finales de mayo de 2018.</span><span class="sxs-lookup"><span data-stu-id="b030c-111">This signing key is deprecated, and will be replaced at the end of May 2018.</span></span> <span data-ttu-id="b030c-112">Para seguir recibiendo actualizaciones con `apt`, asegúrese de instalar también la nueva clave:</span><span class="sxs-lookup"><span data-stu-id="b030c-112">In order to keep getting updates with `apt`, make sure that you also install the new key:</span></span>
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. <span data-ttu-id="b030c-113">Instale la CLI de Azure:</span><span class="sxs-lookup"><span data-stu-id="b030c-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="b030c-114">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="b030c-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="b030c-115">Para iniciar sesión, ejecute el comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="b030c-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="b030c-116">Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b030c-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="b030c-117">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="b030c-117">Troubleshooting</span></span>

<span data-ttu-id="b030c-118">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="b030c-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="b030c-119">Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="b030c-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="b030c-120">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="b030c-120">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="b030c-121">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="b030c-121">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="b030c-122">El error es debido a que falta un componente que `apt-key` necesita.</span><span class="sxs-lookup"><span data-stu-id="b030c-122">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="b030c-123">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="b030c-123">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="b030c-124">bloqueos de apt-key</span><span class="sxs-lookup"><span data-stu-id="b030c-124">apt-key hangs</span></span>

<span data-ttu-id="b030c-125">Si está detrás de un firewall que bloquea las conexiones salientes al puerto 11371, el comando `apt-key` podría producir errores indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="b030c-125">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="b030c-126">El firewall puede requerir el uso de un servidor proxy HTTP para las conexiones salientes:</span><span class="sxs-lookup"><span data-stu-id="b030c-126">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="b030c-127">Si no sabe si tiene un servidor proxy, póngase en contacto con el administrador del sistema.</span><span class="sxs-lookup"><span data-stu-id="b030c-127">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="b030c-128">Si el proxy no requiere un inicio de sesión, omita el usuario, la contraseña y el token `@`.</span><span class="sxs-lookup"><span data-stu-id="b030c-128">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="b030c-129">Actualizar</span><span class="sxs-lookup"><span data-stu-id="b030c-129">Update</span></span>

<span data-ttu-id="b030c-130">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="b030c-130">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="b030c-131">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="b030c-131">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="b030c-132">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="b030c-132">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="b030c-133">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="b030c-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="b030c-134">Desinstale con `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="b030c-134">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="b030c-135">Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="b030c-135">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="b030c-136">Quite los paquetes que no necesite.</span><span class="sxs-lookup"><span data-stu-id="b030c-136">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
