---
title: "Instalación de la CLI de Azure 2.0 con apt"
description: "Instalación de la CLI de Azure 2.0 con el administrador de paquetes apt"
keywords: CLI de Azure, instalar la CLI de Azure, azure apt, azure debian, azure ubuntu
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
ms.openlocfilehash: 65e8e78275b0f40a2298934fe8bc9368bbf796a7
ms.sourcegitcommit: 59f0b667f2202bae8914e6fc8dc5c9dc79fef91c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="39323-104">Instalación de la CLI de Azure 2.0 con apt</span><span class="sxs-lookup"><span data-stu-id="39323-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="39323-105">Si está ejecutando una distribución que incluye `apt`, como Ubuntu o Debian, hay un paquete disponible para la CLI de Azure que se puede instalar en el sistema.</span><span class="sxs-lookup"><span data-stu-id="39323-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="39323-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="39323-106">Install</span></span>

1. <span data-ttu-id="39323-107">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="39323-107">Modify your sources list:</span></span>

   - <span data-ttu-id="39323-108">Sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="39323-108">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="39323-109">Sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="39323-109">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="39323-110">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="39323-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="39323-111">Puede ejecutar la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="39323-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="39323-112">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="39323-112">Troubleshooting</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="39323-113">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="39323-113">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="39323-114">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error.</span><span class="sxs-lookup"><span data-stu-id="39323-114">When running the `apt-key` command, you may see output similar to the following error.</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="39323-115">Esto es debido a que falta un componente que necesita `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="39323-115">This is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="39323-116">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="39323-116">You can resolve this by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="39323-117">Actualizar</span><span class="sxs-lookup"><span data-stu-id="39323-117">Update</span></span>

<span data-ttu-id="39323-118">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="39323-118">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="39323-119">Esto actualizará todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="39323-119">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="39323-120">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="39323-120">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="39323-121">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="39323-121">Uninstall</span></span>

<span data-ttu-id="39323-122">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="39323-122">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="39323-123">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="39323-123">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="39323-124">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="39323-124">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="39323-125">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="39323-125">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="39323-126">Desinstale con `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="39323-126">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="39323-127">Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="39323-127">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="39323-128">Quite los paquetes que no necesite.</span><span class="sxs-lookup"><span data-stu-id="39323-128">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
