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
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/16/2017
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

Puede instalar la CLI con el archivo MSI y utilizarla en la línea de comandos de Windows, o puede instalar la CLI con get-apt en Bash en Ubuntu en Windows.

### <a name="msi-for-the-windows-command-line"></a>MSI para la línea de comandos de Windows 

Para instalar la CLI en Windows y usarla en la línea de comandos de Windows, descargue y ejecute el archivo [msi](https://aka.ms/InstallAzureCliWindows).

> [!NOTE]
> Si la instalación se realiza con el archivo msi, `az component` no es compatible.
> Para actualizar a la última CLI, ejecute [msi](https://aka.ms/InstallAzureCliWindows) de nuevo.
> 
> Para desinstalar la CLI, ejecute [msi](https://aka.ms/InstallAzureCliWindows) de nuevo y elija la opción de desinstalación.

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a>apt-get para Bash en Ubuntu en Windows

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

> [!NOTE]
> Si la instalación se realiza con apt-get, no se admite `az component`.
> Para actualizar la CLI, vuelva a ejecutar `sudo apt-get update && sudo apt-get install azure-cli`.
> 
> Para desinstalarla, ejecute `sudo apt-get remove azure-cli`.

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

Si ha usado apt-get, Docker o el msi para instalar la CLI, utilice la misma herramienta para desinstalarla.

## <a name="reporting-issues-and-feedback"></a>Notificación de problemas y comentarios

Si aparecen errores al usar la herramienta, envíe un problema en la sección [Issues](https://github.com/Azure/azure-cli/issues) (Problemas) del repositorio de GitHub.
Para enviar comentarios desde la línea de comandos, pruebe a hacerlo con el comando `az feedback`.
