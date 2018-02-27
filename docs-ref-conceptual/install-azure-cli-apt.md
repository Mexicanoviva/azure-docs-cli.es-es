---
title: "Instalación de la CLI de Azure 2.0 en Linux con apt"
description: "Instalación de la CLI de Azure 2.0 con el administrador de paquetes apt"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 840e5e7d6531fe92d30235f621e381589266d1d3
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/19/2018
---
# <a name="install-azure-cli-20-with-apt"></a>Instalación de la CLI de Azure 2.0 con apt

Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure. Este paquete se ha probado con:

* Ubuntu trusty, xenial y artful
* Debian wheezy, jessie y stretch

## <a name="install"></a>Instalación

1. Modifique la lista de orígenes:

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
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

Estos son algunos problemas comunes que se han observado cuando se instala con `apt`. Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).

### <a name="apt-key-fails-with-no-dirmngr"></a>Se produce un error en el comando apt-key con "No dirmngr"

Cuando se ejecuta el comando `apt-key`, verá una salida similar al siguiente error:

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

El error es debido a que falta un componente que `apt-key` necesita. Puede resolver este problema mediante la instalación del paquete `dirmngr`.

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a>Actualizar

Para actualizar el paquete de la CLI, use `apt-get upgrade`.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.
> Para actualizar solo la CLI, use `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

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
