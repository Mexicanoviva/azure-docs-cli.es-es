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
ms.openlocfilehash: 7a12da712cd2aad5bb5fb56e27267a8e05df34a6
ms.sourcegitcommit: cae66f994cb7b7f829f75ac528093fdb6851f64e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/31/2018
---
# <a name="install-azure-cli-20-with-docker"></a>Instalación de la CLI de Azure 2.0 con Docker

Puede usar Docker para instalar un contenedor de Linux independiente con la CLI de Azure 2.0 preinstalada. Esto le permite empezar a trabajar rápidamente con un entorno donde puede probar la CLI y decidir si es lo que necesita, o utilizarla como imagen de base.

## <a name="install-with-docker"></a>Instalación con Docker

Instalación de la CLI con `docker run`.

   ```bash
   docker run -it microsoft/azure-cli:<version>
   ```

Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/microsoft/azure-cli/tags/).

La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.

> [!NOTE]
> Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli:<version>
> ```

### <a name="update-with-docker"></a>Actualización con Docker

Para actualizar con Docker es necesario extraer la nueva imagen y volver a crear los contenedores existentes. Por este motivo, debe intentar evitar el uso de un contenedor que hospede la CLI como almacén de datos.

1. Actualización de la imagen local con `docker pull`.

   ```bash
   docker pull microsoft/azure-cli
   ```

2. Obtenga los contenedores que está usando con la imagen de la CLI.

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.

3. Detenga y vuelva a crear los contenedores.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run microsoft/azure-cli
   ```

### <a name="uninstall-with-docker"></a>Desinstalación con Docker

Si alguna vez decide desinstalar la CLI, sentimos que se marche. Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella. Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos. También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).

Para desinstalar correctamente la imagen de Docker de la CLI, debe quitar los contenedores que la ejecutan y, a continuación, eliminar la imagen local.

1. Obtenga los contenedores que están ejecutando la imagen de la CLI de Azure.

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.

2. Elimine los contenedores con la imagen de la CLI.

   ```bash
   docker rm 34a868beb2ab
   ```

3. Quite la imagen de la CLI instalada localmente.

   ```bash
   docker rmi microsoft/azure-cli
   ```

