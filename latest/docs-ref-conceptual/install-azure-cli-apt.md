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
ms.openlocfilehash: 93d947d91973def1c05e2f5b2e7511bc1c5704a2
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="05be2-104">Instalación de la CLI de Azure 2.0 con apt</span><span class="sxs-lookup"><span data-stu-id="05be2-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="05be2-105">Si está ejecutando una distribución que incluye `apt`, como Ubuntu o Debian, hay un paquete disponible para la CLI de Azure que se puede instalar en el sistema.</span><span class="sxs-lookup"><span data-stu-id="05be2-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="05be2-106">Debe tener Python 2.7.x o Python 3.x para poder usar la CLI.</span><span class="sxs-lookup"><span data-stu-id="05be2-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="05be2-107">Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="05be2-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="05be2-108">Instalación</span><span class="sxs-lookup"><span data-stu-id="05be2-108">Install</span></span>

1. <span data-ttu-id="05be2-109">Modifique la lista de orígenes:</span><span class="sxs-lookup"><span data-stu-id="05be2-109">Modify your sources list:</span></span>
 
   - <span data-ttu-id="05be2-110">Sistema de 32 bits</span><span class="sxs-lookup"><span data-stu-id="05be2-110">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="05be2-111">Sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="05be2-111">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="05be2-112">Ejecute los siguientes comandos sudo:</span><span class="sxs-lookup"><span data-stu-id="05be2-112">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="05be2-113">Puede ejecutar la CLI de Azure con el comando `az`.</span><span class="sxs-lookup"><span data-stu-id="05be2-113">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="05be2-114">Actualizar</span><span class="sxs-lookup"><span data-stu-id="05be2-114">Update</span></span>

<span data-ttu-id="05be2-115">Para actualizar el paquete de la CLI, use `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="05be2-115">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="05be2-116">Esto actualizará todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.</span><span class="sxs-lookup"><span data-stu-id="05be2-116">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="05be2-117">Para actualizar solo la CLI, use `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="05be2-117">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="05be2-118">Desinstalación</span><span class="sxs-lookup"><span data-stu-id="05be2-118">Uninstall</span></span>

<span data-ttu-id="05be2-119">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="05be2-119">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="05be2-120">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="05be2-120">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="05be2-121">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="05be2-121">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="05be2-122">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="05be2-122">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="05be2-123">Desinstale con `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="05be2-123">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="05be2-124">Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="05be2-124">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="05be2-125">Quite los paquetes que no necesite.</span><span class="sxs-lookup"><span data-stu-id="05be2-125">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
