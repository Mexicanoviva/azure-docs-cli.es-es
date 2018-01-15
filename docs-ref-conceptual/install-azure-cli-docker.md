---
title: "Instalación de la CLI de Azure con Docker"
description: "Instalación de un contenedor de Docker con la CLI de Azure 2.0"
keywords: CLI de Azure, instalar la CLI de Azure, azure docker, imagen de azure docker,
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 76ecf2c9cd0e6e694a31ac160112d1348863f118
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-docker"></a><span data-ttu-id="4c71b-104">Instalación de la CLI de Azure 2.0 con Docker</span><span class="sxs-lookup"><span data-stu-id="4c71b-104">Install Azure CLI 2.0 with Docker</span></span>

<span data-ttu-id="4c71b-105">Puede usar Docker para instalar un contenedor de Linux independiente con la CLI de Azure 2.0 preinstalada.</span><span class="sxs-lookup"><span data-stu-id="4c71b-105">You can use Docker to install a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="4c71b-106">Esto le permite empezar a trabajar rápidamente con un entorno donde puede probar la CLI y decidir si es lo que necesita, o utilizarla como imagen de base.</span><span class="sxs-lookup"><span data-stu-id="4c71b-106">This lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or allows you to use this as a base image.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="4c71b-107">Instalación con Docker</span><span class="sxs-lookup"><span data-stu-id="4c71b-107">Install with Docker</span></span>

<span data-ttu-id="4c71b-108">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="4c71b-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="4c71b-109">Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="4c71b-109">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="4c71b-110">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="4c71b-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="4c71b-111">Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="4c71b-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

### <a name="update-with-docker"></a><span data-ttu-id="4c71b-112">Actualización con Docker</span><span class="sxs-lookup"><span data-stu-id="4c71b-112">Update with Docker</span></span>

<span data-ttu-id="4c71b-113">Para actualizar con Docker es necesario extraer la nueva imagen y volver a crear los contenedores existentes.</span><span class="sxs-lookup"><span data-stu-id="4c71b-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="4c71b-114">Por este motivo, debe intentar evitar el uso de un contenedor que hospede la CLI como almacén de datos.</span><span class="sxs-lookup"><span data-stu-id="4c71b-114">For this reason you should try and avoid using a container which hosts the CLI as a data store.</span></span>

1. <span data-ttu-id="4c71b-115">Actualización de la imagen local con `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="4c71b-115">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="4c71b-116">Obtenga los contenedores que está usando con la imagen de la CLI.</span><span class="sxs-lookup"><span data-stu-id="4c71b-116">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > <span data-ttu-id="4c71b-117">Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.</span><span class="sxs-lookup"><span data-stu-id="4c71b-117">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="4c71b-118">Detenga y vuelva a crear los contenedores.</span><span class="sxs-lookup"><span data-stu-id="4c71b-118">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="4c71b-119">Desinstalación con Docker</span><span class="sxs-lookup"><span data-stu-id="4c71b-119">Uninstall with Docker</span></span>

<span data-ttu-id="4c71b-120">Si alguna vez decide desinstalar la CLI, sentimos que se marche.</span><span class="sxs-lookup"><span data-stu-id="4c71b-120">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="4c71b-121">Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella.</span><span class="sxs-lookup"><span data-stu-id="4c71b-121">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="4c71b-122">Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos.</span><span class="sxs-lookup"><span data-stu-id="4c71b-122">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="4c71b-123">También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="4c71b-123">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="4c71b-124">Para desinstalar correctamente la imagen de Docker de la CLI, debe quitar los contenedores que la ejecutan y, a continuación, eliminar la imagen local.</span><span class="sxs-lookup"><span data-stu-id="4c71b-124">To properly uninstall the CLI Docker image you need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="4c71b-125">Obtenga los contenedores que están ejecutando la imagen de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="4c71b-125">Get the containers running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > <span data-ttu-id="4c71b-126">Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.</span><span class="sxs-lookup"><span data-stu-id="4c71b-126">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

2. <span data-ttu-id="4c71b-127">Elimine los contenedores con la imagen de la CLI.</span><span class="sxs-lookup"><span data-stu-id="4c71b-127">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="4c71b-128">Quite la imagen de la CLI instalada localmente.</span><span class="sxs-lookup"><span data-stu-id="4c71b-128">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

