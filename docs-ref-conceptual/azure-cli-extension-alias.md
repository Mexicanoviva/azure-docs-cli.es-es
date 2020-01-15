---
title: Extensión alias de la CLI de Azure
description: Cómo usar la extensión alias de la CLI de Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cc6192c3e78f7bc895ed8f4c2f640aa1bf0e883c
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913661"
---
# <a name="the-azure-cli-alias-extension"></a>Extensión alias de la CLI de Azure

La extensión alias permite a los usuarios definir comandos personalizados para la CLI de Azure mediante comandos existentes. Los alias ayudan a simplificar el flujo de trabajo gracias a los accesos directos. Como los alias se basan en el motor de plantillas Jinja2, ofrecen incluso un procesamiento avanzado de los argumentos.

> [!NOTE]
> La extensión alias está en versión preliminar pública. Las características y el formato del archivo de configuración pueden cambiar.

## <a name="install-the-alias-extension"></a>Instalar la extensión alias

La versión mínima necesaria de la CLI de Azure para usar la extensión alias es **2.0.28**. Para comprobar la versión de la CLI, ejecute `az --version`. Si tiene que actualizar la instalación, siga las instrucciones de [Instalación de la CLI de Azure](./install-azure-cli.md).

Instale la extensión con el comando [az extension add](/cli/azure/extension#az-extension-add).

```azurecli-interactive
az extension add --name alias
```

Compruebe la instalación de la extensión con [az extension list](/cli/azure/extension#az-extension-list). Si la extensión alias se instaló correctamente, se muestra en la salida del comando.

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a>Mantener actualizada la extensión

La extensión alias se encuentra en desarrollo activo y se publican nuevas versiones con regularidad. No se instalan nuevas versiones al actualizar la CLI. Instale las actualizaciones de la extensión con [az extension update](/cli/azure/extension#az-extension-update).

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a>Administración de alias de la CLI de Azure

La extensión de alias permite crear y administrar alias para otros comandos de la CLI. Para ver todos los comandos disponibles y los detalles de los parámetros, ejecute el comando de alias con `--help`.

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a>Crear comandos de alias sencillos

Un uso de los alias es acortar los nombres de los comandos o de los grupos de comandos existentes. Por ejemplo, puede acortar el grupo de comandos `group` a `rg` y el comando `list` a `ls`.

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

Ahora puede usar estos alias recién definidos en cualquier lugar donde usaría su definición.

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

No incluya `az` como parte del comando.

Los alias también pueden ser métodos abreviados para comandos completos. En el ejemplo siguiente, se enumeram los grupos de recursos disponibles y su ubicación en la tabla de salida:

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

Ahora, `ls-groups` se puede ejecutar como cualquier otro comando de la CLI.

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a>Crear un comando de alias con argumentos

También puede agregar argumentos posicionales a un comando de alias; para ello, inclúyalos como `{{ arg_name }}` en el nombre de alias. El espacio en blanco entre las llaves es obligatorio.

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

El alias de ejemplo siguiente muestra cómo usar argumentos posicionales para obtener la dirección IP pública de una máquina virtual.

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

Al ejecutar este comando, asigne valores a los argumentos posicionales.

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

También puede usar variables de entorno en los comandos de alias, que se evalúan en tiempo de ejecución. En el ejemplo siguiente, se agrega el alias `create-rg`, que crea un grupo de recursos en `eastus` y agrega una etiqueta `owner`. A esta etiqueta se le asigna el valor de la variable de entorno local `USER`.

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

Para registrar las variables de entorno en el comando del alias, se debe agregar un carácter de escape al signo de dólar `$`.

## <a name="process-arguments-using-jinja2-templates"></a>Procesar argumentos mediante plantillas de Jinja2

La sustitución de argumentos en la extensión de alias la realiza [Jinja2](http://jinja.pocoo.org/docs/2.10/). Las plantillas de Jinja2 permiten manipular los argumentos.

Con las plantillas de Jinja2, puede escribir alias que tomen tipos de argumentos diferentes que los del comando subyacente. Por ejemplo, puede crear un alias que tome una dirección URL de almacenamiento. Después, se analiza esta dirección URL para pasar el nombre de la cuenta y el contenedor al comando de almacenamiento.

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

Para más información sobre el motor de plantillas Jinja2, consulte [la documentación de Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).

## <a name="alias-configuration-file"></a>Archivo de configuración de alias

Otra manera de crear y modificar alias es modificar el archivo de configuración de alias. Las definiciones de los comandos de alias se escriben en un archivo de configuración, ubicado en `$AZURE_USER_CONFIG/alias`. El valor predeterminado de `AZURE_USER_CONFIG` es `$HOME/.azure` en Linux y macOS, y `%USERPROFILE%\.azure` en Windows. El archivo de configuración de alias se escribe en el formato de archivo de configuración INI. El formato de los comandos de alias es:

```ini
[alias_name]
command = invoked_commands
```

Para los alias que tienen argumentos de posición, el formato de los comandos de alias es:

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a>Creación de un comando de alias con argumentos mediante el archivo de configuración de alias

El ejemplo siguiente muestra un alias para un comando con argumentos. Este comando obtiene la dirección IP pública de una máquina virtual. Los comandos de alias deben estar todos en una sola línea y usar todos los argumentos en el nombre de alias.

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a>Desinstalar la extensión alias

Para desinstalar la extensión, use el comando [az extension remove](/cli/azure/extension#az-extension-remove).

```azurecli-interactive
az extension remove --name alias
```

Si desinstala debido a un error u otros problemas con la extensión, [abra un problema en GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que podamos proporcionar una corrección.
