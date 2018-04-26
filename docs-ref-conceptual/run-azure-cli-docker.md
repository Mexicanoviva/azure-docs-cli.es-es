---
title: Ejecución de la CLI de Azure 2.0 en un contenedor de Docker
description: Cómo ejecutar un contenedor de Docker que hospeda la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e394dc5cd375ec6d3393f45f38694f71369379d4
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/20/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="b154c-103">Ejecución de la CLI de Azure 2.0 en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="b154c-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="b154c-104">Puede usar Docker para ejecutar un contenedor de Linux independiente con la CLI de Azure 2.0 preinstalada.</span><span class="sxs-lookup"><span data-stu-id="b154c-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="b154c-105">Docker permite empezar a trabajar rápidamente con un entorno donde puede probar la CLI y decidir si es lo que necesita o utilizar la imagen como base de su propia implementación.</span><span class="sxs-lookup"><span data-stu-id="b154c-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="b154c-106">Ejecución en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="b154c-106">Run in a Docker container</span></span>

<span data-ttu-id="b154c-107">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="b154c-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

<span data-ttu-id="b154c-108">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="b154c-108">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="b154c-109">Para iniciar sesión, ejecute el comando `az login`.</span><span class="sxs-lookup"><span data-stu-id="b154c-109">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="b154c-110">Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b154c-110">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="b154c-111">Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.</span><span class="sxs-lookup"><span data-stu-id="b154c-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a><span data-ttu-id="b154c-112">Actualización de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="b154c-112">Update Docker image</span></span>

<span data-ttu-id="b154c-113">Para actualizar con Docker es necesario extraer la nueva imagen y volver a crear los contenedores existentes.</span><span class="sxs-lookup"><span data-stu-id="b154c-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="b154c-114">Por este motivo, debe intentar evitar el uso de un contenedor que hospede la CLI como almacén de datos.</span><span class="sxs-lookup"><span data-stu-id="b154c-114">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="b154c-115">Actualización de la imagen local con `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="b154c-115">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="b154c-116">Desinstalación de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="b154c-116">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="b154c-117">Después de detener cualquier contenedor que ejecute la imagen de la CLI, elimínela.</span><span class="sxs-lookup"><span data-stu-id="b154c-117">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
