---
title: "Instalación de la CLI de Azure 2.0 en Linux con apt"
description: "Instalación de la CLI de Azure 2.0 con el administrador de paquetes apt"
keywords: CLI de Azure, instalar la CLI de Azure, azure apt, azure debian, azure ubuntu
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: fdd9f0061d5d38ed5a349b11eb0f5f27786bc1ab
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="95aaf-104">Instalación de la CLI de Azure 2.0 con apt</span><span class="sxs-lookup"><span data-stu-id="95aaf-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="95aaf-105">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="95aaf-105">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="95aaf-106">Este paquete se ha probado con Ubuntu Wheezy y Ubuntu Xenial.</span><span class="sxs-lookup"><span data-stu-id="95aaf-106">This package has been tested with Ubuntu Wheezy and Ubuntu Xenial.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="95aaf-107">Instalación</span><span class="sxs-lookup"><span data-stu-id="95aaf-107">Install</span></span>

1. <span data-ttu-id="95aaf-108">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="95aaf-108">Modify your sources list:</span></span>

   - <span data-ttu-id="95aaf-109">Sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="95aaf-109">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="95aaf-110">Sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="95aaf-110">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="95aaf-111">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="95aaf-111">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="95aaf-112">Puede ejecutar la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="95aaf-112">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="95aaf-113">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="95aaf-113">Troubleshooting</span></span>

<span data-ttu-id="95aaf-114">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="95aaf-114">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="95aaf-115">Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="95aaf-115">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="95aaf-116">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="95aaf-116">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="95aaf-117">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="95aaf-117">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="95aaf-118">El error es debido a que falta un componente que `apt-key` necesita.</span><span class="sxs-lookup"><span data-stu-id="95aaf-118">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="95aaf-119">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="95aaf-119">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="95aaf-120">Actualizar</span><span class="sxs-lookup"><span data-stu-id="95aaf-120">Update</span></span>

<span data-ttu-id="95aaf-121">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="95aaf-121">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="95aaf-122">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="95aaf-122">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="95aaf-123">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="95aaf-123">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="95aaf-124">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="95aaf-124">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="95aaf-125">Desinstale con `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="95aaf-125">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="95aaf-126">Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="95aaf-126">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="95aaf-127">Quite los paquetes que no necesite.</span><span class="sxs-lookup"><span data-stu-id="95aaf-127">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
