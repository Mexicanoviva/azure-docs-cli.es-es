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
# <a name="the-azure-cli-alias-extension"></a><span data-ttu-id="48a62-103">Extensión alias de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="48a62-103">The Azure CLI alias extension</span></span>

<span data-ttu-id="48a62-104">La extensión alias permite a los usuarios definir comandos personalizados para la CLI de Azure mediante comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="48a62-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="48a62-105">Los alias ayudan a simplificar el flujo de trabajo gracias a los accesos directos.</span><span class="sxs-lookup"><span data-stu-id="48a62-105">Aliases help keep your workflow simple by allowing shortcuts.</span></span> <span data-ttu-id="48a62-106">Como los alias se basan en el motor de plantillas Jinja2, ofrecen incluso un procesamiento avanzado de los argumentos.</span><span class="sxs-lookup"><span data-stu-id="48a62-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="48a62-107">La extensión alias está en versión preliminar pública.</span><span class="sxs-lookup"><span data-stu-id="48a62-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="48a62-108">Las características y el formato del archivo de configuración pueden cambiar.</span><span class="sxs-lookup"><span data-stu-id="48a62-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="48a62-109">Instalar la extensión alias</span><span class="sxs-lookup"><span data-stu-id="48a62-109">Install the alias extension</span></span>

<span data-ttu-id="48a62-110">La versión mínima necesaria de la CLI de Azure para usar la extensión alias es **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="48a62-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="48a62-111">Para comprobar la versión de la CLI, ejecute `az --version`.</span><span class="sxs-lookup"><span data-stu-id="48a62-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="48a62-112">Si tiene que actualizar la instalación, siga las instrucciones de [Instalación de la CLI de Azure](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="48a62-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI](./install-azure-cli.md).</span></span>

<span data-ttu-id="48a62-113">Instale la extensión con el comando [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="48a62-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli-interactive
az extension add --name alias
```

<span data-ttu-id="48a62-114">Compruebe la instalación de la extensión con [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="48a62-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="48a62-115">Si la extensión alias se instaló correctamente, se muestra en la salida del comando.</span><span class="sxs-lookup"><span data-stu-id="48a62-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="48a62-116">Mantener actualizada la extensión</span><span class="sxs-lookup"><span data-stu-id="48a62-116">Keep the extension up-to-date</span></span>

<span data-ttu-id="48a62-117">La extensión alias se encuentra en desarrollo activo y se publican nuevas versiones con regularidad.</span><span class="sxs-lookup"><span data-stu-id="48a62-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="48a62-118">No se instalan nuevas versiones al actualizar la CLI.</span><span class="sxs-lookup"><span data-stu-id="48a62-118">New versions aren't installed when you update the CLI.</span></span> <span data-ttu-id="48a62-119">Instale las actualizaciones de la extensión con [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="48a62-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="48a62-120">Administración de alias de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="48a62-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="48a62-121">La extensión de alias permite crear y administrar alias para otros comandos de la CLI.</span><span class="sxs-lookup"><span data-stu-id="48a62-121">The alias extension lets you create and manage aliases for other CLI commands.</span></span> <span data-ttu-id="48a62-122">Para ver todos los comandos disponibles y los detalles de los parámetros, ejecute el comando de alias con `--help`.</span><span class="sxs-lookup"><span data-stu-id="48a62-122">To view all the available commands and parameter details, run the alias command with `--help`.</span></span>

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a><span data-ttu-id="48a62-123">Crear comandos de alias sencillos</span><span class="sxs-lookup"><span data-stu-id="48a62-123">Create simple alias commands</span></span>

<span data-ttu-id="48a62-124">Un uso de los alias es acortar los nombres de los comandos o de los grupos de comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="48a62-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="48a62-125">Por ejemplo, puede acortar el grupo de comandos `group` a `rg` y el comando `list` a `ls`.</span><span class="sxs-lookup"><span data-stu-id="48a62-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="48a62-126">Ahora puede usar estos alias recién definidos en cualquier lugar donde usaría su definición.</span><span class="sxs-lookup"><span data-stu-id="48a62-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="48a62-127">No incluya `az` como parte del comando.</span><span class="sxs-lookup"><span data-stu-id="48a62-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="48a62-128">Los alias también pueden ser métodos abreviados para comandos completos.</span><span class="sxs-lookup"><span data-stu-id="48a62-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="48a62-129">En el ejemplo siguiente, se enumeram los grupos de recursos disponibles y su ubicación en la tabla de salida:</span><span class="sxs-lookup"><span data-stu-id="48a62-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="48a62-130">Ahora, `ls-groups` se puede ejecutar como cualquier otro comando de la CLI.</span><span class="sxs-lookup"><span data-stu-id="48a62-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="48a62-131">Crear un comando de alias con argumentos</span><span class="sxs-lookup"><span data-stu-id="48a62-131">Create an alias command with arguments</span></span>

<span data-ttu-id="48a62-132">También puede agregar argumentos posicionales a un comando de alias; para ello, inclúyalos como `{{ arg_name }}` en el nombre de alias.</span><span class="sxs-lookup"><span data-stu-id="48a62-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="48a62-133">El espacio en blanco entre las llaves es obligatorio.</span><span class="sxs-lookup"><span data-stu-id="48a62-133">The whitespace inside the braces is required.</span></span>

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="48a62-134">El alias de ejemplo siguiente muestra cómo usar argumentos posicionales para obtener la dirección IP pública de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="48a62-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="48a62-135">Al ejecutar este comando, asigne valores a los argumentos posicionales.</span><span class="sxs-lookup"><span data-stu-id="48a62-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="48a62-136">También puede usar variables de entorno en los comandos de alias, que se evalúan en tiempo de ejecución.</span><span class="sxs-lookup"><span data-stu-id="48a62-136">You can also use environment variables in aliased commands, which are evaluated at runtime.</span></span> <span data-ttu-id="48a62-137">En el ejemplo siguiente, se agrega el alias `create-rg`, que crea un grupo de recursos en `eastus` y agrega una etiqueta `owner`.</span><span class="sxs-lookup"><span data-stu-id="48a62-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="48a62-138">A esta etiqueta se le asigna el valor de la variable de entorno local `USER`.</span><span class="sxs-lookup"><span data-stu-id="48a62-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="48a62-139">Para registrar las variables de entorno en el comando del alias, se debe agregar un carácter de escape al signo de dólar `$`.</span><span class="sxs-lookup"><span data-stu-id="48a62-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="48a62-140">Procesar argumentos mediante plantillas de Jinja2</span><span class="sxs-lookup"><span data-stu-id="48a62-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="48a62-141">La sustitución de argumentos en la extensión de alias la realiza [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span><span class="sxs-lookup"><span data-stu-id="48a62-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span></span> <span data-ttu-id="48a62-142">Las plantillas de Jinja2 permiten manipular los argumentos.</span><span class="sxs-lookup"><span data-stu-id="48a62-142">Jinja2 templates allow for manipulating the arguments.</span></span>

<span data-ttu-id="48a62-143">Con las plantillas de Jinja2, puede escribir alias que tomen tipos de argumentos diferentes que los del comando subyacente.</span><span class="sxs-lookup"><span data-stu-id="48a62-143">With Jinja2 templates, you can write aliases that take different types of arguments than the underlying command.</span></span> <span data-ttu-id="48a62-144">Por ejemplo, puede crear un alias que tome una dirección URL de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="48a62-144">For example, you can make an alias that takes a storage URL.</span></span> <span data-ttu-id="48a62-145">Después, se analiza esta dirección URL para pasar el nombre de la cuenta y el contenedor al comando de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="48a62-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="48a62-146">Para más información sobre el motor de plantillas Jinja2, consulte [la documentación de Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="48a62-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="alias-configuration-file"></a><span data-ttu-id="48a62-147">Archivo de configuración de alias</span><span class="sxs-lookup"><span data-stu-id="48a62-147">Alias configuration file</span></span>

<span data-ttu-id="48a62-148">Otra manera de crear y modificar alias es modificar el archivo de configuración de alias.</span><span class="sxs-lookup"><span data-stu-id="48a62-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="48a62-149">Las definiciones de los comandos de alias se escriben en un archivo de configuración, ubicado en `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="48a62-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="48a62-150">El valor predeterminado de `AZURE_USER_CONFIG` es `$HOME/.azure` en Linux y macOS, y `%USERPROFILE%\.azure` en Windows.</span><span class="sxs-lookup"><span data-stu-id="48a62-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="48a62-151">El archivo de configuración de alias se escribe en el formato de archivo de configuración INI.</span><span class="sxs-lookup"><span data-stu-id="48a62-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="48a62-152">El formato de los comandos de alias es:</span><span class="sxs-lookup"><span data-stu-id="48a62-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="48a62-153">Para los alias que tienen argumentos de posición, el formato de los comandos de alias es:</span><span class="sxs-lookup"><span data-stu-id="48a62-153">For aliases that have positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="48a62-154">Creación de un comando de alias con argumentos mediante el archivo de configuración de alias</span><span class="sxs-lookup"><span data-stu-id="48a62-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="48a62-155">El ejemplo siguiente muestra un alias para un comando con argumentos.</span><span class="sxs-lookup"><span data-stu-id="48a62-155">The next example shows an alias for a command with arguments.</span></span> <span data-ttu-id="48a62-156">Este comando obtiene la dirección IP pública de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="48a62-156">This command gets the public IP address for a VM.</span></span> <span data-ttu-id="48a62-157">Los comandos de alias deben estar todos en una sola línea y usar todos los argumentos en el nombre de alias.</span><span class="sxs-lookup"><span data-stu-id="48a62-157">Aliased commands must all be on a single line, and use all of the arguments in the alias name.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="48a62-158">Desinstalar la extensión alias</span><span class="sxs-lookup"><span data-stu-id="48a62-158">Uninstall the alias extension</span></span>

<span data-ttu-id="48a62-159">Para desinstalar la extensión, use el comando [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="48a62-159">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli-interactive
az extension remove --name alias
```

<span data-ttu-id="48a62-160">Si desinstala debido a un error u otros problemas con la extensión, [abra un problema en GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que podamos proporcionar una corrección.</span><span class="sxs-lookup"><span data-stu-id="48a62-160">If you uninstalled because a bug or other problem with the extension, [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
