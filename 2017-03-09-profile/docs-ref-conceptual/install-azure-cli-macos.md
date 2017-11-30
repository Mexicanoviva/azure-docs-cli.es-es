---
title: "Instalación de la CLI de Azure para macOS"
description: "Instalación de la CLI de Azure 2.0 en macOS"
keywords: CLI de Azure, instalar la CLI de Azure, azure linux, azure instalar macOS
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-macos"></a>Instalación de la CLI de Azure 2.0 en macOS

Para la plataforma macOS, puede instalar la CLI de Azure mediante el [administrador de paquetes de Homebrew](http://brew.sh), o manualmente. El método de instalación recomendado es con Homebrew, para que sea más fácil instalarlo, obtener actualizaciones y desinstalarlo, si lo necesita.

## <a name="use-homebrew-to-install"></a>Utilice Homebrew para la instalación

Homebrew es la manera más fácil de administrar la instalación de la CLI. Ofrece formas cómodas de instalar, actualizar y desinstalar. Es similar a otros administradores de paquetes como `apt` o `yum`.
Si no tiene Homebrew disponible en el sistema, [instale Homebrew](https://docs.brew.sh/Installation.html) antes de continuar.

### <a name="install-with-homebrew"></a>Instalación con Homebrew

Para instalar la CLI, actualice la información del repositorio de Homebrew y ejecute el comando `install`:

```bash
brew update && brew install azure-cli
```

Después, ejecute la CLI de Azure con el comando `az`.

### <a name="update-with-homebrew"></a>Actualización con Homebrew

La CLI se actualiza regularmente con correcciones de errores, mejoras, nuevas características y funcionalidades en versión preliminar. Hay una nueva versión disponible aproximadamente cada dos semanas. Debe actualizar la información del repositorio local y, a continuación, actualizar el paquete de la CLI.

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a>Solución de problemas

¿Se encontró un problema al instalar o actualizar la CLI con Homebrew? Estos son algunos errores comunes que pueden producirse y métodos para diagnosticar y solucionarlos.

#### <a name="unable-to-find-python-or-installed-packages"></a>No se puede encontrar Python o los paquetes instalados

Si la instalación no puede encontrar Python o los paquetes instalados, podría deberse a una diferencia de versión secundaria o a otro problema que se produjo durante la instalación de Homebrew. Como la CLI no usa un entorno virtual, depende de que pueda encontrar las versiones correctas de Python instaladas por Homebrew. Para corregir estos problemas, puede volver a vincular la instalación de Python:

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a>La versión de la CLI no está actualizada

Si cree que la versión de la CLI que hay instalada podría estar obsoleta, debe ejecutar un comando `brew update`, seguido de `brew upgrade azure-cli`. Si la CLI no se actualiza, tenga en cuenta que los paquetes de Homebrew se lanzan más lentamente que las versiones generales. Si necesita las instalaciones más recientes de la CLI, debe [instalar manualmente](#manage-the-cli-manually).

### <a name="uninstall-with-homebrew"></a>Desinstalación con Homebrew

Si alguna vez decide desinstalar la CLI, sentimos que se marche. Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella. Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos. También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).

Si instaló con Homebrew, debe usarlo también para desinstalar.

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a>Instalación manual de la CLI

Si no puede o no desea que Homebrew administre la instalación de la CLI automáticamente, puede instalarla manualmente.

Siga las [instrucciones de instalación manual de Linux](install-azure-cli-linux.md) para instalar manualmente en macOS. macOS 10.9 y las versiones posteriores deben incluir todas las dependencias necesarias.
