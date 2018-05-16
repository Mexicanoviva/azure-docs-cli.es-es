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
ms.openlocfilehash: d88dbcec947372aa154bce939edd99f65cd9480f
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Ejecución de la CLI de Azure 2.0 en un contenedor de Docker

Puede usar Docker para ejecutar un contenedor de Linux independiente con la CLI de Azure 2.0 preinstalada. Docker permite empezar a trabajar rápidamente con un entorno donde puede probar la CLI y decidir si es lo que necesita o utilizar la imagen como base de su propia implementación.

## <a name="run-in-a-docker-container"></a>Ejecución en un contenedor de Docker

Instalación de la CLI con `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`. Para iniciar sesión, ejecute el comando `az login`.

```azurecli
az login
```

Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).

> [!NOTE]
> Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

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
