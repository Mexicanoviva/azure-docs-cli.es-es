---
title: "Instalación de la CLI de Azure 2.0 en Linux con apt"
description: "Instalación de la CLI de Azure 2.0 con el administrador de paquetes apt"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 840e5e7d6531fe92d30235f621e381589266d1d3
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/19/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="dfd47-103">Instalación de la CLI de Azure 2.0 con apt</span><span class="sxs-lookup"><span data-stu-id="dfd47-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="dfd47-104">Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="dfd47-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="dfd47-105">Este paquete se ha probado con:</span><span class="sxs-lookup"><span data-stu-id="dfd47-105">This package has been tested with:</span></span>

* <span data-ttu-id="dfd47-106">Ubuntu trusty, xenial y artful</span><span class="sxs-lookup"><span data-stu-id="dfd47-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="dfd47-107">Debian wheezy, jessie y stretch</span><span class="sxs-lookup"><span data-stu-id="dfd47-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="dfd47-108">Instalación</span><span class="sxs-lookup"><span data-stu-id="dfd47-108">Install</span></span>

1. <span data-ttu-id="dfd47-109">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="dfd47-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="dfd47-110">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="dfd47-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="dfd47-111">Puede ejecutar la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="dfd47-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="dfd47-112">solución de problemas</span><span class="sxs-lookup"><span data-stu-id="dfd47-112">Troubleshooting</span></span>

<span data-ttu-id="dfd47-113">Estos son algunos problemas comunes que se han observado cuando se instala con `apt`.</span><span class="sxs-lookup"><span data-stu-id="dfd47-113">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="dfd47-114">Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="dfd47-114">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="dfd47-115">Se produce un error en el comando apt-key con "No dirmngr"</span><span class="sxs-lookup"><span data-stu-id="dfd47-115">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="dfd47-116">Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:</span><span class="sxs-lookup"><span data-stu-id="dfd47-116">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="dfd47-117">El error es debido a que falta un componente que `apt-key` necesita.</span><span class="sxs-lookup"><span data-stu-id="dfd47-117">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="dfd47-118">Puede resolver este problema mediante la instalación del paquete `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="dfd47-118">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="dfd47-119">Actualizar</span><span class="sxs-lookup"><span data-stu-id="dfd47-119">Update</span></span>

<span data-ttu-id="dfd47-120">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="dfd47-120">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="dfd47-121">Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="dfd47-121">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="dfd47-122">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="dfd47-122">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="dfd47-123">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="dfd47-123">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="dfd47-124">Desinstale con `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="dfd47-124">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="dfd47-125">Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="dfd47-125">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="dfd47-126">Quite los paquetes que no necesite.</span><span class="sxs-lookup"><span data-stu-id="dfd47-126">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
