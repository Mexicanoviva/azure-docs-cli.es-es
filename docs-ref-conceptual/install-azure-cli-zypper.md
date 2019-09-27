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
ms.openlocfilehash: 84946fc0562e396ef296cbe8dede5e6a65cd6614
ms.sourcegitcommit: 5a29ce9c0a3d7b831f22b1a13b1ae2e239e5549f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/19/2019
ms.locfileid: "71143961"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="58be2-103">Instalación de la CLI de Azure con zypper</span><span class="sxs-lookup"><span data-stu-id="58be2-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="58be2-104">Para las distribuciones de Linux con `zypper`, como openSUSE o SLES, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="58be2-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="58be2-105">Este paquete se ha probado con openSUSE 42.2 y versiones posteriores, y SLES 12 SP 2 y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="58be2-105">This package has been tested with openSUSE 42.2 and later, and SLES 12 SP 2 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="58be2-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="58be2-106">Install</span></span>

1. <span data-ttu-id="58be2-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="58be2-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="58be2-108">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="58be2-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="58be2-109">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="58be2-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="58be2-110">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="58be2-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="58be2-111">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="58be2-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="58be2-112">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="58be2-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="58be2-113">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="58be2-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="58be2-114">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="58be2-114">Troubleshooting</span></span>

<span data-ttu-id="58be2-115">Estos son algunos problemas comunes que se han observado cuando se instala con `zypper`.</span><span class="sxs-lookup"><span data-stu-id="58be2-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="58be2-116">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="58be2-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="58be2-117">Conexión de bloques proxy</span><span class="sxs-lookup"><span data-stu-id="58be2-117">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="58be2-118">También puede configurar explícitamente `zypper` (mediante `yast2`) para usar este servidor proxy en todo momento.</span><span class="sxs-lookup"><span data-stu-id="58be2-118">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="58be2-119">Para ello, ejecute el comando `yast2 proxy` como superusuario y rellene la información del formulario.</span><span class="sxs-lookup"><span data-stu-id="58be2-119">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="58be2-120">Si tiene un administrador de ventanas disponible en el sistema, también puede usar el panel `Network Services > Proxy` en `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="58be2-120">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="58be2-121">Para ver la configuración avanzada o más información, consulte la [documentación de la configuración del servidor proxy de OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).</span><span class="sxs-lookup"><span data-stu-id="58be2-121">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="58be2-122">Para obtener la clave de firma de Microsoft y obtener el paquete de nuestro repositorio, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:</span><span class="sxs-lookup"><span data-stu-id="58be2-122">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="58be2-123">Actualizar</span><span class="sxs-lookup"><span data-stu-id="58be2-123">Update</span></span>

<span data-ttu-id="58be2-124">Puede actualizar el paquete con el comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="58be2-124">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="58be2-125">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="58be2-125">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="58be2-126">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="58be2-126">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="58be2-127">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="58be2-127">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="58be2-128">Si no usa otros paquetes de Microsoft, quite la clave de firma de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="58be2-128">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="58be2-129">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="58be2-129">Next Steps</span></span>

<span data-ttu-id="58be2-130">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="58be2-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="58be2-131">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="58be2-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
