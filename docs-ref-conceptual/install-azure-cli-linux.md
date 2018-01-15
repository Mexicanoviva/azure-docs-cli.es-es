---
title: "Instalación manual de la CLI de Azure 2.0 para Linux"
description: "Instalación manual de la CLI de Azure 2.0 para Linux"
keywords: CLI de Azure, instalar la CLI de Azure, azure linux, azure instalar linux
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Instalación manual de la CLI de Azure 2.0 en Linux

Si no tiene un paquete de la CLI de Azure disponible en la distribución, siempre puede ejecutar manualmente un script de instalación para instalar la CLI. Si dispone de un paquete, siempre es el método de instalación recomendado.

## <a name="prerequisites"></a>Requisitos previos

Para instalar la CLI, necesitará el siguiente software disponible en el sistema:

* [Python 2.7 o Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a>Instalación o actualización manual

Tanto si va a instalar como si va a actualizar la CLI, debe realizar una instalación completa. Una vez que tenga los requisitos previos, puede instalar la CLI ejecutando `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Si no tiene `curl` en el sistema o prefiere ejecutar el script, puede descargarlo y ejecutarlo localmente. Para que algunos cambios surtan efecto, es posible que tenga que reiniciar el shell. Después de la instalación, ejecute la CLI con el comando `az`.

## <a name="troubleshooting"></a>solución de problemas

### <a name="curl-object-moved-error"></a>Error de curl "Object Moved" (objeto movido)

Si `curl` muestra un error relacionado con el parámetro `-L` o un mensaje de error con el texto "Object Moved" (Objeto movido), pruebe a usar la dirección URL completa en lugar de la redirección `aka.ms`:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>Comando `az` no encontrado

Si después de la instalación no se puede ejecutar el comando, debe borrar la memoria caché del hash de comandos del shell. Ejecute

```bash
hash -r
```

y compruebe si el problema se resuelve.

Esto también puede ocurrir si no se reinició el shell después de la instalación. Asegúrese de que la ubicación del comando `az` esté en `$PATH`.

Si ha ejecutado el script de instalación, la ruta será:

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a>Desinstalación manual

Si alguna vez decide desinstalar la CLI, sentimos que se marche. Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella. Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos. También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).

Para desinstalar la CLI, puede eliminar los archivos directamente de la ubicación de instalación. La ubicación de instalación se elige en el momento de la instalación, si realizó la instalación mediante el script `https://aka.ms/InstallAzureCLI`. La ubicación de instalación predeterminada es `$HOME`.

En primer lugar, quite los archivos de la CLI instalados:

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

A continuación, modifique su archivo `$HOME/.bash_profile` para quitar la línea:

```
<install location>/lib/azure-cli/az.completion
```

Y, por último, vuelva a cargar la memoria caché de comandos del shell, si utiliza una. Los usuarios de `bash` y `zsh` tendrán que realizar este paso:

```bash
hash -r
```
