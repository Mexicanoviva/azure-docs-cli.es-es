---
title: Instalación de la CLI de Azure 2.0 en Linux con zypper
description: Instalación de la CLI de Azure 2.0 con zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: dde90e78f3ec53d323ca78c816ceefb8cf65608b
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2018
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="c2756-103">Instalación de la CLI de Azure 2.0 con zypper</span><span class="sxs-lookup"><span data-stu-id="c2756-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="c2756-104">Si está ejecutando una distribución que viene con `zypper`, como openSUSE o SLES, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="c2756-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="c2756-105">Este paquete se ha probado con openSUSE 42.2 y SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="c2756-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="c2756-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="c2756-106">Install</span></span>

1. <span data-ttu-id="c2756-107">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="c2756-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="c2756-108">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="c2756-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="c2756-109">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="c2756-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="c2756-110">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="c2756-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="c2756-111">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="c2756-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="c2756-112">Para iniciar sesión, ejecute el comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="c2756-112">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="c2756-113">Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c2756-113">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="c2756-114">Actualizar</span><span class="sxs-lookup"><span data-stu-id="c2756-114">Update</span></span>

<span data-ttu-id="c2756-115">Puede actualizar el paquete con el comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="c2756-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="c2756-116">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="c2756-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="c2756-117">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="c2756-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="c2756-118">Si no piensa volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="c2756-118">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="c2756-119">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c2756-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

