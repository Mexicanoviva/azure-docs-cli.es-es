---
title: "Instalación de la CLI de Azure 2.0"
description: "Consulte los documentos para la instalación de la CLI de Azure 2.0"
keywords: CLI de Azure, instalar la CLI de Azure, CLI de Azure para Python, referencia de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 36429bb23f392ff6210a9c99885df83f53768386
ms.sourcegitcommit: 5fc7d8ccf2304c5a12fb99a80f0b00a0ad2c34e9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/01/2017
---
# <a name="install-azure-cli-20"></a>Instalación de la CLI de Azure 2.0

Instale hoy mismo la nueva versión de la CLI de Azure.
La hemos mejorado y actualizado para facilitar la administración nativa de los recursos de Azure desde la línea de comandos.
Se puede usar en macOS, Linux y Windows.
Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).

> [!NOTE]
> Si está usando el modelo de Azure Service Management (ASM), [instale la CLI de Azure 1.0](/azure/cli-install-nodejs).

## <a name="a-namemacosinstall-on-macos"></a><a name="macOS"/>Instalación en macOS

En macOS, es posible instalar con [Homebrew](https://brew.sh/) o de forma manual.

### <a name="install-with-homebrew"></a>Instalación con Homebrew

1. Si no lo tiene todavía, instale Homebrew siguiendo las [instrucciones de instalación correspondientes](https://docs.brew.sh/Installation.html).

2. Si ha instalado manualmente la CLI, siga las instrucciones para la [desinstalación manual](#UninstallManually).

3. Actualice los repositorios locales de Homebrew.

   ```bash
   brew update
   ```

4. Instale el paquete `azure-cli`.

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> Si instaló anteriormente la CLI de Azure 1.0 con Homebrew, en lugar de instalar el paquete puede obtener la CLI 2.0 durante el proceso de actualización normal de Homebrew.
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a>Instalación manual

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

### <a name="install-with-msi-for-the-windows-command-line"></a>Instalación con MSI para la línea de comandos de Windows 

Para instalar la CLI en Windows y usarla en la línea de comandos de Windows, descargue y ejecute el [instalador de la CLI de Azure (MSI)](https://aka.ms/InstallAzureCliWindows).

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
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="install-with-apt-package-manager"></a>Instalación con el administrador de paquetes apt 

Para distribuciones que usan el administrador de paquetes `apt` como Ubuntu o Debian, puede instalar la CLI de Azure 2.0 a través de `apt-get`.

> [!NOTE]
> Debe tener Python 2.7.x o Python 3.x para poder usar la CLI. Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).

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

3.  Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="install-with-yum-package-manager"></a>Instalación con el administrador de paquetes yum

Para las distribuciones que utilizan el administrador de paquetes `yum` como Red Hat Enterprise Linux (RHEL), Fedora o CentOS, puede instalar la CLI de Azure 2.0 a través de `yum`.

> [!NOTE]
> Debe tener Python 2.7.x o Python 3.x para poder usar la CLI. Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).

1. Importe la clave del repositorio de Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Cree la información del repositorio `azure-cli` local:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Actualice el índice del paquete `yum` e instálelo:

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="install-with-zypper-package-manager"></a>Instalación con el administrador de paquetes zypper

Para distribuciones que usan el administrador de paquetes `zypper` como OpenSUSE o SLE, puede instalar la CLI de Azure 2.0 a través de `zypper`.

> [!NOTE]
> Debe tener Python 2.7.x o Python 3.x para poder usar la CLI. Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).

1. Importe la clave del repositorio de Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Cree la información del repositorio `azure-cli` local:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. Actualice el índice del paquete `zypper` e instálelo:

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. Ejecute la CLI desde el símbolo del sistema con el comando `az`.

## <a name="install-with-docker"></a>Instalación con Docker

Mantenemos una imagen de Docker preconfigurada con la CLI de Azure 2.0.

Instalación de la CLI con `docker run`.

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).

La CLI se instala en la imagen como el comando `az` en `/usr/local/bin`.

> [!NOTE]
> Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><a name="Linux"/>Instalación en Linux sin un administrador de paquetes

Se recomienda instalar la CLI con un administrador de paquetes si es posible. Si no desea agregar repositorios de Microsoft, o si está trabajando con una distribución para la que no se ha proporcionado ningún paquete, puede instalar manualmente la CLI.

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

Si la distribución no está indicada anteriormente, debe instalar [Python 2.7 o posterior](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) y [OpenSSL](https://www.openssl.org/source/).

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

### <a name="az-command-not-found"></a>Comando `az` no encontrado

Debe borrar la caché de hash de comandos del shell. Ejecute

```bash
hash -r
```

y compruebe si el problema se resuelve. El comando también podría no estar en su variable `$PATH`. Asegúrese de que `<install path>/bin` aparece en la variable `$PATH` y reinicie el shell si es necesario.

## <a name="uninstall-cli-1x-versions"></a>Desinstalación de las versiones 1.x de la CLI

Si tiene una versión de la CLI 1.x anterior en el sistema, puede desinstalarla según el tipo de instalación que se usó.

### <a name="uninstall-with-npm"></a>Desinstalación con npm

Quite la CLI anterior con `npm uninstall`.

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a>Desinstalación con código distribuible

Si realizó la instalación mediante [el instalador de la CLI de Azure (MSI)](http://aka.ms/webpi-azure-cli) o un [paquete de macOS](http://aka.ms/mac-azure-cli), use la misma herramienta para quitar la instalación.

### <a name="uninstall-with-docker"></a>Desinstalación con Docker

Si ha instalado una imagen de Docker para usar la versión anterior de la CLI, quite dicha imagen y los contenedores asociados. Después, puede volver a crear los contenedores después de instalar la nueva imagen de Docker, tal y como se describe en las instrucciones de instalación.

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a>Actualización de la CLI

Para actualizar la CLI de Azure, use el mismo método que usó para su instalación.

### <a name="update-with-homebrew"></a>Actualización con Homebrew

1. Si anteriormente realizó la instalación de forma manual, siga las instrucciones de [instalación con Homebrew](#macOS).

2. Actualice la información del repositorio local de Homebrew.

   ```bash
   brew update
   ```

3. Actualice los paquetes instalados.

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a>Actualización con MSI

Ejecute de nuevo el [instalador de la CLI de Azure (MSI)](https://aka.ms/InstallAzureCliWindows).

### <a name="update-with-apt"></a>Actualización con apt

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

### <a name="update-with-yum"></a>Actualización con yum

Actualice la CLI de Azure con el comando `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

### <a name="update-with-zypper"></a>Actualización con zypper

Puede actualizar el paquete con el comando `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

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

### <a name="uninstall-with-homebrew"></a>Desinstalación con Homebrew

Desinstale el paquete `azure-cli`.

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a>Desinstalación con MSI

Ejecute [MSI](https://aka.ms/InstallAzureCliWindows) de nuevo y elija la opción de desinstalación.

### <a name="uninstall-with-apt"></a>Desinstalación con apt

Desinstalación mediante `apt-get remove`:

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-yum"></a>Desinstalación con yum

1. Elimine el paquete de su equipo.

   ```bash
   sudo yum remove azure-cli
   ```

2. Si no piensa volver a instalar la CLI, elimine la información del repositorio.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-zypper"></a>Desinstalación con zypper

1. Elimine el paquete de su equipo.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Si no piensa volver a instalar la CLI, elimine la información del repositorio.

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
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

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><a name="UninstallManually"/>Desinstalación manual

Si usó el script de https://aka.ms/InstallAzureCli para instalar la CLI, siga estos pasos para desinstalarla.

1. Quite los archivos instalados.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Elimine la línea `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.

3. Si el shell utiliza una caché de comandos, vuelva a cargarlo.

   ```bash
   hash -r
   ```

> [!Note]
> La ubicación de instalación predeterminada es `/Users/<username>` para macOS y `/home/<username>` para Linux.

## <a name="report-cli-issues-and-feedback"></a>Notificación de problemas y comentarios sobre la CLI

Si aparecen errores al usar la herramienta, envíe un problema en la sección [Issues](https://github.com/Azure/azure-cli/issues) (Problemas) del repositorio de GitHub.
Para proporcionar comentarios desde la línea de comandos, use el comando `az feedback`.
