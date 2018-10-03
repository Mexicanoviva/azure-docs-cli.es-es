---
title: Introducción a la CLI de Azure
description: Introducción al uso de la CLI de Azure y los conceptos básicos de los comandos.
keywords: CLI de Azure, ayuda de la CLI, ayuda de Azure, consulta, automatización,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: d23548a9cdfe307c2597d992dc014125f80704d0
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178004"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="6ecb6-104">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="6ecb6-104">Get started with Azure CLI</span></span>

<span data-ttu-id="6ecb6-105">Bienvenido a la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-105">Welcome to the Azure CLI!</span></span> <span data-ttu-id="6ecb6-106">La CLI es una herramienta diseñada para ayudarle a trabajar de forma rápida y eficaz con los servicios de Azure, con énfasis en la automatización.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="6ecb6-107">En este artículo se detallan las características de la CLI y vínculos a recursos que le ayudarán a ser productivo.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="6ecb6-108">Instalación o ejecución en Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6ecb6-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="6ecb6-109">La manera más fácil empezar a trabajar con la CLI de Azure es ejecutarla en un entorno de Azure Cloud Shell en su explorador.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="6ecb6-110">Para más información acerca de Cloud Shell, consulte [Guía de inicio rápido de Bash en Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="6ecb6-111">Cuando esté listo para instalar la CLI, consulte las [instrucciones de instalación](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="6ecb6-112">Iniciar sesión</span><span class="sxs-lookup"><span data-stu-id="6ecb6-112">Sign in</span></span>

<span data-ttu-id="6ecb6-113">Antes de usar los comandos de la CLI en una instalación local, deberá iniciar sesión con [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-113">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6ecb6-114">Hay varias formas de iniciar sesión de una manera no interactiva, que se describen con detalle en [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-114">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="6ecb6-115">Comandos comunes</span><span class="sxs-lookup"><span data-stu-id="6ecb6-115">Common commands</span></span>

<span data-ttu-id="6ecb6-116">En esta tabla se enumeran algunos comandos comunes utilizados en la CLI, así como vínculos a documentación de referencia.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-116">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="6ecb6-117">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="6ecb6-117">Resource type</span></span> | <span data-ttu-id="6ecb6-118">Grupo de comandos de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="6ecb6-118">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="6ecb6-119">Grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="6ecb6-119">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="6ecb6-120">az group</span><span class="sxs-lookup"><span data-stu-id="6ecb6-120">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="6ecb6-121">Máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="6ecb6-121">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="6ecb6-122">az vm</span><span class="sxs-lookup"><span data-stu-id="6ecb6-122">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="6ecb6-123">Cuentas de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="6ecb6-123">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="6ecb6-124">az storage account</span><span class="sxs-lookup"><span data-stu-id="6ecb6-124">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="6ecb6-125">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6ecb6-125">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="6ecb6-126">az keyvault</span><span class="sxs-lookup"><span data-stu-id="6ecb6-126">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="6ecb6-127">Aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="6ecb6-127">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="6ecb6-128">az webapp</span><span class="sxs-lookup"><span data-stu-id="6ecb6-128">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="6ecb6-129">Bases de datos SQL</span><span class="sxs-lookup"><span data-stu-id="6ecb6-129">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="6ecb6-130">az sql server</span><span class="sxs-lookup"><span data-stu-id="6ecb6-130">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="6ecb6-131">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6ecb6-131">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="6ecb6-132">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="6ecb6-132">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="6ecb6-133">Búsqueda de comandos</span><span class="sxs-lookup"><span data-stu-id="6ecb6-133">Finding commands</span></span>

<span data-ttu-id="6ecb6-134">Los comandos de la CLI se organizan como _grupos_ de _comandos_.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-134">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="6ecb6-135">Cada grupo representa un servicio de Azure y los comandos funcionan en ese servicio.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-135">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="6ecb6-136">Para buscar comandos, utilice [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-136">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="6ecb6-137">Por ejemplo, para buscar nombres de comando que contienen `secret`, use el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="6ecb6-137">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="6ecb6-138">Use el argumento `--help` para obtener una lista completa de los comandos y los subgrupos de un grupo.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-138">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="6ecb6-139">Por ejemplo, para encontrar los comandos de la CLI para trabajar con grupos de seguridad de red (NSG):</span><span class="sxs-lookup"><span data-stu-id="6ecb6-139">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="6ecb6-140">La CLI dispone de la función de autocompletar con el tabulador para los comandos en el shell de bash.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="6ecb6-141">Argumentos disponibles globalmente</span><span class="sxs-lookup"><span data-stu-id="6ecb6-141">Globally available arguments</span></span>

<span data-ttu-id="6ecb6-142">Hay algunos argumentos que están disponibles para todos los comandos.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="6ecb6-143">`--help` imprime información de referencia de la CLI sobre los comandos y sus argumentos y enumera los comandos y subgrupos disponibles.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="6ecb6-144">`--output` cambia el formato de salida.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-144">`--output` changes the output format.</span></span> <span data-ttu-id="6ecb6-145">Los formatos de salida disponibles son `json`, `jsonc` (JSON coloreado), `tsv` (Valores separados por tabulaciones) y `table` (tablas ASCII de lenguaje natural).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="6ecb6-146">De forma predeterminada, la CLI genera `json`.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="6ecb6-147">Para más información sobre los formatos de salida disponibles, consulte [Formatos de salida de la CLI de Azure](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-147">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="6ecb6-148">`--query` usa el [lenguaje de consulta JMESPath](http://jmespath.org/) para filtrar los resultados devueltos por los servicios de Azure.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="6ecb6-149">Para más información sobre las consultas, consulte [Consulta de los resultados de los comandos con la CLI de Azure](query-azure-cli.md) y [Tutorial de JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-149">To learn To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="6ecb6-150">`--verbose` imprime información acerca de los recursos creados en Azure durante una operación y otra información de utilidad.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="6ecb6-151">`--debug` imprime más información aún sobre las operaciones de la CLI y se utiliza con fines de depuración.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="6ecb6-152">Si encuentra un error, proporcione la salida que se genera con la marca `--debug` activada al enviar un informe de errores.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-152">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="6ecb6-153">Modo interactivo</span><span class="sxs-lookup"><span data-stu-id="6ecb6-153">Interactive mode</span></span>

<span data-ttu-id="6ecb6-154">La CLI ofrece un modo interactivo que muestra automáticamente información de ayuda y facilita la selección de subcomandos.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="6ecb6-155">Puede entrar en el modo interactivo con el comando [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-155">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="6ecb6-156">Para más información sobre el modo interactivo, consulte [Modo interactivo de la CLI de Azure](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-156">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="6ecb6-157">También hay un [complemento de Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que ofrece una experiencia interactiva, incluida la función de autocompletar y documentación al pasar el ratón.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-157">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="6ecb6-158">Conozca los aspectos básicos de la CLI con las guías de inicio rápido y los tutoriales</span><span class="sxs-lookup"><span data-stu-id="6ecb6-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="6ecb6-159">Para ayudarle a comenzar con la CLI de Azure, pruebe con un tutorial exhaustivo sobre la configuración de máquinas virtuales y el uso de la potencia de la CLI para consultar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-159">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6ecb6-160">Tutorial de creación de máquinas virtuales con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="6ecb6-160">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="6ecb6-161">También hay guías de inicio rápido para otros servicios populares.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-161">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="6ecb6-162">Creación de una cuenta de almacenamiento con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="6ecb6-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="6ecb6-163">Transferencia de objetos a y desde Azure Blob Storage mediante la CLI</span><span class="sxs-lookup"><span data-stu-id="6ecb6-163">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="6ecb6-164">Creación de una sola instancia de Azure SQL Database con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="6ecb6-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="6ecb6-165">Creación de un servidor de Azure Database for MySQL mediante la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="6ecb6-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="6ecb6-166">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Creación de una base de datos Azure Database for PostgreSQL con la CLI de Azure)</span><span class="sxs-lookup"><span data-stu-id="6ecb6-166">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="6ecb6-167">Creación de una aplicación web de Python en Azure</span><span class="sxs-lookup"><span data-stu-id="6ecb6-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="6ecb6-168">Ejecución de una imagen personalizada de Docker Hub en Azure Web Apps for Containers</span><span class="sxs-lookup"><span data-stu-id="6ecb6-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="6ecb6-169">Envíenos sus comentarios</span><span class="sxs-lookup"><span data-stu-id="6ecb6-169">Give feedback</span></span>

<span data-ttu-id="6ecb6-170">Le agradecemos sus comentarios sobre la CLI para ayudarnos a mejorar y resolver errores.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="6ecb6-171">También puede [informar de un problema en Github](https://github.com/azure/azure-cli/issues) o utilizar las características integradas de la CLI para dejar comentarios generales con el comando [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
