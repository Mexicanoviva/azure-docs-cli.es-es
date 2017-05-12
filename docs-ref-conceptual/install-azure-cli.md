---
title: "Instalación de la CLI de Azure 2.0"
description: Documentos de referencia para la CLI de Azure 2.0
keywords: "CLI de Azure 2.0, Referencia de la CLI de Azure 2.0, Instalación de la CLI de Azure 2.0, CLI de CLI de Python de Azure, Desinstalación de la CLI de Azure 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: b7c0b7c50794333b28c034de9b41f1e506053e25
ms.sourcegitcommit: 663d4188ccc4be425d3d551fe32613fafd05a764
ms.translationtype: HT
ms.contentlocale: es-ES
---
# <a name="install-azure-cli-20"></a>Instalación de la CLI de Azure 2.0

Instale hoy mismo la nueva versión de la CLI de Azure.
La hemos mejorado y actualizado para facilitar la administración nativa de los recursos de Azure desde la línea de comandos.
Se puede usar en macOS, Linux y Windows.
Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).

> [!NOTE]
> Si necesita la versión anterior de la CLI de Azure, aquí averiguará cómo [instalar Azure 1.0](/azure/cli-install-nodejs).

## <a name="macos"></a>macOS

1. Instale la CLI de Azure 2.0 con un comando `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell de comandos.

   ```bash
   exec -l $SHELL
   ```
   
3. Ejecute la CLI de Azure 2.0 desde el símbolo del sistema con el comando `az`.

> [!Note]
> Cuando la instalación se realiza con InstallAzureCli, no se admite `az component update`.
> Para actualizar a la CLI más reciente, vuelva a ejecutar `curl -L https://aka.ms/InstallAzureCli | bash`.
> 
> Para desinstalarla, consulte las [instrucciones de desinstalación del manual](#uninstall).

## <a name="windows"></a>Windows

La CLI de Azure 2.0 admite la sintaxis de los comandos de Bash, lo que hace que Bash en Ubuntu en Windows sea una manera excelente de utilizar la CLI.
Si no utiliza Bash, puede instalar y utilizar la CLI en la línea de comandos de Windows.

### <a name="bash-on-ubuntu-on-windows"></a>Bash en Ubuntu en Windows

1. Si no dispone de Bash en Windows, [instálelo](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Abra el shell de Bash.

3. Si no dispone de Python, instálelo.

   ```bash
   sudo apt-get install python3
   ```

   > [!NOTE]
   > Para ver si Python está instalado, ejecute `python --version`.

4. Modifique la lista de orígenes.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

5. Ejecute los siguientes comandos sudo:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> Si la instalación se realiza con apt-get, no se admite `az component`.
> Para actualizar la CLI, vuelva a ejecutar `sudo apt-get update && sudo apt-get install azure-cli`.
> 
> Para desinstalarla, ejecute `sudo apt-get remove azure-cli`.

### <a name="windows-command-line"></a>Línea de comandos de Windows 

1. Visite el sitio de Python y [descargue Python](https://www.python.org/downloads/) para Windows.
   Al instalar Python, asegúrese de instalar el componente de Pip.
   Cando finalice la instalación, agregue Python a la variable de entorno PATH (el instalador se lo solicitará).

2. Compruebe la instalación de Python desde un símbolo del sistema.

   ```bash
   python --version
   ```

3. Instalación de la CLI de Azure 2.0 mediante `pip`.

   ```bash
   pip install --user azure-cli
   ```

4. Agregue la carpeta que contiene el archivo az.bat a la ruta de acceso.
   La CLI `az.bat` se puede instalar en `%USERPROFILE%\AppData\Roaming\Python\Scripts` o `%USERPROFILE%\AppData\Roaming\Python\PythonXY\Scripts`, donde `XY` es la versión de Python (por ejemplo, `%USERPROFILE%\AppData\Roaming\Python\Python27\Scripts`).
   Agregue la carpeta que contiene `az.bat` a la ruta de acceso.
   
4. Ejecute la CLI de Azure 2.0 desde el símbolo del sistema con el comando `az`.

> [!NOTE]
> Si la CLI de Azure 2.0 ya estaba instalada y desea ver si tiene la versión más reciente, use `az --version` para ver qué versión tiene.
> Compárela con la versión más reciente disponible en [https://pypi.python.org/pypi/azure-cli](https://pypi.python.org/pypi/azure-cli).
> 
> Para realizar la actualización a la CLI más reciente, ejecute `az component update`.
> 
> Para desinstalar la CLI, ejecute `pip uninstall azure-cli`.

## <a name="linux"></a>Linux

1. En Linux, es posible que tenga que instalar unos [requisitos previos](#linux-prerequisites) específicos.

2. Instale la CLI de Azure 2.0 con un comando `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell de comandos.

   ```bash
   exec -l $SHELL
   ```

4. Ejecute la CLI de Azure 2.0 desde el símbolo del sistema con el comando `az`.

> [!Note]
> Cuando la instalación se realiza con InstallAzureCli, no se admite `az component update`.
> Para actualizar a la CLI más reciente, vuelva a ejecutar `curl -L https://aka.ms/InstallAzureCli | bash`.
> 
> Para desinstalarla, consulte las [instrucciones de desinstalación del manual](#uninstall).

## <a name="docker"></a>Docker

Mantenemos una imagen de Docker preconfigurada con la CLI de Azure.

Instale la CLI de Azure mediante `docker run`.

```bash
docker run azuresdk/azure-cli-python:<version>
```

Para saber qué versiones hay disponibles, consulte nuestras [etiquetas de Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).

> [!NOTE]
> Si desea seleccionar las claves SSH de su entorno de usuario, puede utilizar `-v ${HOME}:/root` para montar $HOME como `/root`.
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> La imagen de Docker no admite la característica [`component` ](/cli/azure/component).
> Para actualizar la CLI de Azure 2.0, utilice `docker run` para instalar la imagen más reciente, o la imagen específica que desee.

## <a name="apt-get"></a>apt-get

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

> [!NOTE]
> Si la instalación se realiza con apt-get, no se admite `az component`.
> Para actualizar la CLI, vuelva a ejecutar `sudo apt-get update && sudo apt-get install azure-cli`.
> 
> Para desinstalarla, ejecute `sudo apt-get remove azure-cli`.

## <a name="linux-prerequisites"></a>Requisitos previos de Linux

1. Si no lo tiene, instale [Python](https://www.python.org/downloads).

2. En función de la distribución de Linux, instale los requisitos previos.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

## <a name="troubleshooting"></a>Solución de problemas
-------------------------------

### <a name="errors-with-curl-redirection"></a>Errores en el redireccionamiento de curl

Si aparece un error en el comando `curl` relacionado con el parámetro `-L` o el error "Objeto movido", pruebe a usar la dirección URL completa, en lugar de la URL aka.ms:

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```


### <a name="errors-on-install-with-cffi-or-cryptography"></a>Errores en la instalación con `cffi` o criptografía

Si aparecen errores al realizar la instalación en OS X, actualice `pip`.

```bash
pip install --upgrade --force-reinstall pip
```

Si se producen errores al realizar la instalación en **Debian** o **Ubuntu**, como en estos ejemplos, instale `libssl-dev` y `libffi-dev`.

```bash
sudo apt-get update
sudo apt-get install -y libssl-dev libffi-dev
```

Instale también Python Dev como versión de Python.

Python 2:

```bash
sudo apt-get install -y python-dev
```

Python 3:

```bash
sudo apt-get install -y python3-dev
```

Ubuntu 15 puede requerir `build-essential` también:

```bash
sudo apt-get install -y build-essential
```

### <a name="example-errors"></a>Ejemplos de errores

```
Downloading cffi-1.5.2.tar.gz (388kB)
    100% |################################| 389kB 3.9MB/s
    Complete output from command python setup.py egg_info:

        No working compiler found, or bogus compiler options
        passed to the compiler from Python's distutils module.
        See the error messages above.
        (If they are about -mno-fused-madd and you are on OS/X 10.8,
        see http://stackoverflow.com/questions/22313407/ .)

    ----------------------------------------
Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-build-77i2fido/cffi/
```

```
#include <openssl/e_os2.h>
                            ^
compilation terminated.
error: command 'x86_64-linux-gnu-gcc' failed with exit status 1

Failed building wheel for cryptography
```

Vea la pregunta relativa a Stack Overflow - [No se pudo instalar el paquete de criptografía de Python con PIP y setup.py](http://stackoverflow.com/questions/22073516/failed-to-install-python-cryptography-package-with-pip-and-setup-py)

## <a name="uninstall"></a>Desinstalación

Si usó el script de https://aka.ms/InstallAzureCli para instalar la CLI, siga estos pasos para desinstalarla.

1. Quite los archivos instalados.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Elimine la línea `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.

> [!Note]
> La ubicación de instalación predeterminada es `/Users/<username>`.

Si ha usado pip, apt-get o Docker para instalar la CLI, utilice la misma herramienta para desinstalarla.

## <a name="reporting-issues-and-feedback"></a>Notificación de problemas y comentarios

Si aparecen errores al usar la herramienta, envíe un problema en la sección [Issues](https://github.com/Azure/azure-cli/issues) (Problemas) del repositorio de GitHub.
Para enviar comentarios desde la línea de comandos, pruebe a hacerlo con el comando `az feedback`.
