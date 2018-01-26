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
ms.openlocfilehash: 65e8e78275b0f40a2298934fe8bc9368bbf796a7
ms.sourcegitcommit: 59f0b667f2202bae8914e6fc8dc5c9dc79fef91c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2018
---
# <a name="install-azure-cli-20-with-apt"></a>Instalación de la CLI de Azure 2.0 con apt

Si está ejecutando una distribución que incluye `apt`, como Ubuntu o Debian, hay un paquete disponible para la CLI de Azure que se puede instalar en el sistema.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalación

1. Modifique la lista de orígenes:

   - Sistema de 32 bits

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - Sistema de 64 bits

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Ejecute los siguientes comandos sudo:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

Puede ejecutar la CLI de Azure con el comando `az`.

## <a name="troubleshooting"></a>solución de problemas

### <a name="apt-key-fails-with-no-dirmngr"></a>Se produce un error en el comando apt-key con "No dirmngr"

Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error.

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

Esto es debido a que falta un componente que necesita `apt-key`. Puede resolver este problema mediante la instalación del paquete `dirmngr`.

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a>Actualizar

Para actualizar el paquete de la CLI, use `apt-get upgrade`.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Esto actualizará todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.
> Para actualizar solo la CLI, use `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a>Desinstalación

Si alguna vez decide desinstalar la CLI, sentimos que se marche. Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella. Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos. También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).

1. Desinstale con `apt-get remove`.

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Si no piensa volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Quite los paquetes que no necesite.

   ```bash
   sudo apt autoremove
   ```
