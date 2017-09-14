---
title: "Instalación de la CLI de Azure 2.0"
description: "Consulte los documentos para la instalación de la CLI de Azure 2.0"
keywords: CLI de Azure 2.0, Referencia de la CLI de Azure 2.0, Instalar la CLI de Azure 2.0, CLI de Azure Python, Desinstalar la CLI de Azure 2.0, CLI de Azure, Instalar la CLI de Azure, Referencia de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 00d5b555975007d7e57f04ce5d69f4f29e6d0219
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/04/2017
---
# <a name="install-azure-cli-20"></a>Instalación de la CLI de Azure 2.0

Instale hoy mismo la nueva versión de la CLI de Azure.
La hemos mejorado y actualizado para facilitar la administración nativa de los recursos de Azure desde la línea de comandos.
Se puede usar en macOS, Linux y Windows.
Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).

> [!NOTE]
> Si necesita la versión anterior de la CLI de Azure, vea aquí cómo [instalar la CLI de Azure 1.0](/azure/cli-install-nodejs).

## <a name="a-namemacosinstall-on-macos"></a><a name="macOS"/>Instalación en macOS

1. Instalación de la CLI de Azure 2.0 con `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.

   ```bash
   exec -l $SHELL
   ```
   
3. Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="install-on-windows"></a>Instalación en Windows

Puede instalar la CLI de Azure 2.0 con el archivo MSI y utilizarla en la línea de comandos de Windows, o puede instalar la CLI con `apt-get` en Bash en Ubuntu en Windows.

### <a name="install-with-msi-for-the-windows-command-line"></a>Instalación con MSI para la línea de comandos de Windows 

Para instalar la CLI en Windows y usarla en la línea de comandos de Windows, descargue y ejecute el archivo [MSI](https://aka.ms/InstallAzureCliWindows).

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a>Instalación con apt-get para Bash en Ubuntu en Windows

1. Si no dispone de Bash en Windows, [instálelo](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Abra el shell de Bash.

3. Modifique la lista de orígenes.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. Ejecute los siguientes comandos sudo:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="install-on-debianubuntu-with-apt-get"></a>Instalación en Debian/Ubuntu con apt-get

En los sistemas con Debian y Ubuntu, la CLI de Azure 2.0 se puede instalar a través de `apt-get`.

1. Modifique la lista de orígenes.
 
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
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="install-with-docker"></a>Instalación con Docker

Mantenemos una imagen de Docker preconfigurada con la CLI de Azure 2.0.

Instalación de la CLI con `docker run`.

  ```bash
  docker run azuresdk/azure-cli-python:<version>
  ```

Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).

La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.

> [!NOTE]
> Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><a name="Linux"/>Instalación en Linux sin apt-get

Se recomienda que instale la CLI con `apt-get` si es posible. Para las distribuciones que no utilizan el administrador de paquetes de `apt`, puede instalarla manualmente.

1. Instale los requisitos previos en función de la distribución de Linux.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

Si la distribución no está indicada anteriormente, debe instalar [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) y [OpenSSL](https://www.openssl.org/source/).

2. Instalación de la CLI con `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.

   ```bash
   exec -l $SHELL
   ```

4. Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="troubleshooting"></a>Solución de problemas

Si encuentra algún problema durante la instalación de la CLI, consulte esta sección para ver si su caso particular ya está descrito. Si su problema no está aquí, [notifique un problema de Github](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>Error de curl "Object Moved" (objeto movido)

Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a>Homebrew en macOS instala versiones anteriores

La fórmula `azure-cli` de Homebrew disponible para macOS no está actualizada e instalará una versión 1.x de la CLI. Para ver cuándo se actualiza, consulte `brew info azure-cli`.

Hasta entonces, [desinstale la versión anterior](#uninstall_brew) y siga las [instrucciones de instalación de macOS](#macOS).

## <a name="uninstall-cli-1x-versions"></a>Desinstalación de las versiones 1.x de la CLI

Si tiene una versión de la CLI 1.x anterior en el sistema, puede desinstalarla según el tipo de instalación que se usó.

### <a name="uninstall-with-npm"></a>Desinstalación con npm

Quite la CLI anterior con `npm uninstall`.

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><a name="uninstall_brew"/>Desinstalación con Homebrew en macOS

Quite la CLI anterior con `brew uninstall`.

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a>Desinstalación con código distribuible

Si instaló mediante [MSI](http://aka.ms/webpi-azure-cli) o un [paquete de macOS](http://aka.ms/mac-azure-cli), use la misma herramienta para quitar la instalación.

### <a name="uninstall-with-docker"></a>Desinstalación con Docker

Si ha instalado una imagen de Docker para usar la versión anterior de la CLI, quite dicha imagen y los contenedores asociados. Después, puede volver a crear los contenedores después de instalar la nueva imagen de Docker, tal y como se describe en las instrucciones de instalación.

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a>Actualización de la CLI

Para actualizar la CLI de Azure, use el mismo método que usó para su instalación.

### <a name="update-with-msi"></a>Actualización con MSI

Ejecute de nuevo el [MSI](https://aka.ms/InstallAzureCliWindows).

### <a name="update-with-apt-get"></a>Actualización con apt-get

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

### <a name="update-with-docker"></a>Actualización con Docker

1. Actualización de la imagen local con `docker pull`.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. Obtenga los contenedores que está usando con la imagen de la CLI.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.

3. Detenga y vuelva a crear los contenedores.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a>Actualización manual

Para actualizar, siga las instrucciones de instalación manual en [macOS](#macOS) o [Linux](#Linux).

## <a name="uninstall"></a>Desinstalación

Si decide desinstalar la CLI, sentimos que se marche. Debe desinstalar con el mismo método que utilizó para instalar la CLI.

### <a name="uninstall-with-msi"></a>Desinstalación con MSI

Ejecute [MSI](https://aka.ms/InstallAzureCliWindows) de nuevo y elija la opción de desinstalación.

### <a name="uninstall-with-apt-get"></a>Desinstalación con apt-get

Desinstalación mediante `apt-get remove`:

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a>Desinstalación con Docker

Si ha instalado una imagen de Docker, debe quitar los contenedores que la ejecutan y, a continuación, eliminar la imagen local.

1. Obtenga los contenedores que están ejecutando la imagen azure-cli.

  ```bash
  docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
  ```

  ```output
  CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
  34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
  ```

2. Elimine los contenedores con la imagen de la CLI.

  ```bash
  docker rm 34a868beb2ab
  ```

3. Quite la imagen de la CLI instalada localmente.

  ```bash
  docker rmi azuresdk/azure-cli-python
  ```

> [!NOTE]
> Si instaló una versión específica de la imagen, debe agregar `:<version>` al final del nombre de la imagen.

### <a name="uninstall-manually"></a>Desinstalación manual

Si usó el script de https://aka.ms/InstallAzureCli para instalar la CLI, siga estos pasos para desinstalarla.

1. Quite los archivos instalados.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Elimine la línea `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.

> [!Note]
> La ubicación de instalación predeterminada es `/Users/<username>`.

## <a name="report-cli-issues-and-feedback"></a>Notificación de problemas y comentarios sobre la CLI

Si aparecen errores al usar la herramienta, envíe un problema en la sección [Issues](https://github.com/Azure/azure-cli/issues) (Problemas) del repositorio de GitHub.
Para proporcionar comentarios desde la línea de comandos, use el comando `az feedback`.
