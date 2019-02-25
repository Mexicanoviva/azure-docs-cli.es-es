---
title: Ejecución de la CLI de Azure en un contenedor de Docker
description: Cómo ejecutar un contenedor de Docker que hospeda la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 2a4515f5301daca68f6e1a161fb2327f6caa0cf5
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158562"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="afa94-103">Ejecución de la CLI de Azure en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="afa94-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="afa94-104">Puede usar Docker para ejecutar un contenedor de Linux independiente con la CLI de Azure preinstalada.</span><span class="sxs-lookup"><span data-stu-id="afa94-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="afa94-105">Docker le permite comenzar rápidamente con un entorno aislado para ejecutar la CLI.</span><span class="sxs-lookup"><span data-stu-id="afa94-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="afa94-106">La imagen también puede utilizarse como base para sus propias implementaciones.</span><span class="sxs-lookup"><span data-stu-id="afa94-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="afa94-107">Ejecución en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="afa94-107">Run in a Docker container</span></span>

<span data-ttu-id="afa94-108">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="afa94-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="afa94-109">Si desea seleccionar las claves SSH de su entorno de usuario, use `-v ${HOME}/.ssh:/root/.ssh` para montar las claves SSH en el entorno.</span><span class="sxs-lookup"><span data-stu-id="afa94-109">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="afa94-110">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="afa94-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="afa94-111">Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="afa94-111">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="afa94-112">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="afa94-112">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="afa94-113">Actualización de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="afa94-113">Update Docker image</span></span>

<span data-ttu-id="afa94-114">Para actualizar con Docker es necesario extraer la nueva imagen y volver a crear los contenedores existentes.</span><span class="sxs-lookup"><span data-stu-id="afa94-114">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="afa94-115">Por este motivo, debe intentar evitar el uso de un contenedor que hospede la CLI como almacén de datos.</span><span class="sxs-lookup"><span data-stu-id="afa94-115">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="afa94-116">Actualización de la imagen local con `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="afa94-116">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="afa94-117">Desinstalación de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="afa94-117">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="afa94-118">Después de detener cualquier contenedor que ejecute la imagen de la CLI, elimínela.</span><span class="sxs-lookup"><span data-stu-id="afa94-118">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="afa94-119">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="afa94-119">Next Steps</span></span>

<span data-ttu-id="afa94-120">Ahora que está listo para usar la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.</span><span class="sxs-lookup"><span data-stu-id="afa94-120">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="afa94-121">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="afa94-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
