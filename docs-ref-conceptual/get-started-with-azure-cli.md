---
title: Introducción a la CLI de Azure
description: Introducción al uso de la CLI de Azure y los conceptos básicos de los comandos.
keywords: CLI de Azure, ayuda de la CLI, ayuda de Azure, consulta, automatización,
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/30/2020
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 741d092121bbd448595301000acb9a5f51d87ace
ms.sourcegitcommit: d0b2763cc856eef44a6ecb78f6b8c64291625750
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/04/2020
ms.locfileid: "77013257"
---
# <a name="get-started-with-azure-cli"></a>Introducción a la CLI de Azure

Bienvenido a la CLI de Azure.  En este artículo se presenta la CLI y se proporcionan vínculos para que pueda empezar a trabajar con ella.

> [!NOTE]
>
> En los scripts y en el sitio de documentación de Microsoft, los ejemplos de la CLI de Azure están escritos para el shell de `bash`. Los ejemplos de una línea funcionarán en cualquier plataforma. Los ejemplos más largos que incluyan continuaciones de línea (`\`) o asignación de variables deben modificarse para que funcionen en otros shells, incluido PowerShell.

## <a name="install-or-run-in-azure-cloud-shell"></a>Instalación o ejecución en Azure Cloud Shell

La manera más fácil empezar a trabajar con la CLI de Azure es ejecutarla en un entorno de Azure Cloud Shell en su explorador. Para más información acerca de Cloud Shell, consulte [Guía de inicio rápido de Bash en Azure Cloud Shell](/azure/cloud-shell/quickstart).

Cuando esté listo para instalar la CLI, consulte las [instrucciones de instalación](install-azure-cli.md).

Después de instalar la CLI por primera vez, ejecute `az --version` para comprobar que está instalada y que tiene la versión correcta.

## <a name="sign-in"></a>Iniciar sesión

Antes de usar los comandos de la CLI en una instalación local, deberá iniciar sesión con [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Después de iniciar sesión, verá una lista de suscripciones asociadas con su cuenta de Azure. La información de suscripción con `isDefault: true` es la suscripción actualmente activada después de iniciar sesión. Para seleccionar otra suscripción, utilice el comando [az account set](/cli/azure/account#az-account-set) con el identificador de suscripción al que desea cambiar. Para más información sobre la selección de suscripción, consulte [Uso de varias suscripciones de Azure](manage-azure-subscriptions-azure-cli.md).

Hay varias formas de iniciar sesión de una manera no interactiva, que se describen con detalle en [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="common-commands"></a>Comandos comunes

En esta tabla se enumeran algunos comandos comunes utilizados en la CLI, así como vínculos a documentación de referencia.

| Tipo de recurso | Grupo de comandos de la CLI de Azure |
|---------------|-------------------------|
| [Grupos de recursos](/azure/azure-resource-manager/resource-group-overview) | [az group](/cli/azure/group) |
| [Máquinas virtuales](/azure/virtual-machines) | [az vm](/cli/azure/vm) |
| [Cuentas de almacenamiento](/azure/storage/common/storage-introduction) | [az storage account](/cli/azure/storage/account) |
| [Key Vault](/azure/key-vault/key-vault-whatis) | [az keyvault](/cli/azure/keyvault) |
| [Aplicaciones web](/azure/app-service) | [az webapp](/cli/azure/webapp) |
| [Bases de datos SQL](/azure/sql-database) | [az sql server](/cli/azure/sql/server) |
| [CosmosDB](/azure/cosmos-db) | [az cosmosdb](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a>Búsqueda de comandos

Los comandos de la CLI se organizan como _grupos_ de _comandos_. Cada grupo representa un servicio de Azure y los comandos funcionan en ese servicio.

Para buscar comandos, utilice [az find](/cli/azure/reference-index#az-find). Por ejemplo, para buscar nombres de comando que contienen `secret`, use el siguiente comando:

```azurecli-interactive
az find secret
```

Use el argumento `--help` para obtener una lista completa de los comandos y los subgrupos de un grupo. Por ejemplo, para encontrar los comandos de la CLI para trabajar con grupos de seguridad de red (NSG):

```azurecli-interactive
az network nsg --help
```

La CLI dispone de la función de autocompletar con el tabulador para los comandos en el shell de bash.

## <a name="globally-available-arguments"></a>Argumentos disponibles globalmente

Hay algunos argumentos que están disponibles para todos los comandos.

* `--help` imprime información de referencia de la CLI sobre los comandos y sus argumentos y enumera los comandos y subgrupos disponibles.
* `--output` cambia el formato de salida. Los formatos de salida disponibles son `json`, `jsonc` (JSON coloreado), `tsv` (valores separados por tabulaciones), `table` (tablas ASCII en lenguaje natural) y `yaml`. De forma predeterminada, la CLI genera `json`. Para más información sobre los formatos de salida disponibles, consulte [Formatos de salida de la CLI de Azure](format-output-azure-cli.md).
* `--query` usa el [lenguaje de consulta JMESPath](http://jmespath.org/) para filtrar los resultados devueltos por los servicios de Azure. Para más información sobre las consultas, vea [Consulta de los resultados de los comandos con la CLI de Azure](query-azure-cli.md) y [Tutorial de JMESPath](http://jmespath.org/tutorial.html).
* `--verbose` imprime información acerca de los recursos creados en Azure durante una operación y otra información de utilidad.
* `--debug` imprime más información aún sobre las operaciones de la CLI y se utiliza con fines de depuración. Si encuentra un error, proporcione la salida que se genera con la marca `--debug` activada al enviar un informe de errores.

## <a name="interactive-mode"></a>Modo interactivo

La CLI ofrece un modo interactivo que muestra automáticamente información de ayuda y facilita la selección de subcomandos. Puede entrar en el modo interactivo con el comando [az interactive](/cli/azure/reference-index#az-interactive).

```azurecli-interactive
az interactive
```

Para más información sobre el modo interactivo, consulte [Modo interactivo de la CLI de Azure](interactive-azure-cli.md).

También hay un [complemento de Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) que ofrece una experiencia interactiva, incluida la función de autocompletar y documentación al pasar el ratón.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Conozca los aspectos básicos de la CLI con las guías de inicio rápido y los tutoriales

Para ayudarle a comenzar con la CLI de Azure, pruebe con un tutorial exhaustivo sobre la configuración de máquinas virtuales y el uso de la potencia de la CLI para consultar los recursos de Azure.

> [!div class="nextstepaction"]
> [Tutorial de creación de máquinas virtuales con la CLI de Azure](azure-cli-vm-tutorial.yml)

También hay guías de inicio rápido para otros servicios populares.

* [Creación de una cuenta de almacenamiento con la CLI de Azure](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [Transferencia de objetos a y desde Azure Blob Storage mediante la CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [Creación de una base de datos de Azure SQL única con la CLI de Azure](/azure/sql-database/sql-database-get-started-cli)
* [Creación de un servidor de Azure Database for MySQL mediante la CLI de Azure](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Creación de una base de datos Azure Database for PostgreSQL con la CLI de Azure)
* [Creación de una aplicación web de Python en Azure](/azure/app-service/app-service-web-get-started-python)
* [Ejecución de una imagen personalizada de Docker Hub en Azure Web Apps for Containers](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a>Envíenos sus comentarios

Le agradecemos sus comentarios sobre la CLI para ayudarnos a mejorar y resolver errores. También puede [informar de un problema en GitHub](https://github.com/azure/azure-cli/issues) o utilizar las características integradas de la CLI para dejar comentarios generales con el comando [az feedback](/cli/azure/reference-index#az-feedback).

```azurecli-interactive
az feedback
```
