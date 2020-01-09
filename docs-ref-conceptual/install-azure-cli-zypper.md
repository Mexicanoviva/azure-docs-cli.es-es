---
title: Instalación de la CLI de Azure en Linux con zypper
description: Cómo instalar la CLI de Azure con zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7e5897fe545527aa2708432e0ad0cf626584c785
ms.sourcegitcommit: 0088160bdb1ea520724d3e1efe71a4a66f29753d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/19/2019
ms.locfileid: "75216892"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="6f3a9-103">Instalación de la CLI de Azure con zypper</span><span class="sxs-lookup"><span data-stu-id="6f3a9-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="6f3a9-104">Para las distribuciones de Linux con `zypper`, como openSUSE o SLES, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="6f3a9-105">Este paquete se ha probado con openSUSE Leap 15.1 y SLES 15.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="6f3a9-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="6f3a9-106">Install</span></span>

1. <span data-ttu-id="6f3a9-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="6f3a9-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="6f3a9-108">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="6f3a9-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="6f3a9-109">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="6f3a9-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="6f3a9-110">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="6f3a9-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="6f3a9-111">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6f3a9-112">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="6f3a9-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6f3a9-113">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6f3a9-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6f3a9-114">Solución de problemas</span><span class="sxs-lookup"><span data-stu-id="6f3a9-114">Troubleshooting</span></span>

<span data-ttu-id="6f3a9-115">Estos son algunos problemas comunes que se han observado cuando se instala con `zypper`.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="6f3a9-116">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6f3a9-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-sles-12-or-other-other-systems-without-python-36"></a><span data-ttu-id="6f3a9-117">Instalación en SLES 12 u otros sistemas sin Python 3.6</span><span class="sxs-lookup"><span data-stu-id="6f3a9-117">Install on SLES 12 or other other systems without Python 3.6</span></span>

<span data-ttu-id="6f3a9-118">En SLES 12, el paquete predeterminado de python3 es 3.4 y no es compatible con la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-118">On SLES 12, the defualt python3 package is 3.4 and not supported by Azure CLI.</span></span> <span data-ttu-id="6f3a9-119">Puede compilar primero una versión superior de python3 a partir del código fuente.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-119">You can first build a higher version python3 from source.</span></span> <span data-ttu-id="6f3a9-120">Después, puede descargar el paquete de la CLI de Azure e instalarlo sin dependencias.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-120">Then you can download the Azure CLI package and install it without dependency.</span></span>
```bash
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
$ $PYTHON_SRC_DIR/*/configure --with-ssl
$ make
$ sudo make install
#Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
#Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="6f3a9-121">El servidor proxy bloquea la conexión</span><span class="sxs-lookup"><span data-stu-id="6f3a9-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="6f3a9-122">También puede configurar explícitamente `zypper` (mediante `yast2`) para usar este servidor proxy en todo momento.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-122">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="6f3a9-123">Para ello, ejecute el comando `yast2 proxy` como superusuario y rellene la información del formulario.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-123">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="6f3a9-124">Si tiene un administrador de ventanas disponible en el sistema, también puede usar el panel `Network Services > Proxy` en `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-124">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="6f3a9-125">Para ver la configuración avanzada o más información, consulte la [documentación de la configuración del servidor proxy de OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).</span><span class="sxs-lookup"><span data-stu-id="6f3a9-125">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="6f3a9-126">Para obtener la clave de firma de Microsoft y obtener el paquete de nuestro repositorio, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:</span><span class="sxs-lookup"><span data-stu-id="6f3a9-126">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="6f3a9-127">Actualizar</span><span class="sxs-lookup"><span data-stu-id="6f3a9-127">Update</span></span>

<span data-ttu-id="6f3a9-128">Puede actualizar el paquete con el comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-128">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="6f3a9-129">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="6f3a9-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="6f3a9-130">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-130">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="6f3a9-131">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-131">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="6f3a9-132">Si no usa otros paquetes de Microsoft, quite la clave de firma de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-132">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="6f3a9-133">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="6f3a9-133">Next Steps</span></span>

<span data-ttu-id="6f3a9-134">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="6f3a9-134">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6f3a9-135">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="6f3a9-135">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
