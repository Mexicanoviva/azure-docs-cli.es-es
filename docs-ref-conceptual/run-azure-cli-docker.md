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
