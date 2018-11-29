---
title: Instalación de la CLI de Azure en Linux con yum
description: Cómo instalar la CLI de Azure con yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7e2c7c5477c8d5a617875eeaed8e3d267d9bcf8c
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450316"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="e9fb5-103">Instalación de la CLI de Azure con yum</span><span class="sxs-lookup"><span data-stu-id="e9fb5-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="e9fb5-104">Para distribuciones Linux con `yum`, como RHEL, Fedora o CentOS, hay un paquete de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="e9fb5-105">Este paquete se ha probado con RHEL 7, Fedora 19 y versiones posteriores y CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="e9fb5-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="e9fb5-106">Install</span></span>

1. <span data-ttu-id="e9fb5-107">Importe la clave del repositorio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="e9fb5-108">Cree la información del repositorio `azure-cli` local.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="e9fb5-109">Realice la instalación con el comando `yum install`.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="e9fb5-110">Después, ejecute la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="e9fb5-111">Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="e9fb5-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="e9fb5-112">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e9fb5-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e9fb5-113">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="e9fb5-113">Troubleshooting</span></span>

<span data-ttu-id="e9fb5-114">Estos son algunos problemas comunes que se han observado cuando se instala con `yum`.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="e9fb5-115">Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e9fb5-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="e9fb5-116">Actualizar</span><span class="sxs-lookup"><span data-stu-id="e9fb5-116">Update</span></span>

<span data-ttu-id="e9fb5-117">Actualice la CLI de Azure con el comando `yum update`.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-117">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="e9fb5-118">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="e9fb5-118">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="e9fb5-119">Elimine el paquete de su equipo.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-119">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="e9fb5-120">Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-120">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="e9fb5-121">Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-121">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="e9fb5-122">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="e9fb5-122">Next Steps</span></span>

<span data-ttu-id="e9fb5-123">Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="e9fb5-123">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="e9fb5-124">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="e9fb5-124">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
