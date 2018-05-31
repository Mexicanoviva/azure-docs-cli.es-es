---
title: Introducción a la CLI de Azure 2.0
description: Introducción al uso de la CLI de Azure 2.0 y los conceptos básicos de los comandos.
keywords: CLI de Azure, ayuda de la CLI, ayuda de Azure, consulta, automatización,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0c7746e70125dcc1678ed19f93322efea8a2b01b
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306104"
---
# <a name="get-started-with-azure-cli-20"></a>Introducción a la CLI de Azure 2.0

Bienvenido a la CLI de Azure 2.0. La CLI es una herramienta diseñada para ayudarle a trabajar de forma rápida y eficaz con los servicios de Azure, con énfasis en la automatización. En este artículo se detallan las características de la CLI y vínculos a recursos que le ayudarán a ser productivo.

## <a name="install-and-log-in"></a>Instalación e inicio de sesión

Si no lo ha hecho ya, [instale la CLI](install-azure-cli.md) o pruebe el [Azure Cloud Shell](/azure/cloud-shell/overview).

Antes de usar los comandos de la CLI en una instalación local, deberá iniciar sesión con [az login](/cli/azure/reference-index#az-login).

```azurecli
az login
```

Este comando le pide que inicie sesión con un código de autenticación a través de un sitio web. Hay maneras para iniciar sesión de una manera no interactiva, las cuales se tratan detalladamente en [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).

## <a name="common-commands"></a>Comandos comunes

Esta tabla enumera algunos de los comandos más comunes usados en la CLI junto con enlaces a páginas de documentación de referencia.
Todos los subcomandos de estos grupos y su documentación se pueden buscar en la referencia en línea o con el argumento `--help`.

| Tipo de recurso | Grupo de comandos de la CLI de Azure |
|---------------|-------------------------|
| [Grupos de recursos](/azure/azure-resource-manager/resource-group-overview) | [az group](/cli/azure/group) |
| [Máquinas virtuales](/azure/virtual-machines) | [az vm](/cli/azure/vm) |
| [Cuentas de almacenamiento](/azure/storage/common/storage-introduction) | [az storage account](/cli/azure/storage/account) |
| [Key Vault](/azure/key-vault/key-vault-whatis) | [az keyvault](/cli/azure/keyvault) |
| [Aplicaciones web](/azure/ap-service) | [az webapp](/cli/azure/webapp) |
| [Bases de datos SQL](/azure/sql-database) | [az sql server](/cli/azure/sql/server) |
| [CosmosDB](/azure/cosmos-db) | [az cosmosdb](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a>Búsqueda de comandos

Los comandos de la CLI se proporcionan como _subcomandos_ de _grupos_.
Cada grupo representa un servicio suministrado por Azure y los subgrupos dividen comandos para estos servicios en agrupaciones lógicas.

Para buscar comandos, utilice [az find](/cli/azure/reference-index#az-find). Por ejemplo, para buscar nombres de comando que contienen `secret`, use el siguiente comando:

```azurecli-interactive
az find -q secret
```

Si sabe con qué grupo de comandos desea trabajar, el argumento `--help` puede ser una opción mejor. Además de mostrar información detallada para un comando, cuando se usa con un grupo de comandos muestra todos los subcomandos disponibles. Por ejemplo, cuando se trabaja con grupos de seguridad de red (NSG) puede encontrar los comandos y subgrupos de NSG disponibles.

```azurecli-interactive
az network nsg --help
```

La CLI dispone de la función de autocompletar con el tabulador para los comandos en el shell de bash.

## <a name="globally-available-arguments"></a>Argumentos disponibles globalmente

Hay algunos argumentos que están disponibles para todos los comandos.

* `--help` imprime información de referencia de la CLI sobre los comandos y sus argumentos y enumera los comandos y subgrupos disponibles.
* `--output` cambia el formato de salida. Los formatos de salida disponibles son `json`, `jsonc` (JSON coloreado), `tsv` (Valores separados por tabulaciones) y `table` (tablas ASCII de lenguaje natural). De forma predeterminada, la CLI genera `json`. Para más información sobre los formatos de salida disponibles, consulte [Formatos de salida de la CLI de Azure 2.0](format-output-azure-cli.md).
* `--query` usa el [lenguaje de consulta JMESPath](http://jmespath.org/) para filtrar los resultados devueltos por los servicios de Azure. Para más información sobre las consultas, visite [Consulta de los resultados de los comandos con la CLI de Azure 2.0](query-azure-cli.md) y [Tutorial de JMESPath](http://jmespath.org/tutorial.html).
* `--verbose` imprime información acerca de los recursos creados en Azure durante una operación y otra información de utilidad.
* `--debug` imprime más información aún sobre las operaciones de la CLI y se utiliza con fines de depuración. Si se produce un error, proporcione los resultados generados con la marca `--debug` activada al enviar un informe de errores.


## <a name="interactive-mode"></a>Modo interactivo

La CLI ofrece un modo interactivo que muestra automáticamente información de ayuda y facilita la selección de subcomandos. Puede entrar en el modo interactivo con el comando [az interactive](/cli/azure/reference-index#az-interactive).

```azurecli-interactive
az interactive
```

Para más información sobre el modo interactivo, consulte [Modo interactivo de la CLI de Azure 2.0](interactive-azure-cli.md).

También hay un [complemento de Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que ofrece una experiencia interactiva, incluida la función de autocompletar y documentación al pasar el ratón.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Conozca los aspectos básicos de la CLI con las guías de inicio rápido y los tutoriales

Para ayudarle a comenzar con la CLI de Azure 2.0, pruebe con un tutorial exhaustivo sobre la configuración de máquinas virtuales y el uso de la potencia de la CLI para consultar los recursos de Azure.

> [!div class="nextstepaction"]
> [Tutorial de creación de máquinas virtuales con la CLI de Azure 2.0](azure-cli-vm-tutorial.yml)

Si prefiere centrarse en otros servicios, hay una variedad de tutoriales sobre los servicios de Azure que utilizan la CLI.

* [Creación de una cuenta de almacenamiento con la CLI de Azure](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [Transferencia de objetos a y desde Azure Blob Storage mediante la CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [Creación de una sola instancia de Azure SQL Database con la CLI de Azure](/azure/sql-database/sql-database-get-started-cli)
* [Creación de un servidor de Azure Database for MySQL mediante la CLI de Azure](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Creación de una base de datos Azure Database for PostgreSQL con la CLI de Azure)
* [Creación de una aplicación web de Python en Azure](/azure/app-service/app-service-web-get-started-python)
* [Ejecución de una imagen personalizada de Docker Hub en Azure Web Apps for Containers](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a>Envíenos sus comentarios

Le agradecemos sus comentarios sobre la CLI para ayudarnos a mejorar y resolver errores. También puede [informar de un problema en Github](https://github.com/azure/azure-cli/issues) o utilizar las características integradas de la CLI para dejar comentarios generales con el comando [az feedback](/cli/azure/reference-index#az-feedback).

```azurecli-interactive
az feedback
```
