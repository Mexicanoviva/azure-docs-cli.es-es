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
ms.devlang: azure-cli
ms.openlocfilehash: a73576a9caeb7d016f49bb1d90f1903cbd515c63
ms.sourcegitcommit: 6d9169ed547df151f99e5a3ac86578634486419a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/23/2018
ms.locfileid: "49652454"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="2434b-103">Instalación de la CLI de Azure con zypper</span><span class="sxs-lookup"><span data-stu-id="2434b-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="2434b-104">Para las distribuciones de Linux con `zypper`, como openSUSE o SLES, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="2434b-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="2434b-105">Este paquete se ha probado con openSUSE 42.2 y SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="2434b-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="2434b-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="2434b-106">Install</span></span>

1. <span data-ttu-id="2434b-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="2434b-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="2434b-108">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="2434b-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="2434b-109">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="2434b-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="2434b-110">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="2434b-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="2434b-111">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="2434b-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="2434b-112">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="2434b-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="2434b-113">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2434b-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="2434b-114">Actualizar</span><span class="sxs-lookup"><span data-stu-id="2434b-114">Update</span></span>

<span data-ttu-id="2434b-115">Puede actualizar el paquete con el comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="2434b-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="2434b-116">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="2434b-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="2434b-117">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="2434b-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="2434b-118">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="2434b-118">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="2434b-119">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2434b-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
   ## <a name="next-steps"></a><span data-ttu-id="2434b-120">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="2434b-120">Next Steps</span></span>

<span data-ttu-id="2434b-121">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="2434b-121">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="2434b-122">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="2434b-122">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
