---
title: Extensiones de la CLI de Azure
description: Uso de extensiones con la CLI de Azure
keywords: CLI de Azure, extensiones
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4f203f94e9b26e1219bfe69ec0ddd73228d30b64
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158875"
---
# <a name="use-extensions-with-azure-cli"></a>Uso de extensiones con la CLI de Azure 

La CLI de Azure ofrece la posibilidad de cargar extensiones. Las extensiones son archivos wheel de Python que no se distribuyen como parte de la CLI, pero se ejecutan como comandos de la CLI.
Con las extensiones, obtendrá acceso a comandos experimentales y en versión preliminar, además de poder escribir sus propias interfaces de la CLI. En este artículo se explica cómo administrar las extensiones y se da respuesta a preguntas comunes sobre su uso.

## <a name="find-extensions"></a>Buscar extensiones

Para ver las extensiones que Microsoft proporciona y mantiene, use el comando [az extension list-available](/cli/azure/extension#az-extension-list-available).

```azurecli-interactive
az extension list-available --output table
```

También hospedamos una [lista de las extensiones](azure-cli-extensions-list.md) en el sitio de documentación.

## <a name="install-extensions"></a>Instalar extensiones

Una vez que haya encontrado una extensión para instalar, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) para obtenerla. Si la extensión aparece enumerada en `az extension list-available`, puede instalarla por nombre.

```azurecli-interactive
az extension add --name <extension-name>
```

Si la extensión es de un recurso externo o dispone de un vínculo directo a ella, proporcione la dirección URL de origen o la ruta de acceso local. La extensión _debe_ ser un archivo wheel de Python compilado.

```azurecli-interactive
az extension add --source <URL-or-path>
```

Cuando se instala una extensión, se encuentra en el valor de la variable `$AZURE_EXTENSION_DIR` del shell. Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.

## <a name="update-extensions"></a>Actualizar extensiones

Si se instaló una extensión por nombre, actualícela con [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).

```azurecli-interactive
az extension update --name <extension-name>
```

En caso contrario, una extensión se puede actualizar desde el origen siguiendo las instrucciones de [Instalar extensiones](#install-extensions).

Si un nombre de extensión no se puede resolver mediante la CLI, desinstálela e intente volver a instalarla. La extensión también podría haberse vuelto parte de la CLI de base.
Intente actualizar la CLI, tal y como se describe en [Instalación de la CLI de Azure](install-azure-cli.md) y compruebe si se agregaron los comandos de la extensión.

## <a name="uninstall-extensions"></a>Desinstalar extensiones

Si ya no necesita una extensión, quítela con [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).

```azurecli-interactive
az extension remove --name <extension-name>
```

También puede eliminar una extensión de forma manual mediante su eliminación de la ubicación donde se instaló. La variable `$AZURE_EXTENSION_DIR` del shell define donde están instalados los módulos.
Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a>Preguntas más frecuentes

A continuación encontrará respuestas a otras preguntas comunes acerca de las extensiones de la CLI.

### <a name="what-file-formats-are-allowed-for-installation"></a>¿Qué formatos de archivo se permiten para la instalación?

Actualmente, solo pueden instalarse archivos wheel de Python compilados como extensiones.

### <a name="can-extensions-replace-existing-commands"></a>¿Pueden reemplazar las extensiones a comandos existentes?

Sí. Las extensiones pueden reemplazar comandos existentes pero, antes de ejecutar un comando que se ha reemplazado, la CLI emitirá una advertencia.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>¿Cómo se puede saber si una extensión está en versión preliminar?

La documentación y el control de versiones de una extensión mostrarán si se encuentra en versión preliminar. Microsoft publica periódicamente comandos en versión preliminar como extensiones de la CLI, con la opción de trasladarlos más adelante al producto de CLI principal. Cuando se retiran comandos de las extensiones, se debe desinstalar la extensión anterior. 

### <a name="can-extensions-depend-upon-each-other"></a>¿Las extensiones pueden depender entre sí?

 No. Como la CLI no garantiza un orden de carga, puede que las dependencias no se cumplan. La retirada de una extensión no afectará a las demás.

### <a name="are-extensions-updated-along-with-the-cli"></a>¿Las extensiones se actualizan junto con la CLI?

 No. Las extensiones deben actualizarse por separado, tal y como se describe en la sección [Actualizar extensiones](#update-extensions).
