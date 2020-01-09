---
title: Instalación de la CLI de Azure en Linux con yum
description: Cómo instalar la CLI de Azure con yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f65240524942c2534f61b9cc51101812c8d09351
ms.sourcegitcommit: 0088160bdb1ea520724d3e1efe71a4a66f29753d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/19/2019
ms.locfileid: "75216929"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="aeef2-103">Instalación de la CLI de Azure con yum</span><span class="sxs-lookup"><span data-stu-id="aeef2-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="aeef2-104">Para distribuciones Linux con `yum`, como RHEL, Fedora o CentOS, hay un paquete de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="aeef2-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="aeef2-105">Este paquete se ha probado con RHEL 7.7, RHEL 8, Fedora 24 y versiones posteriores, CentOS 7 y CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="aeef2-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="aeef2-106">Instalar</span><span class="sxs-lookup"><span data-stu-id="aeef2-106">Install</span></span>

1. <span data-ttu-id="aeef2-107">Importe la clave del repositorio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="aeef2-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="aeef2-108">Cree la información del repositorio `azure-cli` local.</span><span class="sxs-lookup"><span data-stu-id="aeef2-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="aeef2-109">Realice la instalación con el comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="aeef2-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="aeef2-110">Ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="aeef2-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="aeef2-111">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="aeef2-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="aeef2-112">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="aeef2-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="aeef2-113">Solución de problemas</span><span class="sxs-lookup"><span data-stu-id="aeef2-113">Troubleshooting</span></span>

<span data-ttu-id="aeef2-114">Estos son algunos problemas comunes que se han observado cuando se instala con `yum`.</span><span class="sxs-lookup"><span data-stu-id="aeef2-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="aeef2-115">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="aeef2-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="aeef2-116">Instalación en RHEL 7.6 u otros sistemas sin Python 3</span><span class="sxs-lookup"><span data-stu-id="aeef2-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="aeef2-117">Si es posible, actualice el sistema a una versión con soporte técnico oficial para el paquete `python3`.</span><span class="sxs-lookup"><span data-stu-id="aeef2-117">If you can, please upgrade your system to a verison with official support for `python3` package.</span></span> <span data-ttu-id="aeef2-118">En caso contrario, debe instalar primero un paquete de `python3`, ya sea una [compilación desde el código fuente](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) o una instalación mediante un [repositorio adicional](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="aeef2-118">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="aeef2-119">Después, puede descargar el paquete e instalarlo sin dependencias.</span><span class="sxs-lookup"><span data-stu-id="aeef2-119">Then you can download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="aeef2-120">La opción menos recomendada es continuar con el uso de Python 2 y seguir las [instrucciones de instalación manual](install-azure-cli-linux.md), puesto que Python 2 termina su ciclo de vida el 1 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="aeef2-120">The least recommended option is to still use Python 2 and follow the [manual install instructions](install-azure-cli-linux.md) since Python 2 is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="aeef2-121">Una versión futura de la CLI de Azure eliminará la compatibilidad con Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="aeef2-121">A future version of Azure CLI will drop support for Python 2.7.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="aeef2-122">El servidor proxy bloquea la conexión</span><span class="sxs-lookup"><span data-stu-id="aeef2-122">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="aeef2-123">También puede configurar explícitamente `yum` para usar este servidor proxy en todo momento.</span><span class="sxs-lookup"><span data-stu-id="aeef2-123">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="aeef2-124">Asegúrese de que las líneas siguientes aparecen en la sección `[main]` de `/etc/yum.conf`:</span><span class="sxs-lookup"><span data-stu-id="aeef2-124">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="aeef2-125">Para obtener la clave de firma de Microsoft y obtener el paquete de nuestro repositorio, el servidor proxy debe permitir las conexiones HTTPS a la siguiente dirección:</span><span class="sxs-lookup"><span data-stu-id="aeef2-125">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="aeef2-126">Actualizar</span><span class="sxs-lookup"><span data-stu-id="aeef2-126">Update</span></span>

<span data-ttu-id="aeef2-127">Actualice la CLI de Azure con el comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="aeef2-127">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="aeef2-128">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="aeef2-128">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="aeef2-129">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="aeef2-129">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="aeef2-130">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="aeef2-130">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="aeef2-131">Si no usa otros paquetes de Microsoft, quite la clave de firma.</span><span class="sxs-lookup"><span data-stu-id="aeef2-131">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="aeef2-132">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="aeef2-132">Next Steps</span></span>

<span data-ttu-id="aeef2-133">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="aeef2-133">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="aeef2-134">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="aeef2-134">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
