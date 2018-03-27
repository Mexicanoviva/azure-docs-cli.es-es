---
title: Extensiones de la CLI de Azure 2.0
description: Uso de extensiones con la CLI de Azure 2.0
keywords: CLI de Azure, extensiones
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 548c06c64cc98598a2bd24bcc5959e59bffb4930
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Uso de extensiones con la CLI de Azure 2.0

Las extensiones son módulos individuales que no se distribuyen con la propia CLI de Azure y que agregan funcionalidad mediante nuevos comandos. Podría tratarse de ofertas experimentales o de una versión preliminar, herramientas especializadas de Microsoft o características personalizadas escritas por usted. Las extensiones aportan a la CLI un grado de flexibilidad que le permite modificarla según sus propias necesidades, sin tener que enviar una gran cantidad de paquetes adicionales que no se consideran parte del conjunto de características principales.

Este artículo le ayuda a aprender a instalar, actualizar y eliminar extensiones de la CLI. También responde a preguntas comunes sobre el comportamiento de las extensiones.

## <a name="finding-extensions"></a>Búsqueda de extensiones

Para saber qué extensiones están disponibles, puede usar [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az_extension_list_available). Este comando enumera las extensiones disponibles oficiales proporcionadas por Microsoft.

## <a name="installing-extensions"></a>Instalación de extensiones

Una vez que haya encontrado una extensión para instalar, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_add) para obtenerla. Si la extensión aparece enumerada en `az extension list-available`, puede instalarla por nombre.

```azurecli
az extension add --name <extension-name>
```

Si la extensión es de un recurso externo o dispone de un vínculo directo a ella, puede proporcionar la dirección URL de origen o la ruta de acceso local. Esto _debe_ ser un archivo wheel de Python compilado.

```azurecli
az extension add --source <URL-or-path>
```

Cuando se instala una extensión, se puede encontrar en el valor de la variable del shell `$AZURE_EXTENSION_DIR`. Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.

## <a name="updating-extensions"></a>Actualización de extensiones

Las extensiones se pueden actualizar solo por nombre, mediante [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_update).

```azurecli
az extension update --name <extension-name>
```

Si no se puede resolver un nombre de extensión mediante la CLI por cualquier motivo, vuelva a instalar la extensión para actualizarla. También es posible que la extensión haya dejado de estar en versión preliminar y se haya convertido en un comando integrado de la CLI. En ese caso, actualice la CLI y desinstale la extensión.

## <a name="uninstalling-extensions"></a>Desinstalación de extensiones

Si ya no necesita una extensión, se puede eliminar con [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_remove).

```azurecli
az extension remove --name <extension-name>
```

También puede eliminar una extensión de forma manual mediante su eliminación de la ubicación donde se instaló. Este será el valor de la variable del shell `$AZURE_EXTENSION_DIR`. Si esta variable no está establecida, el valor predeterminado es `$HOME/.azure/cliextensions` en Linux y macOS y `%USERPROFILE%\.azure\cliextensions` en Windows.

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

Nº Las extensiones deben ser paquetes individuales que no confían entre sí. Esto es porque la CLI no ofrece ninguna garantía sobre cuándo se cargan las extensiones, por lo que no se puede garantizar que las dependencias se cumplan. La instalación de una extensión instala solo esa extensión y debe continuar funcionando aunque elimine otras extensiones.

### <a name="are-extensions-updated-along-with-the-cli"></a>¿Las extensiones se actualizan junto con la CLI?

Nº Las extensiones deben actualizarse por separado, tal y como se describe en la sección [Actualización de extensiones](#updating-extensions).
