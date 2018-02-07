---
title: "Instalación de la CLI de Azure para macOS"
description: "Instalación de la CLI de Azure 2.0 en macOS"
keywords: CLI de Azure, instalar la CLI de Azure, azure linux, azure instalar macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 36fd2604677db0b7f820ee11884bf790fb1d75cb
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-macos"></a>Instalación de la CLI de Azure 2.0 en macOS

Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](http://brew.sh). Homebrew facilita mantener actualizada la instalación de la CLI. El paquete de la CLI se ha probado en las versiones de Mac OS 10.9 y versiones posteriores.

## <a name="install"></a>Instalación

Homebrew es la manera más fácil de administrar la instalación de la CLI. Ofrece formas cómodas de instalar, actualizar y desinstalar. Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.

Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:

```bash
brew update && brew install azure-cli
```

Después, ejecute la CLI de Azure con el comando `az`.

## <a name="troubleshooting"></a>solución de problemas

Si se produce un problema al instalar la CLI a través de Homebrew, aquí se muestran algunos errores comunes. Si su problema no está enumerado aquí, [notifique un problema en Github](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>No se puede encontrar Python o los paquetes instalados

Si la instalación no puede encontrar Python o los paquetes instalados, podría deberse a una diferencia de versión secundaria o a otro problema que se produjo durante la instalación de Homebrew. Como la CLI no usa un entorno virtual de Python, depende de que pueda encontrar la versión correcta de Python. Para corregir estos problemas, puede volver a vincular la instalación de Python.

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>Versión de la CLI 1.x instalada

Si se instaló una versión no actualizada, podría deberse a una memoria caché de Homebrew obsoleta. Siga las instrucciones de [actualización](#Update).

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
