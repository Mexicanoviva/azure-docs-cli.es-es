---
title: "Ejecución de la CLI de Azure 2.0 en un contenedor de Docker"
description: "Cómo ejecutar un contenedor de Docker que hospeda la CLI de Azure 2.0"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 3a09eb6d83bb5401628bd952d199a03ecbb8216e
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="fdac3-103">Ejecución de la CLI de Azure 2.0 en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="fdac3-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="fdac3-104">Puede usar Docker para ejecutar un contenedor de Linux independiente con la CLI de Azure 2.0 preinstalada.</span><span class="sxs-lookup"><span data-stu-id="fdac3-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="fdac3-105">Docker permite empezar a trabajar rápidamente con un entorno donde puede probar la CLI y decidir si es lo que necesita o utilizar la imagen como base de su propia implementación.</span><span class="sxs-lookup"><span data-stu-id="fdac3-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="fdac3-106">Ejecución en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="fdac3-106">Run in a Docker container</span></span>

<span data-ttu-id="fdac3-107">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="fdac3-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

<span data-ttu-id="fdac3-108">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="fdac3-108">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="fdac3-109">Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="fdac3-109">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a><span data-ttu-id="fdac3-110">Actualización de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="fdac3-110">Update Docker image</span></span>

<span data-ttu-id="fdac3-111">Para actualizar con Docker es necesario extraer la nueva imagen y volver a crear los contenedores existentes.</span><span class="sxs-lookup"><span data-stu-id="fdac3-111">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="fdac3-112">Por este motivo, debe intentar evitar el uso de un contenedor que hospede la CLI como almacén de datos.</span><span class="sxs-lookup"><span data-stu-id="fdac3-112">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="fdac3-113">Actualización de la imagen local con `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="fdac3-113">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="fdac3-114">Desinstalación de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="fdac3-114">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="fdac3-115">Después de detener cualquier contenedor que ejecute la imagen de la CLI, elimínela.</span><span class="sxs-lookup"><span data-stu-id="fdac3-115">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
