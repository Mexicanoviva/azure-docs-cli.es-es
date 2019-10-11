---
title: Instalación de la CLI de Azure para macOS
description: Cómo instalar la CLI de Azure en macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 790c63a60a5d23863b48227dcc99462bbf950d80
ms.sourcegitcommit: b42ce26476b135bb2047c8d9d787580c858f8b6b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/09/2019
ms.locfileid: "72163850"
---
# <a name="install-azure-cli-on-macos"></a>Instalación de la CLI de Azure en macOS

Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](https://brew.sh). Homebrew facilita mantener actualizada la instalación de la CLI. El paquete de la CLI se ha probado en las versiones de Mac OS 10.9 y versiones posteriores.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a>Instalación con Homebrew

Homebrew es la manera más fácil de administrar la instalación de la CLI. Ofrece formas cómodas de instalar, actualizar y desinstalar.
Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.

Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> La CLI de Azure tiene una dependencia en el paquete `python3` de Homebrew, y lo instalará.
> Se garantiza que la CLI de Azure será compatible con la versión más reciente de `python3` publicada en Homebrew.

Después, ejecute la CLI de Azure con el comando `az`. Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solución de problemas

Si se produce un problema al instalar la CLI a través de Homebrew, aquí se muestran algunos errores comunes. Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>No se puede encontrar Python o los paquetes instalados

Puede haber una discrepancia con la versión secundaria u otros problemas durante la instalación de Homebrew. La CLI no usa un entorno virtual de Python y debe buscar la versión de Python instalada. Una posible solución consiste en instalar y volver a vincular la dependencia de `python3` desde Homebrew.

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>Versión de la CLI 1.x instalada

Si se instaló una versión no actualizada, podría deberse a que la memoria caché de Homebrew estaba obsoleta. Siga las instrucciones de [actualización](#update).

### <a name="proxy-blocks-connection"></a>Conexión de bloques proxy

No puede obtener recursos de Homebrew, a menos que lo haya configurado correctamente para usar el servidor proxy. Siga las [instrucciones de configuración del servidor proxy de Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).

> [!IMPORTANT]
> Si está detrás de un servidor proxy, `HTTP_PROXY` y `HTTPS_PROXY` deben establecerse para conectarse a los servicios de Azure con la CLI.
> Si no utiliza autenticación básica, se recomienda exportar estas variables en su archivo `.bashrc`.
> Siga siempre las directivas de seguridad de su empresa y los requisitos del administrador del sistema.

Para obtener los recursos Bottle de Homebrew, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a>Actualizar

La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar. Hay una nueva versión disponible aproximadamente cada dos semanas. Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete `azure-cli`.

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Use Homebrew para desinstalar el paquete `azure-cli`.

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a>Otros métodos de instalación

Si no puede usar Homebrew para instalar la CLI de Azure en su entorno, es posible usar las instrucciones manuales para Linux. Tenga en cuenta que este proceso no se mantiene oficialmente para que sea compatible con macOS. Siempre se recomienda usar un administrador de paquetes como Homebrew. Solo debe usar el método de instalación manual si no dispone de ninguna otra opción.

Para las instrucciones de instalación manual, consulte [Instalación de la CLI de Azure en Linux manualmente](install-azure-cli-linux.md).

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
