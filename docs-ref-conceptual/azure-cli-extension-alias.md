---
title: Extensión alias de la CLI de Azure 2.0
description: Cómo usar la extensión alias de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 39996693d6b796c2d9a45cd909121829f00291a8
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/18/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="7cec0-103">Extensión alias de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="7cec0-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="7cec0-104">La extensión alias permite a los usuarios definir comandos personalizados para la CLI de Azure mediante comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="7cec0-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="7cec0-105">Los alias son métodos abreviados que ayudan a mantener los flujos de trabajo concisos y sencillos, y permiten usar argumentos posicionales.</span><span class="sxs-lookup"><span data-stu-id="7cec0-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="7cec0-106">Como los alias se basan en el motor de plantillas Jinja2, ofrecen incluso un procesamiento avanzado de los argumentos.</span><span class="sxs-lookup"><span data-stu-id="7cec0-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="7cec0-107">La extensión alias está en versión preliminar pública.</span><span class="sxs-lookup"><span data-stu-id="7cec0-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="7cec0-108">Las características y el formato del archivo de configuración pueden cambiar.</span><span class="sxs-lookup"><span data-stu-id="7cec0-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="7cec0-109">Instalar la extensión alias</span><span class="sxs-lookup"><span data-stu-id="7cec0-109">Install the alias extension</span></span>

<span data-ttu-id="7cec0-110">La versión mínima necesaria de la CLI de Azure para usar la extensión alias es **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="7cec0-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="7cec0-111">Para comprobar la versión de la CLI, ejecute `az --version`.</span><span class="sxs-lookup"><span data-stu-id="7cec0-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="7cec0-112">Si tiene que actualizar la instalación, siga las instrucciones de [Instalación de la CLI de Azure 2.0](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7cec0-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="7cec0-113">Instale la extensión con el comando [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="7cec0-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli-interactive
az extension add --name alias
```

<span data-ttu-id="7cec0-114">Compruebe la instalación de la extensión con [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="7cec0-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="7cec0-115">Si la extensión alias se instaló correctamente, se muestra en la salida del comando.</span><span class="sxs-lookup"><span data-stu-id="7cec0-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="7cec0-116">Mantener actualizada la extensión</span><span class="sxs-lookup"><span data-stu-id="7cec0-116">Keep the extension up to date</span></span>

<span data-ttu-id="7cec0-117">La extensión alias se encuentra en desarrollo activo y se publican nuevas versiones con regularidad.</span><span class="sxs-lookup"><span data-stu-id="7cec0-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="7cec0-118">Las nuevas versiones no se instalan automáticamente cada vez que actualice la CLI.</span><span class="sxs-lookup"><span data-stu-id="7cec0-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="7cec0-119">Instale las actualizaciones de la extensión con [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="7cec0-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="7cec0-120">Administración de alias de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7cec0-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="7cec0-121">La extensión de alias proporciona comandos cómodos y familiares para administrar los alias.</span><span class="sxs-lookup"><span data-stu-id="7cec0-121">The alias extension provides convenient and familiar commands to manage aliases.</span></span> <span data-ttu-id="7cec0-122">Para ver todos los comandos disponibles y los detalles de los parámetros, invoque el comando de alias con `--help`.</span><span class="sxs-lookup"><span data-stu-id="7cec0-122">To view all the available commands and parameter details, invoke the alias command with `--help`.</span></span>

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a><span data-ttu-id="7cec0-123">Crear comandos de alias sencillos</span><span class="sxs-lookup"><span data-stu-id="7cec0-123">Create simple alias commands</span></span>

<span data-ttu-id="7cec0-124">Un uso de los alias es acortar los nombres de los comandos o de los grupos de comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="7cec0-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="7cec0-125">Por ejemplo, puede acortar el grupo de comandos `group` a `rg` y el comando `list` a `ls`.</span><span class="sxs-lookup"><span data-stu-id="7cec0-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="7cec0-126">Ahora puede usar estos alias recién definidos en cualquier lugar donde usaría su definición.</span><span class="sxs-lookup"><span data-stu-id="7cec0-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="7cec0-127">No incluya `az` como parte del comando.</span><span class="sxs-lookup"><span data-stu-id="7cec0-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="7cec0-128">Los alias también pueden ser métodos abreviados para comandos completos.</span><span class="sxs-lookup"><span data-stu-id="7cec0-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="7cec0-129">En el ejemplo siguiente, se enumeram los grupos de recursos disponibles y su ubicación en la tabla de salida:</span><span class="sxs-lookup"><span data-stu-id="7cec0-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="7cec0-130">Ahora, `ls-groups` se puede ejecutar como cualquier otro comando de la CLI.</span><span class="sxs-lookup"><span data-stu-id="7cec0-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="7cec0-131">Crear un comando de alias con argumentos</span><span class="sxs-lookup"><span data-stu-id="7cec0-131">Create an alias command with arguments</span></span>

<span data-ttu-id="7cec0-132">También puede agregar argumentos posicionales a un comando de alias; para ello, inclúyalos como `{{ arg_name }}` en el nombre de alias.</span><span class="sxs-lookup"><span data-stu-id="7cec0-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="7cec0-133">El espacio en blanco entre las llaves es obligatorio.</span><span class="sxs-lookup"><span data-stu-id="7cec0-133">The whitespace inside the braces is required.</span></span>

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="7cec0-134">El alias de ejemplo siguiente muestra cómo usar argumentos posicionales para obtener la dirección IP pública de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="7cec0-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="7cec0-135">Al ejecutar este comando, asigne valores a los argumentos posicionales.</span><span class="sxs-lookup"><span data-stu-id="7cec0-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="7cec0-136">También puede usar variables de entorno en comandos invocados por alias, que se evalúan en tiempo de ejecución.</span><span class="sxs-lookup"><span data-stu-id="7cec0-136">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="7cec0-137">En el ejemplo siguiente, se agrega el alias `create-rg`, que crea un grupo de recursos en `eastus` y agrega una etiqueta `owner`.</span><span class="sxs-lookup"><span data-stu-id="7cec0-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="7cec0-138">A esta etiqueta se le asigna el valor de la variable de entorno local `USER`.</span><span class="sxs-lookup"><span data-stu-id="7cec0-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="7cec0-139">Para registrar las variables de entorno en el comando del alias, se debe agregar un carácter de escape al signo de dólar `$`.</span><span class="sxs-lookup"><span data-stu-id="7cec0-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="7cec0-140">Procesar argumentos mediante plantillas de Jinja2</span><span class="sxs-lookup"><span data-stu-id="7cec0-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="7cec0-141">La sustitución de argumentos en la extensión alias se realiza mediante [Jinja2](http://jinja.pocoo.org/docs/2.10/), lo que le proporciona acceso completo a las funcionalidades del motor de plantillas Jinja2.</span><span class="sxs-lookup"><span data-stu-id="7cec0-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="7cec0-142">Las plantillas permiten realizar acciones como la extracción de datos y la sustitución en cadenas.</span><span class="sxs-lookup"><span data-stu-id="7cec0-142">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="7cec0-143">Con las plantillas de Jinja2, puede escribir alias que tomen tipos de argumentos diferentes del comando subyacente.</span><span class="sxs-lookup"><span data-stu-id="7cec0-143">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="7cec0-144">Por ejemplo, puede crear un alias que tome una dirección URL de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="7cec0-144">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="7cec0-145">Después, se analiza esta dirección URL para pasar el nombre de la cuenta y el contenedor al comando de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="7cec0-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="7cec0-146">Para más información sobre el motor de plantillas Jinja2, consulte [la documentación de Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="7cec0-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="alias-configuration-file"></a><span data-ttu-id="7cec0-147">Archivo de configuración de alias</span><span class="sxs-lookup"><span data-stu-id="7cec0-147">Alias configuration file</span></span>

<span data-ttu-id="7cec0-148">Otra manera de crear y modificar alias es modificar el archivo de configuración de alias.</span><span class="sxs-lookup"><span data-stu-id="7cec0-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="7cec0-149">Las definiciones de los comandos de alias se escriben en un archivo de configuración, ubicado en `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="7cec0-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="7cec0-150">El valor predeterminado de `AZURE_USER_CONFIG` es `$HOME/.azure` en Linux y macOS, y `%USERPROFILE%\.azure` en Windows.</span><span class="sxs-lookup"><span data-stu-id="7cec0-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="7cec0-151">El archivo de configuración de alias se escribe en el formato de archivo de configuración INI.</span><span class="sxs-lookup"><span data-stu-id="7cec0-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="7cec0-152">El formato de los comandos de alias es:</span><span class="sxs-lookup"><span data-stu-id="7cec0-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="7cec0-153">Para los alias que contienen argumentos de posición, el formato de los comandos de alias es:</span><span class="sxs-lookup"><span data-stu-id="7cec0-153">For aliases that contain positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="7cec0-154">Creación de un comando de alias con argumentos mediante el archivo de configuración de alias</span><span class="sxs-lookup"><span data-stu-id="7cec0-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="7cec0-155">A continuación se muestra un archivo de configuración de alias que contiene un comando de alias de ejemplo con argumentos, que obtiene la dirección IP pública de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="7cec0-155">Below is an alias configuration file that contains an example alias command with arguments, which gets the public IP address for a VM.</span></span> <span data-ttu-id="7cec0-156">Asegúrese de que el comando invocado está en una sola línea y que contiene los mismos argumentos que se definen en el alias.</span><span class="sxs-lookup"><span data-stu-id="7cec0-156">Ensure that the invoked command is in a single line, and contains the same arguments defined in the alias.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="7cec0-157">Desinstalar la extensión alias</span><span class="sxs-lookup"><span data-stu-id="7cec0-157">Uninstall the alias extension</span></span>

<span data-ttu-id="7cec0-158">Para desinstalar la extensión, use el comando [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="7cec0-158">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli-interactive
az extension remove --name alias
```

<span data-ttu-id="7cec0-159">Si desinstala debido a un error u otro problema con la extensión, [abra un problema en GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que podamos proporcionar una corrección.</span><span class="sxs-lookup"><span data-stu-id="7cec0-159">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
