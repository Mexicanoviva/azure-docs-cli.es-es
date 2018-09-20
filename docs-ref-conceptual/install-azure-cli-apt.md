---
title: Instalación de la CLI de Azure 2.0 en Linux con apt
description: Instalación de la CLI de Azure 2.0 con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 88b4570f62858ec1e12898aea51a5dbce6d677b5
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388429"
---
# <a name="install-azure-cli-20-with-apt"></a>Instalación de la CLI de Azure 2.0 con apt

Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete de 64 bits disponible para la CLI de Azure. Este paquete se ha probado con:

* Ubuntu trusty, xenial, artful y bionic
* Debian wheezy, jessie y stretch

## <a name="install"></a>Instalación

1. <div id="install-step-1"/>Modifique la lista de orígenes:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/>Obtenga la clave de firma de Microsoft:

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. Instale la CLI de Azure:

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada. Si recibe errores de clave de firma, asegúrese de que ha [adquirido la clave de firma más reciente](#signingKey).

Después, ejecute la CLI de Azure con el comando `az`. Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solución de problemas

Estos son algunos problemas comunes que se han observado cuando se instala con `apt`. Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-fails-with-command-not-found"></a>Se produce un error en lsb_release con el mensaje "No se encontró el comando"

Cuando se ejecuta el comando `lsb_release`, verá una salida similar al siguiente error:

```output
-bash: lsb_release: command not found
```

El error se debe a que el comando `lsb_release` no está instalado. Puede resolver este problema mediante la instalación del paquete `lsb-release`.

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a>lsb_release no devuelve la versión de distribución de base

Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`. Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar. Si conoce el nombre de la versión de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente en el [paso 1 de la instalación](#install-step-1). En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre de la distribución base y establezca `AZ_REPO` en el valor correcto.

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

### <a name="apt-key-hangs"></a>bloqueos de apt-key

Si está detrás de un firewall que bloquea las conexiones salientes al puerto 11371, el comando `apt-key` podría producir errores indefinidamente. El firewall puede requerir el uso de un servidor proxy HTTP para las conexiones salientes:

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

Para determinar si tiene un servidor proxy, póngase en contacto con el administrador del sistema. Si el proxy no requiere un inicio de sesión, omita el usuario, la contraseña y el token `@`.

## <a name="update"></a>Actualizar

Para actualizar el paquete de la CLI, use `apt-get upgrade`.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> La clave de firma se actualizó en mayo de 2018 y ha sido reemplazada. Si recibe errores de clave de firma, asegúrese de que ha [adquirido la clave de firma más reciente](#signingKey).
>
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

2. Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure.

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Quite los paquetes que no necesite.

   ```bash
   sudo apt autoremove
   ```
