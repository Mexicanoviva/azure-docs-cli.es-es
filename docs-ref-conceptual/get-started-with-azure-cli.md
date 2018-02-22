---
title: "Introducción a la CLI de Azure 2.0"
description: "Introducción al uso de la CLI de Azure 2.0 y los conceptos básicos de los comandos."
keywords: "CLI de Azure, ayuda de la CLI, ayuda de Azure, consulta, automatización,"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/05/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: c2758922d74080d3a3110b1e3a507ddf0f8d85d1
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="92d9d-104">Introducción a la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="92d9d-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="92d9d-105">Bienvenido a la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="92d9d-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="92d9d-106">La CLI es una herramienta diseñada para ayudarle a trabajar de forma rápida y eficaz con los servicios de Azure, con énfasis en la automatización.</span><span class="sxs-lookup"><span data-stu-id="92d9d-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="92d9d-107">En este artículo se detallan las características de la CLI y vínculos a recursos que le ayudarán a ser productivo.</span><span class="sxs-lookup"><span data-stu-id="92d9d-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-log-in"></a><span data-ttu-id="92d9d-108">Instalación e inicio de sesión</span><span class="sxs-lookup"><span data-stu-id="92d9d-108">Install and log in</span></span>

<span data-ttu-id="92d9d-109">Si no lo ha hecho ya, [instale la CLI](install-azure-cli.md) o pruebe el [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="92d9d-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="92d9d-110">Antes de usar los comandos de la CLI en una instalación local, deberá iniciar sesión con [az login](/cli/azure/index#az_login).</span><span class="sxs-lookup"><span data-stu-id="92d9d-110">Before using any CLI commands with a local install, you need to log in with [az login](/cli/azure/index#az_login).</span></span>

```azurecli
az login
```

<span data-ttu-id="92d9d-111">Este comando le pide que inicie sesión con un código de autenticación a través de un sitio web.</span><span class="sxs-lookup"><span data-stu-id="92d9d-111">This command prompts you to log in with an authentication code via a website.</span></span> <span data-ttu-id="92d9d-112">Hay maneras para iniciar sesión de una manera no interactiva, las cuales se tratan detalladamente en [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="92d9d-112">There are ways to log in non-interactively, which are covered in detail in [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="92d9d-113">Comandos comunes</span><span class="sxs-lookup"><span data-stu-id="92d9d-113">Common commands</span></span>

<span data-ttu-id="92d9d-114">Esta tabla enumera algunos de los comandos más comunes usados en la CLI junto con enlaces a páginas de documentación de referencia.</span><span class="sxs-lookup"><span data-stu-id="92d9d-114">This table lists a few of the common commands used in the CLI links out to their documentation pages in the reference.</span></span>
<span data-ttu-id="92d9d-115">Todos los subcomandos de estos grupos y su documentación se pueden buscar en la referencia en línea o con el argumento `--help`.</span><span class="sxs-lookup"><span data-stu-id="92d9d-115">All subcommands of these groups and their documentation can be looked up in online reference or with the `--help` argument.</span></span>

| <span data-ttu-id="92d9d-116">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="92d9d-116">Resource type</span></span> | <span data-ttu-id="92d9d-117">Grupo de comandos de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="92d9d-117">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="92d9d-118">Grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="92d9d-118">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="92d9d-119">az group</span><span class="sxs-lookup"><span data-stu-id="92d9d-119">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="92d9d-120">Máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="92d9d-120">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="92d9d-121">az vm</span><span class="sxs-lookup"><span data-stu-id="92d9d-121">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="92d9d-122">Cuentas de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="92d9d-122">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="92d9d-123">az storage account</span><span class="sxs-lookup"><span data-stu-id="92d9d-123">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="92d9d-124">Key Vault</span><span class="sxs-lookup"><span data-stu-id="92d9d-124">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="92d9d-125">az keyvault</span><span class="sxs-lookup"><span data-stu-id="92d9d-125">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="92d9d-126">Aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="92d9d-126">Web applications</span></span>](/azure/ap-service) | [<span data-ttu-id="92d9d-127">az webapp</span><span class="sxs-lookup"><span data-stu-id="92d9d-127">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="92d9d-128">Bases de datos SQL</span><span class="sxs-lookup"><span data-stu-id="92d9d-128">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="92d9d-129">az sql server</span><span class="sxs-lookup"><span data-stu-id="92d9d-129">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="92d9d-130">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="92d9d-130">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="92d9d-131">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="92d9d-131">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="92d9d-132">Búsqueda de comandos</span><span class="sxs-lookup"><span data-stu-id="92d9d-132">Finding commands</span></span>

<span data-ttu-id="92d9d-133">Los comandos de la CLI se proporcionan como _subcomandos_ de _grupos_.</span><span class="sxs-lookup"><span data-stu-id="92d9d-133">Commands in the CLI are provided as _subcommands_ of _groups_.</span></span>
<span data-ttu-id="92d9d-134">Cada grupo representa un servicio suministrado por Azure y los subgrupos dividen comandos para estos servicios en agrupaciones lógicas.</span><span class="sxs-lookup"><span data-stu-id="92d9d-134">Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings.</span></span>

<span data-ttu-id="92d9d-135">Para buscar comandos, utilice [az find](/cli/azure/index#az_find).</span><span class="sxs-lookup"><span data-stu-id="92d9d-135">To search for commands, use [az find](/cli/azure/index#az_find).</span></span> <span data-ttu-id="92d9d-136">Por ejemplo, para buscar nombres de comando que contienen `secret`, use el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="92d9d-136">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli
az find -q secret
```

<span data-ttu-id="92d9d-137">Si sabe con qué grupo de comandos desea trabajar, el argumento `--help` puede ser una opción mejor.</span><span class="sxs-lookup"><span data-stu-id="92d9d-137">If you know which group of commands you want to work with, the `--help` argument may be a better choice.</span></span> <span data-ttu-id="92d9d-138">Además de mostrar información detallada para un comando, cuando se usa con un grupo de comandos muestra todos los subcomandos disponibles.</span><span class="sxs-lookup"><span data-stu-id="92d9d-138">This displays not just detailed information for a command, but when used with a command group, displays all of the available subcommands.</span></span> <span data-ttu-id="92d9d-139">Por ejemplo, cuando se trabaja con grupos de seguridad de red (NSG) puede encontrar los comandos y subgrupos de NSG disponibles.</span><span class="sxs-lookup"><span data-stu-id="92d9d-139">For example, when working with Network Security Groups (NSGs) you can find the available NSG subgroups and commands.</span></span>

```azurecli
az network nsg --help
```

<span data-ttu-id="92d9d-140">La CLI dispone de la función de autocompletar con el tabulador para los comandos en el shell de bash.</span><span class="sxs-lookup"><span data-stu-id="92d9d-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="92d9d-141">Argumentos disponibles globalmente</span><span class="sxs-lookup"><span data-stu-id="92d9d-141">Globally available arguments</span></span>

<span data-ttu-id="92d9d-142">Hay algunos argumentos que están disponibles para todos los comandos.</span><span class="sxs-lookup"><span data-stu-id="92d9d-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="92d9d-143">`--help` imprime información de referencia de la CLI sobre los comandos y sus argumentos y enumera los comandos y subgrupos disponibles.</span><span class="sxs-lookup"><span data-stu-id="92d9d-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="92d9d-144">`--output` cambia el formato de salida.</span><span class="sxs-lookup"><span data-stu-id="92d9d-144">`--output` changes the output format.</span></span> <span data-ttu-id="92d9d-145">Los formatos de salida disponibles son `json`, `jsonc` (JSON coloreado), `tsv` (Valores separados por tabulaciones) y `table` (tablas ASCII de lenguaje natural).</span><span class="sxs-lookup"><span data-stu-id="92d9d-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="92d9d-146">De forma predeterminada, la CLI genera `json`.</span><span class="sxs-lookup"><span data-stu-id="92d9d-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="92d9d-147">Para más información sobre los formatos de salida disponibles, consulte [Formatos de salida de la CLI de Azure 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="92d9d-147">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="92d9d-148">`--query` usa el [lenguaje de consulta JMESPath](http://jmespath.org/) para filtrar los resultados devueltos por los servicios de Azure.</span><span class="sxs-lookup"><span data-stu-id="92d9d-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="92d9d-149">Para más información sobre las consultas, visite [Consulta de los resultados de los comandos con la CLI de Azure 2.0](query-azure-cli.md) y [Tutorial de JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="92d9d-149">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="92d9d-150">`--verbose` imprime información acerca de los recursos creados en Azure durante una operación y otra información de utilidad.</span><span class="sxs-lookup"><span data-stu-id="92d9d-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="92d9d-151">`--debug` imprime más información aún sobre las operaciones de la CLI y se utiliza con fines de depuración.</span><span class="sxs-lookup"><span data-stu-id="92d9d-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="92d9d-152">Si se produce un error, proporcione los resultados generados con la marca `--debug` activada al enviar un informe de errores.</span><span class="sxs-lookup"><span data-stu-id="92d9d-152">If you encounter a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>


## <a name="interactive-mode"></a><span data-ttu-id="92d9d-153">Modo interactivo</span><span class="sxs-lookup"><span data-stu-id="92d9d-153">Interactive mode</span></span>

<span data-ttu-id="92d9d-154">La CLI ofrece un modo interactivo que muestra automáticamente información de ayuda y facilita la selección de subcomandos.</span><span class="sxs-lookup"><span data-stu-id="92d9d-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="92d9d-155">Puede entrar en el modo interactivo con el comando `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="92d9d-155">You enter interactive mode with the `az interactive` command.</span></span> <span data-ttu-id="92d9d-156">Para más información sobre el modo interactivo y cómo ayuda a obtener información sobre la CLI, consulte [Modo interactivo de la CLI de Azure 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="92d9d-156">For more information on interactive mode and how it helps you learn the CLI, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="92d9d-157">También hay un [complemento de Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que ofrece una experiencia interactiva, incluida la función de autocompletar y documentación al pasar el ratón.</span><span class="sxs-lookup"><span data-stu-id="92d9d-157">There is also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>



## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="92d9d-158">Conozca los aspectos básicos de la CLI con las guías de inicio rápido y los tutoriales</span><span class="sxs-lookup"><span data-stu-id="92d9d-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="92d9d-159">Para ayudarle a comenzar con la CLI de Azure 2.0, pruebe con un tutorial exhaustivo sobre la configuración de máquinas virtuales y el uso de la potencia de la CLI para consultar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="92d9d-159">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="92d9d-160">Tutorial de creación de máquinas virtuales con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="92d9d-160">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="92d9d-161">Si prefiere centrarse en otros servicios, hay una variedad de tutoriales sobre los servicios de Azure que utilizan la CLI.</span><span class="sxs-lookup"><span data-stu-id="92d9d-161">If you would rather focus on other services, there are a variety of quickstarts for Azure services that use the CLI.</span></span>

* [<span data-ttu-id="92d9d-162">Creación de una cuenta de almacenamiento con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="92d9d-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cl)
* [<span data-ttu-id="92d9d-163">Transferencia de objetos a y desde Azure Blob Storage mediante la CLI</span><span class="sxs-lookup"><span data-stu-id="92d9d-163">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="92d9d-164">Creación de una sola instancia de Azure SQL Database con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="92d9d-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="92d9d-165">Creación de un servidor de Azure Database for MySQL mediante la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="92d9d-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="92d9d-166">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Creación de una base de datos Azure Database for PostgreSQL con la CLI de Azure)</span><span class="sxs-lookup"><span data-stu-id="92d9d-166">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="92d9d-167">Creación de una aplicación web de Python en Azure</span><span class="sxs-lookup"><span data-stu-id="92d9d-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="92d9d-168">Ejecución de una imagen personalizada de Docker Hub en Azure Web Apps for Containers</span><span class="sxs-lookup"><span data-stu-id="92d9d-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="92d9d-169">Envíenos sus comentarios</span><span class="sxs-lookup"><span data-stu-id="92d9d-169">Give feedback</span></span>

<span data-ttu-id="92d9d-170">Le agradecemos sus comentarios sobre la CLI para ayudarnos a mejorar y resolver errores.</span><span class="sxs-lookup"><span data-stu-id="92d9d-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="92d9d-171">También puede [informar de un problema en Github](https://github.com/azure/azure-cli/issues) o utilizar las características integradas de la CLI para dejar comentarios generales con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="92d9d-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the `az feedback` command.</span></span>

```azurecli
az feedback
```
