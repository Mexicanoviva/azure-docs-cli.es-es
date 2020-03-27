---
title: Introducción a la CLI de Azure
description: Introducción al uso de la CLI de Azure y los conceptos básicos de los comandos.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/30/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: bc9b86db6fb9c5b3731550df9dda96debcbfba9f
ms.sourcegitcommit: 93d8137f37e974f7d314a0b1deb65ac563c2e2c5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/21/2020
ms.locfileid: "79990115"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="28990-103">Introducción a la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-103">Get started with Azure CLI</span></span>

<span data-ttu-id="28990-104">Bienvenido a la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="28990-104">Welcome to the Azure CLI!</span></span>  <span data-ttu-id="28990-105">En este artículo se presenta la CLI y se facilita ayuda sobre la realización de tareas comunes.</span><span class="sxs-lookup"><span data-stu-id="28990-105">This article introduces the CLI and helps you complete common tasks.</span></span>

> [!NOTE]
>
> <span data-ttu-id="28990-106">En los scripts y en el sitio de documentación de Microsoft, los ejemplos de la CLI de Azure están escritos para el shell de `bash`.</span><span class="sxs-lookup"><span data-stu-id="28990-106">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="28990-107">Los ejemplos de una línea funcionarán en cualquier plataforma.</span><span class="sxs-lookup"><span data-stu-id="28990-107">One-line examples will run on any platform.</span></span> <span data-ttu-id="28990-108">Los ejemplos más largos que incluyan continuaciones de línea (`\`) o asignación de variables deben modificarse para que funcionen en otros shells, incluido PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28990-108">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="28990-109">Instalación o ejecución en Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="28990-109">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="28990-110">La manera más fácil empezar a trabajar con la CLI de Azure es ejecutarla en un entorno de Azure Cloud Shell en su explorador.</span><span class="sxs-lookup"><span data-stu-id="28990-110">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="28990-111">Para más información acerca de Cloud Shell, consulte [Guía de inicio rápido de Bash en Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="28990-111">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="28990-112">Cuando esté listo para instalar la CLI, consulte las [instrucciones de instalación](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="28990-112">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="28990-113">Después de instalar la CLI por primera vez, ejecute `az --version` para comprobar que está instalada y que tiene la versión correcta.</span><span class="sxs-lookup"><span data-stu-id="28990-113">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

> [!NOTE]
> <span data-ttu-id="28990-114">Si usa el modelo de implementación clásico de Azure, [instale la CLI clásica de Azure](install-classic-cli.md).</span><span class="sxs-lookup"><span data-stu-id="28990-114">If you're using the Azure classic deployment model, [install the Azure classic CLI](install-classic-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="28990-115">Iniciar sesión</span><span class="sxs-lookup"><span data-stu-id="28990-115">Sign in</span></span>

<span data-ttu-id="28990-116">Antes de usar los comandos de la CLI en una instalación local, deberá iniciar sesión con [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="28990-116">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="28990-117">Después de iniciar sesión, verá una lista de suscripciones asociadas con su cuenta de Azure.</span><span class="sxs-lookup"><span data-stu-id="28990-117">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="28990-118">La información de suscripción con `isDefault: true` es la suscripción actualmente activada después de iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="28990-118">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="28990-119">Para seleccionar otra suscripción, utilice el comando [az account set](/cli/azure/account#az-account-set) con el identificador de suscripción al que desea cambiar.</span><span class="sxs-lookup"><span data-stu-id="28990-119">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="28990-120">Para más información sobre la selección de suscripción, consulte [Uso de varias suscripciones de Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="28990-120">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="28990-121">Hay varias formas de iniciar sesión de una manera no interactiva, que se describen con detalle en [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="28990-121">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="28990-122">Comandos comunes</span><span class="sxs-lookup"><span data-stu-id="28990-122">Common commands</span></span>

<span data-ttu-id="28990-123">En esta tabla se enumeran algunos comandos comunes utilizados en la CLI, así como vínculos a documentación de referencia.</span><span class="sxs-lookup"><span data-stu-id="28990-123">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="28990-124">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="28990-124">Resource type</span></span> | <span data-ttu-id="28990-125">Grupo de comandos de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-125">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="28990-126">Grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="28990-126">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="28990-127">az group</span><span class="sxs-lookup"><span data-stu-id="28990-127">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="28990-128">Máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="28990-128">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="28990-129">az vm</span><span class="sxs-lookup"><span data-stu-id="28990-129">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="28990-130">Cuentas de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="28990-130">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="28990-131">az storage account</span><span class="sxs-lookup"><span data-stu-id="28990-131">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="28990-132">Key Vault</span><span class="sxs-lookup"><span data-stu-id="28990-132">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="28990-133">az keyvault</span><span class="sxs-lookup"><span data-stu-id="28990-133">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="28990-134">Aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="28990-134">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="28990-135">az webapp</span><span class="sxs-lookup"><span data-stu-id="28990-135">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="28990-136">Bases de datos SQL</span><span class="sxs-lookup"><span data-stu-id="28990-136">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="28990-137">az sql server</span><span class="sxs-lookup"><span data-stu-id="28990-137">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="28990-138">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="28990-138">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="28990-139">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="28990-139">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="28990-140">Búsqueda de comandos</span><span class="sxs-lookup"><span data-stu-id="28990-140">Finding commands</span></span>

<span data-ttu-id="28990-141">Los comandos de la CLI se organizan como _grupos_ de _comandos_.</span><span class="sxs-lookup"><span data-stu-id="28990-141">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="28990-142">Cada grupo representa un servicio de Azure y los comandos funcionan en ese servicio.</span><span class="sxs-lookup"><span data-stu-id="28990-142">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="28990-143">Para buscar comandos, utilice [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="28990-143">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="28990-144">Por ejemplo, para buscar nombres de comando que contienen `secret`, use el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="28990-144">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find secret
```

<span data-ttu-id="28990-145">Use el argumento `--help` para obtener una lista completa de los comandos y los subgrupos de un grupo.</span><span class="sxs-lookup"><span data-stu-id="28990-145">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="28990-146">Por ejemplo, para encontrar los comandos de la CLI para trabajar con grupos de seguridad de red (NSG):</span><span class="sxs-lookup"><span data-stu-id="28990-146">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="28990-147">La CLI dispone de la función de autocompletar con el tabulador para los comandos en el shell de bash.</span><span class="sxs-lookup"><span data-stu-id="28990-147">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="28990-148">Argumentos disponibles globalmente</span><span class="sxs-lookup"><span data-stu-id="28990-148">Globally available arguments</span></span>

<span data-ttu-id="28990-149">Hay algunos argumentos que están disponibles para todos los comandos.</span><span class="sxs-lookup"><span data-stu-id="28990-149">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="28990-150">`--help` imprime información de referencia de la CLI sobre los comandos y sus argumentos y enumera los comandos y subgrupos disponibles.</span><span class="sxs-lookup"><span data-stu-id="28990-150">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="28990-151">`--output` cambia el formato de salida.</span><span class="sxs-lookup"><span data-stu-id="28990-151">`--output` changes the output format.</span></span> <span data-ttu-id="28990-152">Los formatos de salida disponibles son `json`, `jsonc` (JSON coloreado), `tsv` (valores separados por tabulaciones), `table` (tablas ASCII en lenguaje natural) y `yaml`.</span><span class="sxs-lookup"><span data-stu-id="28990-152">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="28990-153">De forma predeterminada, la CLI genera `json`.</span><span class="sxs-lookup"><span data-stu-id="28990-153">By default the CLI outputs `json`.</span></span> <span data-ttu-id="28990-154">Para más información sobre los formatos de salida disponibles, consulte [Formatos de salida de la CLI de Azure](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="28990-154">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="28990-155">`--query` usa el [lenguaje de consulta JMESPath](http://jmespath.org/) para filtrar los resultados devueltos por los servicios de Azure.</span><span class="sxs-lookup"><span data-stu-id="28990-155">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="28990-156">Para más información sobre las consultas, vea [Consulta de los resultados de los comandos con la CLI de Azure](query-azure-cli.md) y [Tutorial de JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="28990-156">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="28990-157">`--verbose` imprime información acerca de los recursos creados en Azure durante una operación y otra información de utilidad.</span><span class="sxs-lookup"><span data-stu-id="28990-157">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="28990-158">`--debug` imprime más información aún sobre las operaciones de la CLI y se utiliza con fines de depuración.</span><span class="sxs-lookup"><span data-stu-id="28990-158">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="28990-159">Si encuentra un error, proporcione la salida que se genera con la marca `--debug` activada al enviar un informe de errores.</span><span class="sxs-lookup"><span data-stu-id="28990-159">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="28990-160">Modo interactivo</span><span class="sxs-lookup"><span data-stu-id="28990-160">Interactive mode</span></span>

<span data-ttu-id="28990-161">La CLI ofrece un modo interactivo que muestra automáticamente información de ayuda y facilita la selección de subcomandos.</span><span class="sxs-lookup"><span data-stu-id="28990-161">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="28990-162">Puede entrar en el modo interactivo con el comando [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="28990-162">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="28990-163">Para más información sobre el modo interactivo, consulte [Modo interactivo de la CLI de Azure](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="28990-163">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="28990-164">También hay un [complemento de Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que ofrece una experiencia interactiva, incluida la función de autocompletar y documentación al pasar el ratón.</span><span class="sxs-lookup"><span data-stu-id="28990-164">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="28990-165">Conozca los aspectos básicos de la CLI con las guías de inicio rápido y los tutoriales</span><span class="sxs-lookup"><span data-stu-id="28990-165">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="28990-166">Para ayudarle a comenzar con la CLI de Azure, pruebe con un tutorial exhaustivo sobre la configuración de máquinas virtuales y el uso de la potencia de la CLI para consultar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="28990-166">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="28990-167">Tutorial de creación de máquinas virtuales con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-167">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="28990-168">También hay guías de inicio rápido para otros servicios populares.</span><span class="sxs-lookup"><span data-stu-id="28990-168">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="28990-169">Creación de una cuenta de almacenamiento con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-169">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="28990-170">Transferencia de objetos a y desde Azure Blob Storage mediante la CLI</span><span class="sxs-lookup"><span data-stu-id="28990-170">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="28990-171">Creación de una base de datos de Azure SQL única con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-171">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="28990-172">Creación de un servidor de Azure Database for MySQL mediante la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-172">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="28990-173">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Creación de una base de datos Azure Database for PostgreSQL con la CLI de Azure)</span><span class="sxs-lookup"><span data-stu-id="28990-173">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="28990-174">Creación de una aplicación web de Python en Azure</span><span class="sxs-lookup"><span data-stu-id="28990-174">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="28990-175">Ejecución de una imagen personalizada de Docker Hub en Azure Web Apps for Containers</span><span class="sxs-lookup"><span data-stu-id="28990-175">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="28990-176">Envíenos sus comentarios</span><span class="sxs-lookup"><span data-stu-id="28990-176">Give feedback</span></span>

<span data-ttu-id="28990-177">Le agradecemos sus comentarios sobre la CLI para ayudarnos a mejorar y resolver errores.</span><span class="sxs-lookup"><span data-stu-id="28990-177">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="28990-178">También puede [informar de un problema en GitHub](https://github.com/azure/azure-cli/issues) o utilizar las características integradas de la CLI para dejar comentarios generales con el comando [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="28990-178">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

## <a name="see-also"></a><span data-ttu-id="28990-179">Consulte también</span><span class="sxs-lookup"><span data-stu-id="28990-179">See also</span></span>

* [<span data-ttu-id="28990-180">Servicios que se pueden administrar con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-180">Services the Azure CLI can manage</span></span>](azure-services-the-azure-cli-can-manage.md)
* [<span data-ttu-id="28990-181">Lista de referencia de comandos completa para la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-181">Full command reference list for the Azure CLI</span></span>](/cli/azure/reference-index)
* [<span data-ttu-id="28990-182">Artículos populares sobre el uso de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="28990-182">Popular articles on using the Azure CLI</span></span>](popular-articles-using-the-azure-cli.md)
