---
title: Extensión alias de la CLI de Azure 2.0
description: Cómo usar la extensión alias de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e8419394bb221d2614e15171bd19dd76fd9cd773
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/28/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="f11d5-103">Extensión alias de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="f11d5-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="f11d5-104">La extensión alias permite a los usuarios definir comandos personalizados para la CLI de Azure mediante comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="f11d5-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="f11d5-105">Los alias son métodos abreviados que ayudan a mantener los flujos de trabajo concisos y sencillos, y permiten usar argumentos posicionales.</span><span class="sxs-lookup"><span data-stu-id="f11d5-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="f11d5-106">Como los alias se basan en el motor de plantillas Jinja2, ofrecen incluso un procesamiento avanzado de los argumentos.</span><span class="sxs-lookup"><span data-stu-id="f11d5-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="f11d5-107">La extensión alias está en versión preliminar pública.</span><span class="sxs-lookup"><span data-stu-id="f11d5-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="f11d5-108">Las características y el formato del archivo de configuración pueden cambiar.</span><span class="sxs-lookup"><span data-stu-id="f11d5-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="f11d5-109">Instalar la extensión alias</span><span class="sxs-lookup"><span data-stu-id="f11d5-109">Install the alias extension</span></span>

<span data-ttu-id="f11d5-110">La versión mínima necesaria de la CLI de Azure para usar la extensión alias es **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="f11d5-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="f11d5-111">Para comprobar la versión de la CLI, ejecute `az --version`.</span><span class="sxs-lookup"><span data-stu-id="f11d5-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="f11d5-112">Si tiene que actualizar la instalación, siga las instrucciones de [Instalación de la CLI de Azure 2.0](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f11d5-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="f11d5-113">Instale la extensión con el comando [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="f11d5-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli
az extension add --name alias
```

<span data-ttu-id="f11d5-114">Compruebe la instalación de la extensión con [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="f11d5-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="f11d5-115">Si la extensión alias se instaló correctamente, se muestra en la salida del comando.</span><span class="sxs-lookup"><span data-stu-id="f11d5-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli
az extension list --output table
```

```output
ExtensionType    Name                       Version
---------------  -------------------------  ---------
whl              alias                      0.2.0
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="f11d5-116">Mantener actualizada la extensión</span><span class="sxs-lookup"><span data-stu-id="f11d5-116">Keep the extension up to date</span></span>

<span data-ttu-id="f11d5-117">La extensión alias se encuentra en desarrollo activo y se publican nuevas versiones con regularidad.</span><span class="sxs-lookup"><span data-stu-id="f11d5-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="f11d5-118">Las nuevas versiones no se instalan automáticamente cada vez que actualice la CLI.</span><span class="sxs-lookup"><span data-stu-id="f11d5-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="f11d5-119">Instale las actualizaciones de la extensión con [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="f11d5-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name alias
```

## <a name="alias-commands-file-format"></a><span data-ttu-id="f11d5-120">Formato del archivo de comandos de alias</span><span class="sxs-lookup"><span data-stu-id="f11d5-120">Alias commands file format</span></span>

<span data-ttu-id="f11d5-121">Las definiciones de los comandos de alias se escriben en un archivo de configuración, ubicado en `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="f11d5-121">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="f11d5-122">El valor predeterminado de `AZURE_USER_CONFIG` es `$HOME/.azure` en Linux y macOS, y `%USERPROFILE%\.azure` en Windows.</span><span class="sxs-lookup"><span data-stu-id="f11d5-122">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="f11d5-123">El archivo de configuración de alias se escribe en el formato de archivo de configuración INI.</span><span class="sxs-lookup"><span data-stu-id="f11d5-123">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="f11d5-124">El formato general de los comandos de alias es:</span><span class="sxs-lookup"><span data-stu-id="f11d5-124">The general format for alias commands is:</span></span>

```
[command_name]
command = invoked_commands
```

<span data-ttu-id="f11d5-125">No incluya `az` como parte del comando.</span><span class="sxs-lookup"><span data-stu-id="f11d5-125">Don't include `az` as part of the command.</span></span>

## <a name="create-simple-alias-commands"></a><span data-ttu-id="f11d5-126">Crear comandos de alias sencillos</span><span class="sxs-lookup"><span data-stu-id="f11d5-126">Create simple alias commands</span></span>

<span data-ttu-id="f11d5-127">Un uso de los alias es acortar los nombres de los comandos o de los grupos de comandos existentes.</span><span class="sxs-lookup"><span data-stu-id="f11d5-127">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="f11d5-128">Por ejemplo, puede acortar el grupo de comandos `group` a `rg` y el comando `list` a `ls`.</span><span class="sxs-lookup"><span data-stu-id="f11d5-128">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```
[rg]
command = group

[ls]
command = list
```

<span data-ttu-id="f11d5-129">Ahora puede usar estos alias recién definidos en cualquier lugar donde usaría su definición.</span><span class="sxs-lookup"><span data-stu-id="f11d5-129">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="f11d5-130">Los alias también pueden ser métodos abreviados para comandos completos.</span><span class="sxs-lookup"><span data-stu-id="f11d5-130">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="f11d5-131">En el ejemplo siguiente, se enumeram los grupos de recursos disponibles y su ubicación en la tabla de salida:</span><span class="sxs-lookup"><span data-stu-id="f11d5-131">The next example lists available resource groups and their locations in table output:</span></span>

```
[ls-groups]
command = group list --query '[].{Name:name, Location:location}' --output table
```

<span data-ttu-id="f11d5-132">Ahora, `ls-groups` se puede ejecutar como cualquier otro comando de la CLI.</span><span class="sxs-lookup"><span data-stu-id="f11d5-132">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="f11d5-133">Crear un comando de alias con argumentos</span><span class="sxs-lookup"><span data-stu-id="f11d5-133">Create an alias command with arguments</span></span>

<span data-ttu-id="f11d5-134">También puede agregar argumentos posicionales a un comando de alias; para ello, inclúyalos como `{{ arg_name }}` en el nombre de alias.</span><span class="sxs-lookup"><span data-stu-id="f11d5-134">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="f11d5-135">El espacio en blanco entre las llaves es obligatorio.</span><span class="sxs-lookup"><span data-stu-id="f11d5-135">The whitespace inside the curly braces is required.</span></span>

```
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoke_including_args
```

<span data-ttu-id="f11d5-136">El alias de ejemplo siguiente muestra cómo usar argumentos posicionales para obtener la dirección IP pública de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="f11d5-136">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

<span data-ttu-id="f11d5-137">Al ejecutar este comando, asigne valores a los argumentos posicionales.</span><span class="sxs-lookup"><span data-stu-id="f11d5-137">When running this command, you give values to the positional arguments.</span></span>

```azruecli
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="f11d5-138">También puede usar variables de entorno en comandos invocados por alias, que se evalúan en tiempo de ejecución.</span><span class="sxs-lookup"><span data-stu-id="f11d5-138">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="f11d5-139">En el ejemplo siguiente, se agrega el alias `create-rg`, que crea un grupo de recursos en `eastus` y agrega una etiqueta `owner`.</span><span class="sxs-lookup"><span data-stu-id="f11d5-139">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="f11d5-140">A esta etiqueta se le asigna el valor de la variable de entorno local `USER`.</span><span class="sxs-lookup"><span data-stu-id="f11d5-140">This tag is assigned the value of the local environment variable `USER`.</span></span>

```
[create-rg {{ groupName }}]
command = group create --name {{ groupName }} --location eastus --tags owner=$USER
```

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="f11d5-141">Procesar argumentos mediante plantillas de Jinja2</span><span class="sxs-lookup"><span data-stu-id="f11d5-141">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="f11d5-142">La sustitución de argumentos en la extensión alias se realiza mediante [Jinja2](http://jinja.pocoo.org/docs/2.10/), lo que le proporciona acceso completo a las funcionalidades del motor de plantillas Jinja2.</span><span class="sxs-lookup"><span data-stu-id="f11d5-142">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="f11d5-143">Las plantillas permiten realizar acciones como la extracción de datos y la sustitución en cadenas.</span><span class="sxs-lookup"><span data-stu-id="f11d5-143">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="f11d5-144">Con las plantillas de Jinja2, puede escribir alias que tomen tipos de argumentos diferentes del comando subyacente.</span><span class="sxs-lookup"><span data-stu-id="f11d5-144">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="f11d5-145">Por ejemplo, puede crear un alias que tome una dirección URL de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="f11d5-145">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="f11d5-146">Después, se analiza esta dirección URL para pasar el nombre de la cuenta y el contenedor al comando de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="f11d5-146">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```
[storage-ls {{ url }}]
command = storage blob list --account-name {{ url.replace('https://', '').split('.')[0] }} --container-name {{ url.replace('https://', '').split('/')[1] }}
```

<span data-ttu-id="f11d5-147">Para más información sobre el motor de plantillas Jinja2, consulte [la documentación de Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="f11d5-147">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="f11d5-148">Desinstalar la extensión alias</span><span class="sxs-lookup"><span data-stu-id="f11d5-148">Uninstall the alias extension</span></span>

<span data-ttu-id="f11d5-149">Para desinstalar la extensión, use el comando [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="f11d5-149">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```bash
az extension remove --name alias
```

<span data-ttu-id="f11d5-150">Si desinstala debido a un error u otro problema con la extensión, [abra un problema en GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que podamos proporcionar una corrección.</span><span class="sxs-lookup"><span data-stu-id="f11d5-150">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
