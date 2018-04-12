---
title: Opciones de configuración de la CLI de Azure
description: Cómo configurar la CLI de Azure 2.0
keywords: CLI de Azure, configuración, valores, Azure
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 12/13/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 7ef6175815014ac3f822e8c1038b4f5af8bba9dc
ms.sourcegitcommit: c9da729f4a42a839f13106f7589deaa0ca19cc4e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/06/2018
---
# <a name="azure-cli-20-configuration"></a>Configuración de la CLI de Azure 2.0

La CLI de Azure 2.0 permite que la configuración de usuario reemplace valores internos como la recopilación de datos y el registro, y proporciona opciones predeterminadas para algunos parámetros necesarios. La CLI ofrece un práctico comando para administrar algunos de estos valores, `az configure`, y se pueden establecer otros valores en un archivo de configuración o con variables de entorno.

Los valores de configuración usados por la CLI se evalúan según la siguiente prioridad, con mayor prioridad en los elementos superiores de la lista.

1. Parámetros de línea de comandos
2. Variables de entorno
3. Valores en el archivo de configuración o establecidos con `az configure`

## <a name="cli-configuration-with-az-configure"></a>Configuración de la CLI con az configure

Los valores predeterminados para la CLI se establecen con el comando [az configure](/cli/azure/reference-index#az-configure).
Este comando toma un argumento, `--defaults`, que es una lista de pares `key=value` separada por espacios. La CLI utiliza los valores proporcionados en lugar de los argumentos necesarios.

La siguiente es una lista de claves disponibles que puede usar.

| NOMBRE | DESCRIPCIÓN |
|------|-------------|
| group | El grupo de recursos predeterminado que se utilizará para todos los comandos. |
| location | La ubicación predeterminada que se utilizará para todos los comandos. |
| web | El nombre de la aplicación predeterminada que se usará para los comandos `az webapp`. |
| vm | El nombre de la máquina virtual predeterminada que se usará para los comandos `az vm`. |
| vmss | El nombre del VMSS predeterminado que se usará para los comandos `az vmss`. |
| acr | El nombre del registro de contenedor predeterminado que se usará para los comandos `az acr`. |
| acs | El nombre del servicio de contenedor predeterminado que se usará para los comandos `az acs`. |

Por ejemplo, aquí se muestra cómo se establecería el grupo de recursos y la ubicación de forma predeterminada para todos los comandos.

```azurecli
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>Archivo de configuración de la CLI

El archivo de configuración de la CLI contiene otros valores que se usan para administrar el comportamiento de la CLI. El archivo de configuración se encuentra en `$AZURE_CONFIG_DIR/config`. El valor predeterminado de `AZURE_CONFIG_DIR` es `$HOME/.azure` en Linux y macOS y `%USERPROFILE%\.azure` en Windows.

Los archivos de configuración se escriben en el formato de archivos INI. Estos archivos se componen de secciones que empiezan por un encabezado `[section-name]` seguido de una lista de entradas `key=value`. Los nombres de sección distinguen mayúsculas de minúsculas y los nombres de clave, no.
Los comentarios son cualquier línea que comience por un `#` o `;`. No se permiten comentarios en línea. Los valores booleanos no distinguen mayúsculas de minúsculas y se representan por los valores siguientes.

* __Verdadero__: 1, yes, true, on
* __Falso__: 0, no, false, off

Este es un ejemplo de un archivo de configuración de la CLI que deshabilita los mensajes de confirmación y establece el registro en el directorio `/var/log/azure`.

```
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

Consulte la siguiente sección para obtener los detalles de todos los valores de configuración disponibles y su significado. Para obtener los detalles completos sobre el formato de archivos INI, consulte la [documentación de Python sobre INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).

## <a name="cli-configuration-values-and-environment-variables"></a>Valores de configuración de la CLI y variables de entorno

La tabla siguiente contiene todos los nombres de las secciones y de las opciones que se pueden utilizar en un archivo de configuración. Las variables de entorno correspondientes se pueden establecer como `AZURE_{section}_{name}`, todo en mayúsculas. Por ejemplo, en la sección `batchai`, puede establecer el valor predeterminado de `storage_account` en la variable `AZURE_BATCHAI_STORAGE_ACCOUNT`.

Cualquier valor con un valor predeterminado disponible no necesita estar presente en los argumentos de la línea de comandos, incluso si es obligatorio.

| Sección | NOMBRE      | type | DESCRIPCIÓN|
|---------|-----------|------|------------|
| __core__ | output | string | El formato de salida predeterminado. Puede ser `json`, `jsonc`, `tsv` o `table`. |
| | disable\_confirm\_prompt | boolean | Activa o desactiva los mensajes de confirmación. |
| | collect\_telemetry | boolean | Permite que Microsoft recopile datos anónimos sobre el uso de la CLI. Para obtener información de privacidad, consulte los [Términos de uso de la CLI de Azure 2.0](http://aka.ms/AzureCliLegal). |
| __logging__ | enable\_log\_file | boolean | Activar o desactivar el registro. |
| | log\_dir | string | El directorio en el que se escribe el registro. De manera predeterminada, será `${AZURE_CONFIG_DIR}/logs`. |
| __storage__ | connection\_string | string | La cadena de conexión predeterminada que se usará para los comandos `az storage`. |
| | cuenta | string | El nombre de la cuenta predeterminada que se usará para los comandos `az storage`. |
| | key | string | La clave de la cuenta predeterminada que se usará para los comandos `az storage`. |
| | sas\_token | string | El token de SAS predeterminado que se usará para los comandos `az storage`. |
| __batchai__ | storage\_account | string | La cuenta de almacenamiento predeterminada que se usará para los comandos `az batchai`. |
| | storage\_key | string | La clave de almacenamiento predeterminada que se usará para los comandos `az batchai`. |
| __batch__ | cuenta | string | El nombre de la cuenta de Azure Batch predeterminada que se usará para los comandos `az batch`. |
| | access\_key | string | La clave de acceso predeterminada que se usará para los comandos `az batch`. Solo se usa con autorización `aad`. |
| | endpoint | string | El punto de conexión predeterminado para los comandos `az batch`. |
| | auth\_mode | string | El modo de autorización que se usará para los comandos `az batch`. Puede ser `shared_key` o `aad`. |

> [!NOTE]
> Puede ver otros valores en el archivo de configuración, pero estos se administran directamente mediante comandos de la CLI, incluido `az configure`. Los que aparecen en la tabla anterior son los únicos valores que debe cambiar usted mismo.
