---
title: "Instalación de la CLI de Azure 2.0 con zypper"
description: "Instalación de la CLI de Azure 2.0 con zypper"
keywords: "cli de azure, instalación de la cli de azure, azure cli zypper, azure cli opensuse, azure cli sle"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: c01679ccb77880f1f628f4e48683d8ff030a568b
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="cbec3-104">Instalación de la CLI de Azure 2.0 con zypper</span><span class="sxs-lookup"><span data-stu-id="cbec3-104">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="cbec3-105">Si está ejecutando una distribución que incluye `zypper`, como OpenSUSE o SLE, hay un paquete disponible para la CLI de Azure que se puede instalar en el sistema.</span><span class="sxs-lookup"><span data-stu-id="cbec3-105">If you are running a distirbution that comes with `zypper`, such as OpenSUSE or SLE, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="cbec3-106">Debe tener Python 2.7.x o Python 3.x para poder usar la CLI.</span><span class="sxs-lookup"><span data-stu-id="cbec3-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="cbec3-107">Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="cbec3-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="cbec3-108">Instalación</span><span class="sxs-lookup"><span data-stu-id="cbec3-108">Install</span></span> 

1. <span data-ttu-id="cbec3-109">Instale `curl`:</span><span class="sxs-lookup"><span data-stu-id="cbec3-109">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="cbec3-110">Importe la clave del repositorio de Microsoft:</span><span class="sxs-lookup"><span data-stu-id="cbec3-110">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="cbec3-111">Cree la información del repositorio `azure-cli` local:</span><span class="sxs-lookup"><span data-stu-id="cbec3-111">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="cbec3-112">Actualice el índice del paquete `zypper` e instálelo:</span><span class="sxs-lookup"><span data-stu-id="cbec3-112">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="cbec3-113">Puede ejecutar la CLI con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="cbec3-113">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="cbec3-114">Actualizar</span><span class="sxs-lookup"><span data-stu-id="cbec3-114">Update</span></span>

<span data-ttu-id="cbec3-115">Puede actualizar el paquete con el comando `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="cbec3-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="cbec3-116">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="cbec3-116">Uninstall</span></span>

<span data-ttu-id="cbec3-117">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="cbec3-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="cbec3-118">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="cbec3-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="cbec3-119">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="cbec3-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="cbec3-120">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="cbec3-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="cbec3-121">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="cbec3-121">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="cbec3-122">Si no piensa volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="cbec3-122">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="cbec3-123">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cbec3-123">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

