---
title: Extensión alias de la CLI de Azure 2.0
description: Cómo usar la extensión alias de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 40a43f5013a5dd0d7bb65b21140bb4fc82769267
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2018
---
# <a name="the-azure-cli-20-alias-extension"></a>Extensión alias de la CLI de Azure 2.0

La extensión alias permite a los usuarios definir comandos personalizados para la CLI de Azure mediante comandos existentes. Los alias son métodos abreviados que ayudan a mantener los flujos de trabajo concisos y sencillos, y permiten usar argumentos posicionales. Como los alias se basan en el motor de plantillas Jinja2, ofrecen incluso un procesamiento avanzado de los argumentos.

> [!NOTE]
> La extensión alias está en versión preliminar pública. Las características y el formato del archivo de configuración pueden cambiar.

## <a name="install-the-alias-extension"></a>Instalar la extensión alias

La versión mínima necesaria de la CLI de Azure para usar la extensión alias es **2.0.28**. Para comprobar la versión de la CLI, ejecute `az --version`. Si tiene que actualizar la instalación, siga las instrucciones de [Instalación de la CLI de Azure 2.0](./install-azure-cli.md).

Instale la extensión con el comando [az extension add](/cli/azure/extension#az-extension-add).

```azurecli
az extension add --name alias
```

Compruebe la instalación de la extensión con [az extension list](/cli/azure/extension#az-extension-list). Si la extensión alias se instaló correctamente, se muestra en la salida del comando.

```azurecli
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```


## <a name="keep-the-extension-up-to-date"></a>Mantener actualizada la extensión

La extensión alias se encuentra en desarrollo activo y se publican nuevas versiones con regularidad. Las nuevas versiones no se instalan automáticamente cada vez que actualice la CLI. Instale las actualizaciones de la extensión con [az extension update](/cli/azure/extension#az-extension-update).

```azurecli
az extension update --name alias
```


## <a name="manage-aliases-for-the-azure-cli"></a>Administración de alias de la CLI de Azure

La extensión de alias proporciona comandos cómodos y familiares para administrar los alias. Para ver todos los comandos disponibles y los detalles de los parámetros, invoque el comando de alias con `--help`.

```azurecli
az alias --help
```


## <a name="create-simple-alias-commands"></a>Crear comandos de alias sencillos

Un uso de los alias es acortar los nombres de los comandos o de los grupos de comandos existentes. Por ejemplo, puede acortar el grupo de comandos `group` a `rg` y el comando `list` a `ls`.

```azurecli
az alias create --name rg --command group
az alias create --name ls --command list
```

Ahora puede usar estos alias recién definidos en cualquier lugar donde usaría su definición.

```azurecli
az rg list
az rg ls
az vm ls
```

No incluya `az` como parte del comando.

Los alias también pueden ser métodos abreviados para comandos completos. En el ejemplo siguiente, se enumeram los grupos de recursos disponibles y su ubicación en la tabla de salida:

```azurecli
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

Ahora, `ls-groups` se puede ejecutar como cualquier otro comando de la CLI.

```azurecli
az ls-groups
```


## <a name="create-an-alias-command-with-arguments"></a>Crear un comando de alias con argumentos

También puede agregar argumentos posicionales a un comando de alias; para ello, inclúyalos como `{{ arg_name }}` en el nombre de alias. El espacio en blanco entre las llaves es obligatorio.

```azurecli
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

El alias de ejemplo siguiente muestra cómo usar argumentos posicionales para obtener la dirección IP pública de una máquina virtual.

```azurecli
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

Al ejecutar este comando, asigne valores a los argumentos posicionales.

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

También puede usar variables de entorno en comandos invocados por alias, que se evalúan en tiempo de ejecución. En el ejemplo siguiente, se agrega el alias `create-rg`, que crea un grupo de recursos en `eastus` y agrega una etiqueta `owner`. A esta etiqueta se le asigna el valor de la variable de entorno local `USER`.

```azurecli
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

Para registrar las variables de entorno en el comando del alias, se debe agregar un carácter de escape al signo de dólar `$`.


## <a name="process-arguments-using-jinja2-templates"></a>Procesar argumentos mediante plantillas de Jinja2

La sustitución de argumentos en la extensión alias se realiza mediante [Jinja2](http://jinja.pocoo.org/docs/2.10/), lo que le proporciona acceso completo a las funcionalidades del motor de plantillas Jinja2. Las plantillas permiten realizar acciones como la extracción de datos y la sustitución en cadenas.

Con las plantillas de Jinja2, puede escribir alias que tomen tipos de argumentos diferentes del comando subyacente. Por ejemplo, puede crear un alias que tome una dirección URL de almacenamiento. Después, se analiza esta dirección URL para pasar el nombre de la cuenta y el contenedor al comando de almacenamiento.

```azurecli
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

Para los alias que contienen argumentos de posición, el formato de los comandos de alias es:

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```


## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a>Creación de un comando de alias con argumentos mediante el archivo de configuración de alias

A continuación se muestra un archivo de configuración de alias que contiene un comando de alias de ejemplo con argumentos, que obtiene la dirección IP pública de una máquina virtual. Asegúrese de que el comando invocado está en una sola línea y que contiene los mismos argumentos que se definen en el alias.

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```


## <a name="uninstall-the-alias-extension"></a>Desinstalar la extensión alias

Para desinstalar la extensión, use el comando [az extension remove](/cli/azure/extension#az-extension-remove).

```azurecli
az extension remove --name alias
```

Si desinstala debido a un error u otro problema con la extensión, [abra un problema en GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que podamos proporcionar una corrección.
