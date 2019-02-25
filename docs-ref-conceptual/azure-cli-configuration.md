---
title: Opciones de configuración de la CLI de Azure
description: Cómo configurar la CLI de Azure
keywords: CLI de Azure, configuración, valores, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d23f576a1f7447ffab0606b4554a81ae5c536e85
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158487"
---
# <a name="azure-cli-configuration"></a>Configuración de la CLI de Azure

La CLI de Azure permite que el usuario configure opciones tales como el registro, la recopilación de datos y los valores de argumento predeterminados.
La CLI ofrece un práctico comando para administrar algunos valores predeterminados, `az configure`. Otros valores se pueden establecer en un archivo de configuración o con variables de entorno.

Los valores de configuración usados por la CLI se evalúan según la siguiente prioridad, con mayor prioridad en los elementos superiores de la lista.

1. Parámetros de línea de comandos
2. Variables de entorno
3. Valores en el archivo de configuración o establecidos con `az configure`

## <a name="cli-configuration-with-az-configure"></a>Configuración de la CLI con az configure

Los valores predeterminados para la CLI se establecen con el comando [az configure](/cli/azure/reference-index#az-configure).
Este comando toma un argumento, `--defaults`, que es una lista de pares `key=value` separada por espacios. La CLI utiliza los valores proporcionados en lugar de los argumentos necesarios.

La tabla siguiente contiene una lista de las claves de configuración disponibles.

| NOMBRE | DESCRIPCIÓN |
|------|-------------|
| group | El grupo de recursos predeterminado que se utilizará para todos los comandos. |
| location | La ubicación predeterminada que se utilizará para todos los comandos. |
| web | El nombre de la aplicación predeterminada que se usará para los comandos `az webapp`. |
| vm | El nombre de la máquina virtual predeterminada que se usará para los comandos `az vm`. |
| vmss | Nombre del conjunto de escalado de máquinas virtuales (VMSS) predeterminado que se usará para los comandos `az vmss`. |
| acr | El nombre del registro de contenedor predeterminado que se usará para los comandos `az acr`. |

Por ejemplo, aquí se muestra cómo se establecería el grupo de recursos y la ubicación de forma predeterminada para todos los comandos.

```azurecli-interactive
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>Archivo de configuración de la CLI

El archivo de configuración de la CLI contiene otros valores que se usan para administrar el comportamiento de la CLI. El archivo de configuración se encuentra en `$AZURE_CONFIG_DIR/config`. El valor predeterminado de `AZURE_CONFIG_DIR` es `$HOME/.azure` en Linux y macOS y `%USERPROFILE%\.azure` en Windows.

Los archivos de configuración se escriben en el formato de archivos INI. Este formato de archivo se define mediante encabezados de sección, seguidos de una lista de pares clave-valor.

* Los encabezados de sección se escriben como `[section-name]`. Los nombres de sección distinguen entre mayúsculas y minúsculas.
* Las entradas se escriben como `key=value`. Los nombres de clave no distinguen mayúsculas de minúsculas.
* Los comentarios son cualquier línea que comience por un `#` o `;`. No se permiten comentarios en línea.

Los valores booleanos no distinguen mayúsculas de minúsculas y se representan por los valores siguientes.

* __True__: 1, yes, true, on
* __False__: 0, no, false, off

Este es un ejemplo de un archivo de configuración de la CLI que deshabilita los avisos de confirmación y establece el registro en el directorio `/var/log/azure`.

```ini
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

Consulte la siguiente sección para obtener los detalles de todos los valores de configuración disponibles y su significado. Para obtener los detalles completos sobre el formato de archivos INI, consulte la [documentación de Python sobre INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).

## <a name="cli-configuration-values-and-environment-variables"></a>Valores de configuración de la CLI y variables de entorno

La tabla siguiente contiene todos los nombres de las secciones y de las opciones que se pueden utilizar en un archivo de configuración. Las variables de entorno correspondientes se establecen como `AZURE_{section}_{name}`, todo en mayúsculas. Por ejemplo, el valor predeterminado `storage_account` de `batchai` se establece en la variable `AZURE_BATCHAI_STORAGE_ACCOUNT`.

Al proporcionar un valor predeterminado, ningún comando necesita ya ese argumento. En su lugar, se usa el valor predeterminado.

| Sección | NOMBRE      | Type | DESCRIPCIÓN|
|---------|-----------|------|------------|
| __core__ | output | string | El formato de salida predeterminado. Puede ser `json`, `jsonc`, `tsv` o `table`. |
| | disable\_confirm\_prompt | boolean | Activa o desactiva los mensajes de confirmación. |
| | collect\_telemetry | boolean | Permite que Microsoft recopile datos anónimos sobre el uso de la CLI. Para obtener información de privacidad, consulte los [Términos de uso de la CLI de Azure](http://aka.ms/AzureCliLegal). |
| __logging__ | enable\_log\_file | boolean | Activar o desactivar el registro. |
| | log\_dir | string | El directorio en el que se escribe el registro. De manera predeterminada, este valor es `${AZURE_CONFIG_DIR}/logs`. |
| __storage__ | connection\_string | string | La cadena de conexión predeterminada que se usará para los comandos `az storage`. |
| | account | string | El nombre de la cuenta predeterminada que se usará para los comandos `az storage`. |
| | key | string | La clave de la cuenta predeterminada que se usará para los comandos `az storage`. |
| | sas\_token | string | El token de SAS predeterminado que se usará para los comandos `az storage`. |
| __batchai__ | storage\_account | string | La cuenta de almacenamiento predeterminada que se usará para los comandos `az batchai`. |
| | storage\_key | string | La clave de almacenamiento predeterminada que se usará para los comandos `az batchai`. |
| __batch__ | account | string | El nombre de la cuenta de Azure Batch predeterminada que se usará para los comandos `az batch`. |
| | access\_key | string | La clave de acceso predeterminada que se usará para los comandos `az batch`. Solo se usa con autorización `aad`. |
| | punto de conexión | string | El punto de conexión predeterminado para los comandos `az batch`. |
| | auth\_mode | string | El modo de autorización que se usará para los comandos `az batch`. Puede ser `shared_key` o `aad`. |

> [!NOTE]
> Puede ver otros valores en el archivo de configuración, pero estos se administran directamente mediante comandos de la CLI, incluido `az configure`. Los que aparecen en la tabla anterior son los únicos valores que debe cambiar usted mismo.
