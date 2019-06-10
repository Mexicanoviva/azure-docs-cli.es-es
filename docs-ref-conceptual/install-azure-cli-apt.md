---
title: Instalación de la CLI de Azure en Linux con apt
description: Instalación de la CLI de Azure con el administrador de paquetes apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f22ada48502602cb4d9b502cb887412a6ddcf5cf
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516339"
---
# <a name="install-azure-cli-with-apt"></a>Instalación de la CLI de Azure con apt

Si está ejecutando una distribución que viene con `apt`, como Ubuntu o Debian, hay un paquete x86_64 disponible para la CLI de Azure. Este paquete se ha probado y es compatible con:

* Ubuntu trusty, xenial, artful, bionic y disco
* Debian wheezy, jessie y stretch

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> El paquete para la CLI de Azure instala su propio intérprete de Python y no utiliza el sistema Python.

## <a name="install"></a>Instalación

Ofrecemos dos formas de instalar la CLI de Azure con las distribuciones compatibles con `apt`: Como un script integral que ejecuta automáticamente los comandos de instalación, y con instrucciones que puede seguir paso a paso por su cuenta.

### <a name="install-with-one-command"></a>Instalación con un comando

Ofrecemos y mantenemos un script que ejecuta todos los comandos de instalación en un solo paso. Ejecútelo con `curl` y canalícelo directamente a `bash`, o descargue el script en un archivo e inspecciónelo antes de ejecutarlo.

> [!IMPORTANT]
> Este script solo se ha comprobado con Ubuntu 16.04 y Debian 8, y las versiones posteriores de ambos. Puede que no funcione en otras distribuciones.
> Si usa una distribución derivada como Linux Mint, siga las instrucciones de instalación manual y solucione todos los posibles problemas.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a>Instrucciones de instalación manual

Si no desea ejecutar un script como superusuario, siga estos pasos manuales para instalar la CLI de Azure.

1. Obtenga los paquetes necesarios para el proceso de instalación:

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. Descargue e instale la clave de firma de Microsoft:

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/>Agregue el repositorio de software de la CLI de Azure:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. Actualice la información del repositorio e instale el paquete `azure-cli`:

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

Ejecute la CLI de Azure con el comando `az`. Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solución de problemas

Estos son algunos problemas comunes que se han observado cuando se instala con `apt`. Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>lsb_release no devuelve la versión de distribución de base correcta

Algunas distribuciones derivadas de Ubuntu o Debian, como Linux Mint, no pueden devolver el nombre de la versión correcta de `lsb_release`. Este valor se utiliza en el proceso de instalación para determinar el paquete que desea instalar. Si conoce el nombre de código de la versión de Ubuntu o Debian de la que deriva su distribución, puede establecer el valor de `AZ_REPO` manualmente al [agregar el repositorio](#set-release). En caso contrario, busque información relativa a su distribución acerca de cómo determinar el nombre del código de distribución base y establezca `AZ_REPO` en el valor correcto.

### <a name="no-package-for-your-distribution"></a>No hay ningún paquete para su distribución

A veces hace falta un tiempo desde el lanzamiento de una distribución para que haya un paquete de la CLI de Azure disponible. La CLI de Azure se ha diseñado para ser resistente con respecto a versiones futuras de las dependencias, y a usar las menos posibles. Si no hay ningún paquete disponible para su distribución de base, pruebe un paquete de una distribución anterior.

Para ello, establezca el valor de `AZ_REPO` manualmente al [agregar el repositorio](#set-release). Para las distribuciones de Ubuntu, use el repositorio `bionic` y, para las distribuciones de Debian, use `stretch`. Las distribuciones lanzadas antes de Ubuntu Trusty y Debian Wheezy no se admiten.

### <a name="proxy-blocks-connection"></a>Conexión de bloques proxy

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

También puede configurar explícitamente `apt` para usar este servidor proxy en todo momento. Asegúrese de que las líneas siguientes aparecen en un archivo de configuración `apt` en `/etc/apt/apt.conf.d/`. Se recomienda usar el archivo de configuración global existente, un archivo de configuración de proxy existente, `40proxies` o `99local`, pero seguir sus requisitos de administración del sistema.

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

Si el proxy no utiliza autenticación básica, __quite__ la parte `[username]:[password]@` del URI del servidor proxy. Si necesita más información para configurar el servidor proxy, consulte la documentación oficial de Ubuntu:

* [apt.conf manpage](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [Wiki de Ubuntu: apt-get howto](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

Para obtener la clave de firma de Microsoft y obtener el paquete de nuestro repositorio, el servidor proxy debe permitir las conexiones HTTPS a la siguiente dirección:

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Actualizar

Para actualizar el paquete de la CLI, use `apt-get upgrade`.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Este comando actualiza todos los paquetes instalados en el sistema que no hayan tenido un cambio de dependencia.
> Para actualizar solo la CLI, use `apt-get install`.
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Desinstale con `apt-get remove`:

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio de la CLI de Azure:

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Quite la clave de firma:

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. Quite los paquetes que no necesite:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
