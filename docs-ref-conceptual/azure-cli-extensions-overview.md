---
title: Extensiones de la CLI de Azure 2.0
description: Uso de extensiones con la CLI de Azure 2.0
keywords: CLI de Azure, extensiones
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b503c51ffc55ceda30738e34171c7da92532f328
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967731"
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Uso de extensiones con la CLI de Azure 2.0

Las extensiones son módulos individuales que no se distribuyen con la propia CLI de Azure y que agregan funcionalidad mediante nuevos comandos. Podría tratarse de ofertas experimentales o de una versión preliminar, herramientas especializadas de Microsoft o características personalizadas escritas por usted. Las extensiones aportan a la CLI un grado de flexibilidad que le permite modificarla según sus propias necesidades, sin tener que enviar una gran cantidad de paquetes adicionales que no se consideran parte del conjunto de características principales.

Este artículo le ayuda a aprender a instalar, actualizar y eliminar extensiones de la CLI. También responde a preguntas comunes sobre el comportamiento de las extensiones.

## <a name="find-extensions"></a>Buscar extensiones

Para saber qué extensiones están disponibles, puede usar [az extension list-available](/cli/azure/extension#az-extension-list-available). Este comando muestra las extensiones oficiales proporcionadas y mantenidas por Microsoft.

```azurecli-interactive
az extension list-available --output table
```

También hospedamos una [lista de las extensiones de Microsoft](azure-cli-extensions-list.md) en el sitio de documentación.

## <a name="install-extensions"></a>Instalar extensiones

Una vez que haya encontrado una extensión para instalar, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) para obtenerla. Si la extensión aparece enumerada en `az extension list-available`, puede instalarla por nombre.

```azurecli-interactive
az extension add --name <extension-name>
```

Si la extensión es de un recurso externo o dispone de un vínculo directo a ella, puede proporcionar la dirección URL de origen o la ruta de acceso local. Esto _debe_ ser un archivo wheel de Python compilado.

```azurecli-interactive
az extension add --source <URL-or-path>
```

Cuando se instala una extensión, se puede encontrar en el valor de la variable del shell `$AZURE_EXTENSION_DIR`. Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.

## <a name="update-extensions"></a>Actualizar extensiones

Si se instaló una extensión por nombre, se puede actualizar con [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).

```azurecli-interactive
az extension update --name <extension-name>
```

En caso contrario, una extensión se puede actualizar desde el origen siguiendo las instrucciones de [Instalar extensiones](#install-extensions).

Si un nombre de extensión no se puede resolver mediante la CLI, desinstálela e intente volver a instalarla. También es posible que la extensión haya dejado de estar en versión preliminar y se haya convertido en un comando integrado de la CLI. Intente actualizar la CLI, tal y como se describe en [Instalación de la CLI de Azure 2.0](install-azure-cli.md) y vea si se agregaron los comandos de la extensión.

## <a name="uninstall-extensions"></a>Desinstalar extensiones

Si ya no necesita una extensión, se puede eliminar con [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).

```azurecli-interactive
az extension remove --name <extension-name>
```

También puede eliminar una extensión de forma manual mediante su eliminación de la ubicación donde se instaló. Este será el valor de la variable del shell `$AZURE_EXTENSION_DIR`.
Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

Se recomienda realizar la desinstalación con `az extension remove`.

## <a name="faq"></a>Preguntas más frecuentes

A continuación encontrará respuestas a otras preguntas comunes acerca de las extensiones de la CLI.

### <a name="what-file-formats-are-allowed-for-installation"></a>¿Qué formatos de archivo se permiten para la instalación?

Actualmente, solo pueden instalarse archivos wheel de Python compilados como extensiones.

### <a name="can-extensions-replace-existing-commands"></a>¿Pueden reemplazar las extensiones a comandos existentes?

Sí. Las extensiones pueden reemplazar comandos existentes pero, antes de ejecutar un comando que se ha reemplazado, la CLI emitirá una advertencia.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>¿Cómo se puede saber si una extensión está en versión preliminar?

Una extensión debe indicar si se encuentra en versión preliminar en su propia documentación y en el control de versiones. También es común que Microsoft publique comandos de la CLI en versión preliminar como extensiones, con intención de moverlos a la interfaz principal de la CLI una vez que el producto haya dejado de estar en versión preliminar.

### <a name="can-extensions-depend-upon-each-other"></a>¿Las extensiones pueden depender entre sí?

No. Las extensiones deben ser paquetes individuales que no confían entre sí. Esto es porque la CLI no ofrece ninguna garantía sobre cuándo se cargan las extensiones, por lo que no se puede garantizar que las dependencias se cumplan. La instalación de una extensión instala solo esa extensión y debe continuar funcionando aunque elimine otras extensiones.

### <a name="are-extensions-updated-along-with-the-cli"></a>¿Las extensiones se actualizan junto con la CLI?

No. Las extensiones deben actualizarse por separado, tal y como se describe en la sección [Actualizar extensiones](#update-extensions).
