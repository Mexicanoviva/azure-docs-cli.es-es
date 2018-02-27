---
title: "Instalación de la CLI de Azure 2.0 en Linux con yum"
description: "Instalación de la CLI de Azure 2.0 con yum"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 5b7afe999d1afe5be40c4957d9cd0f832b680099
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/19/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="b31ad-103">Instalación de la CLI de Azure 2.0 con yum</span><span class="sxs-lookup"><span data-stu-id="b31ad-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="b31ad-104">Si está ejecutando una distribución que viene con `yum`, como RHEL, Fedora o CentOS, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="b31ad-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="b31ad-105">Este paquete se ha probado con RHEL 7, Fedora 19 y versiones posteriores y CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="b31ad-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="b31ad-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="b31ad-106">Install</span></span>

1. <span data-ttu-id="b31ad-107">Importe la clave del repositorio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b31ad-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="b31ad-108">Cree la información del repositorio `azure-cli` local.</span><span class="sxs-lookup"><span data-stu-id="b31ad-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="b31ad-109">Realice la instalación con el comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="b31ad-109">Install with the `yum install` command.</span></span> 

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="b31ad-110">Ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="b31ad-110">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="b31ad-111">Actualizar</span><span class="sxs-lookup"><span data-stu-id="b31ad-111">Update</span></span>

<span data-ttu-id="b31ad-112">Actualice la CLI de Azure con el comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="b31ad-112">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="b31ad-113">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="b31ad-113">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="b31ad-114">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="b31ad-114">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="b31ad-115">Si no piensa volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="b31ad-115">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="b31ad-116">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b31ad-116">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
