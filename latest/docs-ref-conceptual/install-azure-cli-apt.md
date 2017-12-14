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
ms.openlocfilehash: 75c531a13a4b730158cd2e874cb6c5d581a27598
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="a0c09-104">Instalación de la CLI de Azure 2.0 con apt</span><span class="sxs-lookup"><span data-stu-id="a0c09-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="a0c09-105">Si está ejecutando una distribución que incluye `apt`, como Ubuntu o Debian, hay un paquete disponible para la CLI de Azure que se puede instalar en el sistema.</span><span class="sxs-lookup"><span data-stu-id="a0c09-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="a0c09-106">Instalación</span><span class="sxs-lookup"><span data-stu-id="a0c09-106">Install</span></span>

1. <span data-ttu-id="a0c09-107">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="a0c09-107">Modify your sources list:</span></span>

   - <span data-ttu-id="a0c09-108">Sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="a0c09-108">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="a0c09-109">Sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="a0c09-109">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="a0c09-110">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="a0c09-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="a0c09-111">Puede ejecutar la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="a0c09-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="a0c09-112">Actualizar</span><span class="sxs-lookup"><span data-stu-id="a0c09-112">Update</span></span>

<span data-ttu-id="a0c09-113">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="a0c09-113">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="a0c09-114">Esto actualizará todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="a0c09-114">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="a0c09-115">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="a0c09-115">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="a0c09-116">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="a0c09-116">Uninstall</span></span>

<span data-ttu-id="a0c09-117">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="a0c09-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="a0c09-118">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="a0c09-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="a0c09-119">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="a0c09-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="a0c09-120">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="a0c09-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="a0c09-121">Desinstale con `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="a0c09-121">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="a0c09-122">Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="a0c09-122">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="a0c09-123">Quite los paquetes que no necesite.</span><span class="sxs-lookup"><span data-stu-id="a0c09-123">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
