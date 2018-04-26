---
title: Instalación de la CLI de Azure 2.0 en Linux con yum
description: Instalación de la CLI de Azure 2.0 con yum
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 6a63d1ccd6b182b0c7144101f7efbf3264a6cb72
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="ab0f1-103">Instalación de la CLI de Azure 2.0 con yum</span><span class="sxs-lookup"><span data-stu-id="ab0f1-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="ab0f1-104">Si está ejecutando una distribución que viene con `yum`, como RHEL, Fedora o CentOS, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="ab0f1-105">Este paquete se ha probado con RHEL 7, Fedora 19 y versiones posteriores y CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="ab0f1-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="ab0f1-106">Install</span></span>

1. <span data-ttu-id="ab0f1-107">Importe la clave del repositorio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="ab0f1-108">Cree la información del repositorio `azure-cli` local.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="ab0f1-109">Realice la instalación con el comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-109">Install with the `yum install` command.</span></span> 

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="ab0f1-110">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ab0f1-111">Para iniciar sesión, ejecute el comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-111">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="ab0f1-112">Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ab0f1-112">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="ab0f1-113">Actualizar</span><span class="sxs-lookup"><span data-stu-id="ab0f1-113">Update</span></span>

<span data-ttu-id="ab0f1-114">Actualice la CLI de Azure con el comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="ab0f1-115">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="ab0f1-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="ab0f1-116">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="ab0f1-117">Si no piensa volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-117">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="ab0f1-118">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ab0f1-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
