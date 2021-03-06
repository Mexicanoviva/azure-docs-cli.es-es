---
title: Instalación manual de la CLI de Azure para Linux
description: Cómo instalar manualmente la CLI de Azure en Linux
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9a98da54f397c1fd03a7cc6b581a769afe84ef88
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779591"
---
# <a name="install-azure-cli-on-linux-manually"></a>Instalación manual de la CLI de Azure en Linux

Si no hay ningún paquete de la CLI de Azure para su distribución, ejecute un script para instalar la CLI manualmente.

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> Se recomienda utilizar un administrador de paquetes para instalar la CLI. Con un administrador de paquetes se asegura de que siempre tendrá las últimas actualizaciones y garantiza la estabilidad de los componentes de la CLI. Compruebe si existe un paquete para su distribución antes de instalar manualmente.

## <a name="prerequisites"></a>Prerrequisitos

La CLI requiere el software siguiente:

* [Python 3.6.x, 3.7.x o 3.8.x](https://www.python.org/downloads/). 
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> La CLI ha dejado de ser compatible con Python 2.7 a partir de la versión `2.1.0`. Las nuevas versiones ya no garantizan su ejecución correcta con Python 2.7.

## <a name="install-or-update"></a>Instalación o actualización

Para instalar y actualizar la CLI es necesario volver a ejecutar el script de instalación. Ejecute `curl` para instalar la CLI.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

El script también se puede descargar y ejecutar localmente. Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell.

Después, ejecute la CLI de Azure con el comando `az`. Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Solución de problemas

Estos son algunos problemas comunes que se han observado durante la instalación manual. Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>Error de curl "Object Moved" (objeto movido)

Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>Comando `az` no encontrado

Si después de la instalación no se puede ejecutar el comando y utiliza `bash` o `zsh`, debe borrar la memoria caché del hash de comandos del shell. Ejecute

```bash
hash -r
```

y compruebe si el problema se resuelve.

Este problema también puede ocurrir si no reinició el shell después de la instalación. Asegúrese de que la ubicación del comando `az` esté en `$PATH`. La ubicación del comando `az` es

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a>El servidor proxy bloquea la conexión

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Para obtener los scripts de instalación, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* Puntos de conexión usados por el administrador de paquetes de su distribución (si existe) para los paquetes principales.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Para desinstalar la CLI, puede eliminar los archivos directamente de la ubicación elegida en el momento de la instalación. La ubicación de instalación predeterminada es `$HOME`.

1. Elimine los archivos de la CLI instalados.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Modifique el archivo `$HOME/.bash_profile` para eliminar la línea siguiente:

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. Si usa `bash` o `zsh`, vuelva a cargar la memoria caché de comandos del shell.

   ```bash
   hash -r
   ```

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
