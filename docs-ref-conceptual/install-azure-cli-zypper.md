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
ms.openlocfilehash: 4cdbeaffb00e87b590080c1d341ec9e7ee198410
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593530"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="97a8a-103">Instalación de la CLI de Azure con zypper</span><span class="sxs-lookup"><span data-stu-id="97a8a-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="97a8a-104">Para las distribuciones de Linux con `zypper`, como openSUSE o SLES, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="97a8a-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="97a8a-105">Este paquete se ha probado con openSUSE 42.2 y SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="97a8a-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="97a8a-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="97a8a-106">Install</span></span>

1. <span data-ttu-id="97a8a-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="97a8a-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="97a8a-108">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="97a8a-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="97a8a-109">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="97a8a-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="97a8a-110">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="97a8a-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="97a8a-111">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="97a8a-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="97a8a-112">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="97a8a-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="97a8a-113">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="97a8a-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="97a8a-114">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="97a8a-114">Troubleshooting</span></span>

<span data-ttu-id="97a8a-115">Estos son algunos problemas comunes que se han observado cuando se instala con `zypper`.</span><span class="sxs-lookup"><span data-stu-id="97a8a-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="97a8a-116">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="97a8a-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]


## <a name="update"></a><span data-ttu-id="97a8a-117">Actualizar</span><span class="sxs-lookup"><span data-stu-id="97a8a-117">Update</span></span>

<span data-ttu-id="97a8a-118">Puede actualizar el paquete con el comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="97a8a-118">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="97a8a-119">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="97a8a-119">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="97a8a-120">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="97a8a-120">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="97a8a-121">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="97a8a-121">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="97a8a-122">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="97a8a-122">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
   ## <a name="next-steps"></a><span data-ttu-id="97a8a-123">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="97a8a-123">Next Steps</span></span>

<span data-ttu-id="97a8a-124">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="97a8a-124">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="97a8a-125">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="97a8a-125">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
