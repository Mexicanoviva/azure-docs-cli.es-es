---
title: Introducción a la CLI de Azure 2.0
description: Introducción al uso de la CLI de Azure 2.0 y los conceptos básicos de los comandos.
keywords: CLI de Azure, ayuda de la CLI, ayuda de Azure, consulta, automatización,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 165da295d187edf7dbc19a332670fd49d8f8bdd5
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388565"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="7cf5b-104">Introducción a la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="7cf5b-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="7cf5b-105">Bienvenido a la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="7cf5b-106">La CLI es una herramienta diseñada para ayudarle a trabajar de forma rápida y eficaz con los servicios de Azure, con énfasis en la automatización.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="7cf5b-107">En este artículo se detallan las características de la CLI y vínculos a recursos que le ayudarán a ser productivo.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-sign-in"></a><span data-ttu-id="7cf5b-108">Instalación e inicio de sesión</span><span class="sxs-lookup"><span data-stu-id="7cf5b-108">Install and sign in</span></span>

<span data-ttu-id="7cf5b-109">Si no lo ha hecho ya, [instale la CLI](install-azure-cli.md) o pruebe el [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="7cf5b-110">Antes de usar los comandos de la CLI en una instalación local, deberá iniciar sesión con [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-110">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="7cf5b-111">Hay varias formas de iniciar sesión de una manera no interactiva, que se describen con detalle en [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-111">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="7cf5b-112">Comandos comunes</span><span class="sxs-lookup"><span data-stu-id="7cf5b-112">Common commands</span></span>

<span data-ttu-id="7cf5b-113">En esta tabla se enumeran algunos comandos comunes utilizados en la CLI, así como vínculos a documentación de referencia.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-113">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="7cf5b-114">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="7cf5b-114">Resource type</span></span> | <span data-ttu-id="7cf5b-115">Grupo de comandos de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7cf5b-115">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="7cf5b-116">Grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="7cf5b-116">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="7cf5b-117">az group</span><span class="sxs-lookup"><span data-stu-id="7cf5b-117">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="7cf5b-118">Máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="7cf5b-118">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="7cf5b-119">az vm</span><span class="sxs-lookup"><span data-stu-id="7cf5b-119">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="7cf5b-120">Cuentas de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7cf5b-120">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="7cf5b-121">az storage account</span><span class="sxs-lookup"><span data-stu-id="7cf5b-121">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="7cf5b-122">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7cf5b-122">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="7cf5b-123">az keyvault</span><span class="sxs-lookup"><span data-stu-id="7cf5b-123">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="7cf5b-124">Aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="7cf5b-124">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="7cf5b-125">az webapp</span><span class="sxs-lookup"><span data-stu-id="7cf5b-125">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="7cf5b-126">Bases de datos SQL</span><span class="sxs-lookup"><span data-stu-id="7cf5b-126">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="7cf5b-127">az sql server</span><span class="sxs-lookup"><span data-stu-id="7cf5b-127">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="7cf5b-128">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7cf5b-128">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="7cf5b-129">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="7cf5b-129">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="7cf5b-130">Búsqueda de comandos</span><span class="sxs-lookup"><span data-stu-id="7cf5b-130">Finding commands</span></span>

<span data-ttu-id="7cf5b-131">Los comandos de la CLI se organizan como _grupos_ de _comandos_.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-131">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="7cf5b-132">Cada grupo representa un servicio de Azure y los comandos funcionan en ese servicio.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-132">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="7cf5b-133">Para buscar comandos, utilice [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-133">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="7cf5b-134">Por ejemplo, para buscar nombres de comando que contienen `secret`, use el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="7cf5b-134">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="7cf5b-135">Use el argumento `--help` para obtener una lista completa de los comandos y los subgrupos de un grupo.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-135">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="7cf5b-136">Por ejemplo, para encontrar los comandos de la CLI para trabajar con grupos de seguridad de red (NSG):</span><span class="sxs-lookup"><span data-stu-id="7cf5b-136">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="7cf5b-137">La CLI dispone de la función de autocompletar con el tabulador para los comandos en el shell de bash.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-137">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="7cf5b-138">Argumentos disponibles globalmente</span><span class="sxs-lookup"><span data-stu-id="7cf5b-138">Globally available arguments</span></span>

<span data-ttu-id="7cf5b-139">Hay algunos argumentos que están disponibles para todos los comandos.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-139">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="7cf5b-140">`--help` imprime información de referencia de la CLI sobre los comandos y sus argumentos y enumera los comandos y subgrupos disponibles.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-140">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="7cf5b-141">`--output` cambia el formato de salida.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-141">`--output` changes the output format.</span></span> <span data-ttu-id="7cf5b-142">Los formatos de salida disponibles son `json`, `jsonc` (JSON coloreado), `tsv` (Valores separados por tabulaciones) y `table` (tablas ASCII de lenguaje natural).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-142">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="7cf5b-143">De forma predeterminada, la CLI genera `json`.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-143">By default the CLI outputs `json`.</span></span> <span data-ttu-id="7cf5b-144">Para más información sobre los formatos de salida disponibles, consulte [Formatos de salida de la CLI de Azure 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-144">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="7cf5b-145">`--query` usa el [lenguaje de consulta JMESPath](http://jmespath.org/) para filtrar los resultados devueltos por los servicios de Azure.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-145">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="7cf5b-146">Para más información sobre las consultas, visite [Consulta de los resultados de los comandos con la CLI de Azure 2.0](query-azure-cli.md) y [Tutorial de JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-146">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="7cf5b-147">`--verbose` imprime información acerca de los recursos creados en Azure durante una operación y otra información de utilidad.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-147">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="7cf5b-148">`--debug` imprime más información aún sobre las operaciones de la CLI y se utiliza con fines de depuración.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-148">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="7cf5b-149">Si encuentra un error, proporcione la salida que se genera con la marca `--debug` activada al enviar un informe de errores.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-149">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="7cf5b-150">Modo interactivo</span><span class="sxs-lookup"><span data-stu-id="7cf5b-150">Interactive mode</span></span>

<span data-ttu-id="7cf5b-151">La CLI ofrece un modo interactivo que muestra automáticamente información de ayuda y facilita la selección de subcomandos.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-151">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="7cf5b-152">Puede entrar en el modo interactivo con el comando [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-152">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="7cf5b-153">Para más información sobre el modo interactivo, consulte [Modo interactivo de la CLI de Azure 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-153">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="7cf5b-154">También hay un [complemento de Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que ofrece una experiencia interactiva, incluida la función de autocompletar y documentación al pasar el ratón.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-154">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="7cf5b-155">Conozca los aspectos básicos de la CLI con las guías de inicio rápido y los tutoriales</span><span class="sxs-lookup"><span data-stu-id="7cf5b-155">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="7cf5b-156">Para ayudarle a comenzar con la CLI de Azure 2.0, pruebe con un tutorial exhaustivo sobre la configuración de máquinas virtuales y el uso de la potencia de la CLI para consultar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-156">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="7cf5b-157">Tutorial de creación de máquinas virtuales con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="7cf5b-157">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="7cf5b-158">También hay guías de inicio rápido para otros servicios populares.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-158">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="7cf5b-159">Creación de una cuenta de almacenamiento con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7cf5b-159">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="7cf5b-160">Transferencia de objetos a y desde Azure Blob Storage mediante la CLI</span><span class="sxs-lookup"><span data-stu-id="7cf5b-160">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="7cf5b-161">Creación de una sola instancia de Azure SQL Database con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7cf5b-161">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="7cf5b-162">Creación de un servidor de Azure Database for MySQL mediante la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7cf5b-162">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="7cf5b-163">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Creación de una base de datos Azure Database for PostgreSQL con la CLI de Azure)</span><span class="sxs-lookup"><span data-stu-id="7cf5b-163">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="7cf5b-164">Creación de una aplicación web de Python en Azure</span><span class="sxs-lookup"><span data-stu-id="7cf5b-164">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="7cf5b-165">Ejecución de una imagen personalizada de Docker Hub en Azure Web Apps for Containers</span><span class="sxs-lookup"><span data-stu-id="7cf5b-165">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="7cf5b-166">Envíenos sus comentarios</span><span class="sxs-lookup"><span data-stu-id="7cf5b-166">Give feedback</span></span>

<span data-ttu-id="7cf5b-167">Le agradecemos sus comentarios sobre la CLI para ayudarnos a mejorar y resolver errores.</span><span class="sxs-lookup"><span data-stu-id="7cf5b-167">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="7cf5b-168">También puede [informar de un problema en Github](https://github.com/azure/azure-cli/issues) o utilizar las características integradas de la CLI para dejar comentarios generales con el comando [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="7cf5b-168">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
