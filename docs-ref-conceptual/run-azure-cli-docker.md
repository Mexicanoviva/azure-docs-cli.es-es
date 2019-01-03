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
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593836"
---
# <a name="run-azure-cli-in-a-docker-container"></a>Ejecución de la CLI de Azure en un contenedor de Docker

Puede usar Docker para ejecutar un contenedor de Linux independiente con la CLI de Azure preinstalada. Docker le permite comenzar rápidamente con un entorno aislado para ejecutar la CLI. La imagen también puede utilizarse como base para sus propias implementaciones.

## <a name="run-in-a-docker-container"></a>Ejecución en un contenedor de Docker

Instalación de la CLI con `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> Si desea seleccionar las claves SSH de su entorno de usuario, use `-v ${HOME}/.ssh:/root/.ssh` para montar las claves SSH en el entorno.
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`. Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="update-docker-image"></a>Actualización de una imagen de Docker

Para actualizar con Docker es necesario extraer la nueva imagen y volver a crear los contenedores existentes. Por este motivo, debe intentar evitar el uso de un contenedor que hospede la CLI como almacén de datos.

Actualización de la imagen local con `docker pull`.

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a>Desinstalación de una imagen de Docker

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Después de detener cualquier contenedor que ejecute la imagen de la CLI, elimínela.

```bash
docker rmi microsoft/azure-cli
```

## <a name="next-steps"></a>Pasos siguientes

Ahora que está listo para usar la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
