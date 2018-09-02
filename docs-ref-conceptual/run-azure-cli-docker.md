---
title: Ejecución de la CLI de Azure 2.0 en un contenedor de Docker
description: Cómo ejecutar un contenedor de Docker que hospeda la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7a50682d549f6383e68128f2c2aef02dc2877a8e
ms.sourcegitcommit: 83826ca154c9f32c6091c63ce4b3e480694ba8d1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/09/2018
ms.locfileid: "43144882"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="6885e-103">Ejecución de la CLI de Azure 2.0 en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="6885e-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="6885e-104">Puede usar Docker para ejecutar un contenedor de Linux independiente con la CLI de Azure 2.0 preinstalada.</span><span class="sxs-lookup"><span data-stu-id="6885e-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="6885e-105">Docker permite empezar a trabajar rápidamente con un entorno donde puede probar la CLI y decidir si es lo que necesita o utilizar la imagen como base de su propia implementación.</span><span class="sxs-lookup"><span data-stu-id="6885e-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="6885e-106">Ejecución en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="6885e-106">Run in a Docker container</span></span>

<span data-ttu-id="6885e-107">Instalación de la CLI con `docker run`.</span><span class="sxs-lookup"><span data-stu-id="6885e-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="6885e-108">Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}/.ssh:/root/.ssh` para montar las claves SSH en el entorno.</span><span class="sxs-lookup"><span data-stu-id="6885e-108">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="6885e-109">La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="6885e-109">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="6885e-110">Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="6885e-110">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6885e-111">Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6885e-111">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="6885e-112">Actualización de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="6885e-112">Update Docker image</span></span>

<span data-ttu-id="6885e-113">Para actualizar con Docker es necesario extraer la nueva imagen y volver a crear los contenedores existentes.</span><span class="sxs-lookup"><span data-stu-id="6885e-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="6885e-114">Por este motivo, debe intentar evitar el uso de un contenedor que hospede la CLI como almacén de datos.</span><span class="sxs-lookup"><span data-stu-id="6885e-114">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="6885e-115">Actualización de la imagen local con `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="6885e-115">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="6885e-116">Desinstalación de una imagen de Docker</span><span class="sxs-lookup"><span data-stu-id="6885e-116">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="6885e-117">Después de detener cualquier contenedor que ejecute la imagen de la CLI, elimínela.</span><span class="sxs-lookup"><span data-stu-id="6885e-117">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
