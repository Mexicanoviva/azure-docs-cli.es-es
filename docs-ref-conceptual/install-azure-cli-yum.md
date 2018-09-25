---
title: Instalación de la CLI de Azure 2.0 en Linux con yum
description: Instalación de la CLI de Azure 2.0 con yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 25eb473aa56d3ddd34f8e1808b84ebb5f6324f2b
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/20/2018
ms.locfileid: "46470021"
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="56d21-103">Instalación de la CLI de Azure 2.0 con yum</span><span class="sxs-lookup"><span data-stu-id="56d21-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="56d21-104">Para distribuciones Linux con `yum`, como RHEL, Fedora o CentOS, hay un paquete de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="56d21-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="56d21-105">Este paquete se ha probado con RHEL 7, Fedora 19 y versiones posteriores y CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="56d21-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="56d21-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="56d21-106">Install</span></span>

1. <span data-ttu-id="56d21-107">Importe la clave del repositorio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="56d21-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="56d21-108">Cree la información del repositorio `azure-cli` local.</span><span class="sxs-lookup"><span data-stu-id="56d21-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="56d21-109">Realice la instalación con el comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="56d21-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="56d21-110">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="56d21-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="56d21-111">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="56d21-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="56d21-112">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="56d21-112">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="56d21-113">Actualizar</span><span class="sxs-lookup"><span data-stu-id="56d21-113">Update</span></span>

<span data-ttu-id="56d21-114">Actualice la CLI de Azure con el comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="56d21-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="56d21-115">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="56d21-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="56d21-116">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="56d21-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="56d21-117">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="56d21-117">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="56d21-118">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="56d21-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

## <a name="next-steps"></a><span data-ttu-id="56d21-119">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="56d21-119">Next Steps</span></span>

<span data-ttu-id="56d21-120">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="56d21-120">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="56d21-121">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="56d21-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
