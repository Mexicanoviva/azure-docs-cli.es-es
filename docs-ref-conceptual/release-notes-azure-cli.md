---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d8307ca9797a9a780d7e08d6d21cb66446c7e289
ms.sourcegitcommit: 6d9e8ee6dd07cfd07239a2948304d7f50ef781cc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2019
ms.locfileid: "58508909"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="7046c-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7046c-103">Azure CLI release notes</span></span>
## <a name="march-26-2019"></a><span data-ttu-id="7046c-104">26 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="7046c-104">March 26, 2019</span></span>

### <a name="core"></a><span data-ttu-id="7046c-105">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-105">Core</span></span>
* <span data-ttu-id="7046c-106">Se han corregido problemas con la incompatibilidad de la extensión de desarrollo.</span><span class="sxs-lookup"><span data-stu-id="7046c-106">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="7046c-107">El control de errores ahora dirige a los clientes a la página de problemas.</span><span class="sxs-lookup"><span data-stu-id="7046c-107">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="7046c-108">Nube</span><span class="sxs-lookup"><span data-stu-id="7046c-108">Cloud</span></span>
* <span data-ttu-id="7046c-109">Se ha corregido un error de "suscripción no encontrada" en `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="7046c-109">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-110">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-110">ACR</span></span>
* <span data-ttu-id="7046c-111">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="7046c-111">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="7046c-112">Se ha agregado `--auth-mode` a los comandos `acr build`, `acr run`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-112">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="7046c-113">Se ha agregado el grupo de comandos "acr task credential" para administrar las credenciales de una tarea.</span><span class="sxs-lookup"><span data-stu-id="7046c-113">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="7046c-114">Se ha agregado "--no-wait" al comando `acr build`.</span><span class="sxs-lookup"><span data-stu-id="7046c-114">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-115">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-115">AppService</span></span>
* <span data-ttu-id="7046c-116">Se ha corregido el error por el que `webapp up` no controlaba correctamente los escenarios de ejecución desde un directorio o de código desconocido.</span><span class="sxs-lookup"><span data-stu-id="7046c-116">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="7046c-117">Se ha corregido el error por el que los espacios no funcionaban para `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="7046c-117">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="7046c-118">Servicio BOT</span><span class="sxs-lookup"><span data-stu-id="7046c-118">BOT Service</span></span>
* <span data-ttu-id="7046c-119">Se ha agregado `bot prepare-deploy` para preparar la implementación de bots mediante `webapp`.</span><span class="sxs-lookup"><span data-stu-id="7046c-119">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="7046c-120">Se ha cambiado `bot create --kind registration` para que muestre la contraseña si no se proporciona una.</span><span class="sxs-lookup"><span data-stu-id="7046c-120">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="7046c-121">[CAMBIO IMPORTANTE] Se ha cambiado `--endpoint` en `bot create --kind registration` a que sea una cadena vacía de forma predeterminada en lugar de que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="7046c-121">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="7046c-122">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="7046c-122">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="7046c-123">CDN</span><span class="sxs-lookup"><span data-stu-id="7046c-123">CDN</span></span>
* <span data-ttu-id="7046c-124">Se agregó compatibilidad para `--no-wait` a `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-124">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="7046c-125">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento de almacenamiento de cadenas de consulta en caché predeterminado de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-125">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="7046c-126">El valor predeterminado ya no es "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="7046c-126">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7046c-127">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="7046c-127">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-128">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="7046c-128">Cosmosdb</span></span>
* <span data-ttu-id="7046c-129">Se ha agregado compatibilidad con `--enable-multiple-write-locations` al actualizar la cuenta.</span><span class="sxs-lookup"><span data-stu-id="7046c-129">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="7046c-130">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="7046c-130">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-131">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-131">Interactive</span></span>
* <span data-ttu-id="7046c-132">Se ha corregido la incompatibilidad con la extensión interactiva instalada mediante azdev.</span><span class="sxs-lookup"><span data-stu-id="7046c-132">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-133">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-133">Monitor</span></span>
* <span data-ttu-id="7046c-134">Se ha cambiado para permitir el valor de dimensión `*` para `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-134">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-135">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-135">Network</span></span>
* <span data-ttu-id="7046c-136">Se ha agregado el grupo de comandos `rewrite-rule` a `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="7046c-136">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-137">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-137">Profile</span></span>
* <span data-ttu-id="7046c-138">Se ha agregado a `login` compatibilidad de la cuenta en el nivel de inquilino para la identidad de servicio administrada.</span><span class="sxs-lookup"><span data-stu-id="7046c-138">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="7046c-139">Postgres</span><span class="sxs-lookup"><span data-stu-id="7046c-139">Postgres</span></span> 
* <span data-ttu-id="7046c-140">Se han agregado los comandos postgresql `replica` y el comando `restart server`.</span><span class="sxs-lookup"><span data-stu-id="7046c-140">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="7046c-141">Se ha cambiado para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="7046c-141">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-142">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-142">Resource</span></span>
* <span data-ttu-id="7046c-143">Se ha mejorado la salida de tabla de `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-143">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="7046c-144">Se ha corregido el problema con `deployment [create|validate]` por el que no reconocía el tipo secureObject.</span><span class="sxs-lookup"><span data-stu-id="7046c-144">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="7046c-145">Grafo</span><span class="sxs-lookup"><span data-stu-id="7046c-145">Graph</span></span>
* <span data-ttu-id="7046c-146">Se agregó compatibilidad para `--end-date` a `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="7046c-146">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="7046c-147">Se ha agregado compatibilidad para agregar permisos con `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="7046c-147">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="7046c-148">Se ha corregido un error con `ad app permission list` cuando no había ningún permiso.</span><span class="sxs-lookup"><span data-stu-id="7046c-148">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="7046c-149">Se ha cambiado `ad sp delete` para omitir la eliminación de la asignación de roles si la cuenta actual no tiene ninguna suscripción.</span><span class="sxs-lookup"><span data-stu-id="7046c-149">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="7046c-150">Se ha cambiado `ad app create` para que `--identifier-uris` sea una lista vacía de forma predeterminada si no se proporciona.</span><span class="sxs-lookup"><span data-stu-id="7046c-150">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-151">storage</span><span class="sxs-lookup"><span data-stu-id="7046c-151">storage</span></span>
* <span data-ttu-id="7046c-152">Se ha agregado `--snapshot` a `storage file download-batch` para descargar desde una instantánea de recurso compartido.</span><span class="sxs-lookup"><span data-stu-id="7046c-152">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="7046c-153">Se ha cambiado la barra de progreso `storage blob [download-batch|upload-batch]` para que sea menos detallada y que indique el blob actual.</span><span class="sxs-lookup"><span data-stu-id="7046c-153">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="7046c-154">Se ha corregido el problema con `storage account update` al actualizar los parámetros de cifrado.</span><span class="sxs-lookup"><span data-stu-id="7046c-154">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="7046c-155">Se ha corregido el problema por el que `storage blob show` producía un error al usar oauth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="7046c-155">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-156">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-156">VM</span></span>
* <span data-ttu-id="7046c-157">Se agregó el comando `image update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-157">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="7046c-158">12 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="7046c-158">March 12, 2019</span></span>

<span data-ttu-id="7046c-159">Versión 2.0.60</span><span class="sxs-lookup"><span data-stu-id="7046c-159">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="7046c-160">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-160">Core</span></span>

* <span data-ttu-id="7046c-161">Se ha corregido un error incorrecto en `cloud set` sobre la suscripción no encontrada.</span><span class="sxs-lookup"><span data-stu-id="7046c-161">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-162">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-162">ACR</span></span>

* <span data-ttu-id="7046c-163">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="7046c-163">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-164">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-164">ACS</span></span>

* <span data-ttu-id="7046c-165">Se ha cambiado para ignorar el argumento `--listen-address` a `aks browse` si `kubectl` no lo admite.</span><span class="sxs-lookup"><span data-stu-id="7046c-165">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-166">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-166">AppService</span></span>

* <span data-ttu-id="7046c-167">Se ha agregado `[webapp|functionapp] deployment list-publishing-credentials` para obtener la dirección URL y sus credenciales de publicación de Kudu.</span><span class="sxs-lookup"><span data-stu-id="7046c-167">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="7046c-168">Se ha quitado la instrucción de impresión errónea para `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-168">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="7046c-169">Se ha corregido `functionapp` para establecer la imagen correcta en el entorno de ejecución en los planes de App Service de Linux</span><span class="sxs-lookup"><span data-stu-id="7046c-169">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="7046c-170">Se ha quitado la etiqueta de versión preliminar para `webapp up` y se han agregado mejoras al comando.</span><span class="sxs-lookup"><span data-stu-id="7046c-170">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="7046c-171">Botservice</span><span class="sxs-lookup"><span data-stu-id="7046c-171">Botservice</span></span>

* <span data-ttu-id="7046c-172">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="7046c-172">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7046c-173">Se han agregado `Microsoft-BotFramework-AppId` y `Microsoft-BotFramework-AppPassword` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web</span><span class="sxs-lookup"><span data-stu-id="7046c-173">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7046c-174">Se han quitado las comillas simples de la salida del comando `bot publish` al final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-174">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="7046c-175">Se ha cambiado `bot publish` para que sea asincrónico.</span><span class="sxs-lookup"><span data-stu-id="7046c-175">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="7046c-176">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-176">Container</span></span>

* <span data-ttu-id="7046c-177">Se agregó el argumento `--no-wait` a `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="7046c-177">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="7046c-178">EventHub</span><span class="sxs-lookup"><span data-stu-id="7046c-178">EventHub</span></span>

* <span data-ttu-id="7046c-179">Se ha agregado la marca `--skip-empty-archives` a `eventhub create|update` para admitir archivos vacíos en la captura.</span><span class="sxs-lookup"><span data-stu-id="7046c-179">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="7046c-180">Buscar</span><span class="sxs-lookup"><span data-stu-id="7046c-180">Find</span></span>

* <span data-ttu-id="7046c-181">Actualización de la funcionalidad principal</span><span class="sxs-lookup"><span data-stu-id="7046c-181">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7046c-182">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7046c-182">HDInsight</span></span>

* <span data-ttu-id="7046c-183">Se ha agregado el parámetro `--storage-account-managed-identity` a `hdinsight create` para admitir MSI de ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="7046c-183">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="7046c-184">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-184">Network</span></span>

* <span data-ttu-id="7046c-185">Se ha corregido un problema con `vpn-connection update` por el que no se podía actualizar una conexión VPN entre pasarelas de diferentes suscripciones.</span><span class="sxs-lookup"><span data-stu-id="7046c-185">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-186">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7046c-186">Rdbms</span></span>

* <span data-ttu-id="7046c-187">Correcciones menores para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="7046c-187">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="7046c-188">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-188">Role</span></span>

* <span data-ttu-id="7046c-189">Se ha corregido `role definition update` para usar el identificador para resolver la definición correctamente.</span><span class="sxs-lookup"><span data-stu-id="7046c-189">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="7046c-190">Se ha cambiado `ad app credential reset` para eliminar la suposición de que la entidad de servicio de la aplicación siempre existe.</span><span class="sxs-lookup"><span data-stu-id="7046c-190">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7046c-191">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7046c-191">Service Fabric</span></span>

* <span data-ttu-id="7046c-192">Se ha corregido un problema con `sf cluster list` que no se podía iterar.</span><span class="sxs-lookup"><span data-stu-id="7046c-192">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="7046c-193">26 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="7046c-193">February 26, 2019</span></span>

<span data-ttu-id="7046c-194">Versión 2.0.59</span><span class="sxs-lookup"><span data-stu-id="7046c-194">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="7046c-195">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-195">Core</span></span>

* <span data-ttu-id="7046c-196">Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.</span><span class="sxs-lookup"><span data-stu-id="7046c-196">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-197">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-197">ACR</span></span>

* <span data-ttu-id="7046c-198">Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-198">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="7046c-199">Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.</span><span class="sxs-lookup"><span data-stu-id="7046c-199">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-200">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-200">ACS</span></span>

* <span data-ttu-id="7046c-201">Se agregó la opción `--listen-address` a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="7046c-201">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-202">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-202">AppService</span></span>

* <span data-ttu-id="7046c-203">Se agregó el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="7046c-203">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-204">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-204">Batch</span></span>
* <span data-ttu-id="7046c-205">[CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="7046c-205">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="7046c-206">[CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.</span><span class="sxs-lookup"><span data-stu-id="7046c-206">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="7046c-207">Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="7046c-207">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="7046c-208">[CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`.</span><span class="sxs-lookup"><span data-stu-id="7046c-208">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="7046c-209">Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.</span><span class="sxs-lookup"><span data-stu-id="7046c-209">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="7046c-210">Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.</span><span class="sxs-lookup"><span data-stu-id="7046c-210">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-211">CosmosDB</span></span>

* <span data-ttu-id="7046c-212">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="7046c-212">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="7046c-213">Kusto</span><span class="sxs-lookup"><span data-stu-id="7046c-213">Kusto</span></span>

* <span data-ttu-id="7046c-214">[CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.</span><span class="sxs-lookup"><span data-stu-id="7046c-214">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="7046c-215">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-215">Network</span></span>

* <span data-ttu-id="7046c-216">Se agregó el argumento `--express-route-gateway-bypass` a `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-216">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="7046c-217">Se han agregado grupos de comandos desde extensiones `express-route`.</span><span class="sxs-lookup"><span data-stu-id="7046c-217">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="7046c-218">Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="7046c-218">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="7046c-219">Se agregó el argumento `--legacy-mode` a `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-219">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="7046c-220">Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-220">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="7046c-221">Se agregó el argumento `--gateway-default-site` a `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-221">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="7046c-222">Se han agregado comandos `ipsec-policy` a `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="7046c-222">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-223">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-223">Resource</span></span>

* <span data-ttu-id="7046c-224">Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7046c-224">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="7046c-225">Se ha agregado compatibilidad para el archivo de parámetros basado en URI a `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-225">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="7046c-226">Se ha agregado compatibilidad para definiciones y parámetros basados en URI para `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-226">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="7046c-227">Se ha corregido el control de parámetros y reglas para `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-227">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="7046c-228">Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.</span><span class="sxs-lookup"><span data-stu-id="7046c-228">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="7046c-229">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-229">Role</span></span>

* <span data-ttu-id="7046c-230">Se ha agregado compatibilidad con roles de aplicación a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-230">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-231">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-231">VM</span></span>

* <span data-ttu-id="7046c-232">Se ha corregido un problema con `vm create where `--acelerated-networking\` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="7046c-232">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="7046c-233">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="7046c-233">February 12, 2019</span></span>

<span data-ttu-id="7046c-234">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="7046c-234">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="7046c-235">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-235">Core</span></span>

* <span data-ttu-id="7046c-236">`az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="7046c-236">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="7046c-237">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="7046c-237">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-238">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-238">ACR</span></span>
* <span data-ttu-id="7046c-239">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="7046c-239">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="7046c-240">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.</span><span class="sxs-lookup"><span data-stu-id="7046c-240">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-241">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-241">ACS</span></span>
* <span data-ttu-id="7046c-242">Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.</span><span class="sxs-lookup"><span data-stu-id="7046c-242">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="7046c-243">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="7046c-243">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="7046c-244">Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="7046c-244">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="7046c-245">AMS</span><span class="sxs-lookup"><span data-stu-id="7046c-245">AMS</span></span>
* <span data-ttu-id="7046c-246">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-246">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="7046c-247">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-247">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-248">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-248">Appservice</span></span>
* <span data-ttu-id="7046c-249">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="7046c-249">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="7046c-250">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="7046c-250">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="7046c-251">Se ha mejorado la ayuda de `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-251">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="7046c-252">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="7046c-252">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="7046c-253">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="7046c-253">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="7046c-254">Botservice</span><span class="sxs-lookup"><span data-stu-id="7046c-254">Botservice</span></span>
* <span data-ttu-id="7046c-255">Se ha mejorado la experiencia de usuario de `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="7046c-255">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="7046c-256">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="7046c-256">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="7046c-257">Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-257">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="7046c-258">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="7046c-258">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="7046c-259">[EN DESUSO] Se ha dejado de usar el argumento `--proj-name` en favor de `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="7046c-259">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="7046c-260">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="7046c-260">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="7046c-261">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="7046c-261">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="7046c-262">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="7046c-262">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="7046c-263">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="7046c-263">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="7046c-264">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="7046c-264">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="7046c-265">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7046c-265">Key Vault</span></span>
* <span data-ttu-id="7046c-266">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.</span><span class="sxs-lookup"><span data-stu-id="7046c-266">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-267">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-267">Monitor</span></span>
* <span data-ttu-id="7046c-268">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.</span><span class="sxs-lookup"><span data-stu-id="7046c-268">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-269">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-269">Network</span></span>
* <span data-ttu-id="7046c-270">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="7046c-270">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="7046c-271">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="7046c-271">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="7046c-272">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="7046c-272">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="7046c-273">Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-273">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7046c-274">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="7046c-274">Policy Insights</span></span>
* <span data-ttu-id="7046c-275">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="7046c-275">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-276">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7046c-276">RDBMS</span></span>
* <span data-ttu-id="7046c-277">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="7046c-277">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="7046c-278">Redis</span><span class="sxs-lookup"><span data-stu-id="7046c-278">Redis</span></span>
* <span data-ttu-id="7046c-279">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="7046c-279">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="7046c-280">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="7046c-280">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="7046c-281">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="7046c-281">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="7046c-282">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="7046c-282">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="7046c-283">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="7046c-283">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="7046c-284">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="7046c-284">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="7046c-285">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="7046c-285">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="7046c-286">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-286">Role</span></span>
* <span data-ttu-id="7046c-287">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="7046c-287">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="7046c-288">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-288">SQL VM</span></span>
* <span data-ttu-id="7046c-289">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="7046c-289">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-290">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-290">VM</span></span>
* <span data-ttu-id="7046c-291">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.</span><span class="sxs-lookup"><span data-stu-id="7046c-291">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="7046c-292">Se agregó `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-292">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="7046c-293">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="7046c-293">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="7046c-294">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="7046c-294">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="7046c-295">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="7046c-295">January 31, 2019</span></span>

<span data-ttu-id="7046c-296">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="7046c-296">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="7046c-297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-297">Core</span></span>

* <span data-ttu-id="7046c-298">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="7046c-298">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="7046c-299">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="7046c-299">January 28, 2019</span></span>

<span data-ttu-id="7046c-300">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="7046c-300">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-301">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-301">ACR</span></span>
* <span data-ttu-id="7046c-302">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="7046c-302">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-303">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-303">ACS</span></span>
* <span data-ttu-id="7046c-304">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="7046c-304">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7046c-305">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="7046c-305">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="7046c-306">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="7046c-306">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="7046c-307">AMS</span><span class="sxs-lookup"><span data-stu-id="7046c-307">AMS</span></span>
* <span data-ttu-id="7046c-308">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="7046c-308">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="7046c-309">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="7046c-309">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-310">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-310">Appservice</span></span>
* <span data-ttu-id="7046c-311">Se ha agregado compatibilidad para App Insights en `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-311">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="7046c-312">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="7046c-312">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="7046c-313">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="7046c-313">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="7046c-314">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-314">Container</span></span>
* <span data-ttu-id="7046c-315">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="7046c-315">Added `container start` command</span></span>
* <span data-ttu-id="7046c-316">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="7046c-316">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7046c-317">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7046c-317">EventGrid</span></span>
* <span data-ttu-id="7046c-318">Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-318">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="7046c-319">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="7046c-319">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="7046c-320">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="7046c-320">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="7046c-321">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="7046c-321">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="7046c-322">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="7046c-322">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7046c-323">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7046c-323">HDInsight</span></span>
* <span data-ttu-id="7046c-324">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-324">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="7046c-325">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="7046c-325">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="7046c-326">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-326">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="7046c-327">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-327">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="7046c-328">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="7046c-328">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="7046c-329">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-329">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-330">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-330">IoT</span></span>
* <span data-ttu-id="7046c-331">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="7046c-331">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="7046c-332">Kusto</span><span class="sxs-lookup"><span data-stu-id="7046c-332">Kusto</span></span>
* <span data-ttu-id="7046c-333">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-333">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-334">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-334">Monitor</span></span>
* <span data-ttu-id="7046c-335">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7046c-335">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-336">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-336">Profile</span></span>
* <span data-ttu-id="7046c-337">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.</span><span class="sxs-lookup"><span data-stu-id="7046c-337">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-338">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-338">Network</span></span>
* <span data-ttu-id="7046c-339">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="7046c-339">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="7046c-340">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="7046c-340">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-341">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-341">Resource</span></span>
* <span data-ttu-id="7046c-342">Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-342">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="7046c-343">Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-343">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="7046c-344">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-344">SQL Virtual Machine</span></span>
* <span data-ttu-id="7046c-345">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-345">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-346">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-346">Storage</span></span>
* <span data-ttu-id="7046c-347">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="7046c-347">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="7046c-348">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="7046c-348">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-349">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-349">VM</span></span>
* <span data-ttu-id="7046c-350">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="7046c-350">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="7046c-351">Se ha agregado la marca `--force` a `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="7046c-351">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="7046c-352">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="7046c-352">January 15, 2019</span></span>

<span data-ttu-id="7046c-353">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="7046c-353">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-354">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-354">ACR</span></span>
* <span data-ttu-id="7046c-355">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="7046c-355">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="7046c-356">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="7046c-356">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="7046c-357">[EN DESUSO] El parámetro `--resource-group` está en desuso en los comandos:</span><span class="sxs-lookup"><span data-stu-id="7046c-357">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="7046c-358">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-358">ACS</span></span>
* <span data-ttu-id="7046c-359">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="7046c-359">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-360">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-360">Appservice</span></span>
* <span data-ttu-id="7046c-361">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="7046c-361">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="7046c-362">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="7046c-362">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="7046c-363">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="7046c-363">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="7046c-364">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="7046c-364">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="7046c-365">Botservice</span><span class="sxs-lookup"><span data-stu-id="7046c-365">Botservice</span></span>
* <span data-ttu-id="7046c-366">Se han agregado actualizaciones al estado de implementación a `bot create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-366">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="7046c-367">Configuración</span><span class="sxs-lookup"><span data-stu-id="7046c-367">Configure</span></span>
* <span data-ttu-id="7046c-368">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="7046c-368">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-369">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-369">CosmosDB</span></span>
* <span data-ttu-id="7046c-370">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="7046c-370">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7046c-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7046c-371">HDInsight</span></span>
* <span data-ttu-id="7046c-372">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="7046c-372">Added commands for managing applications</span></span>
* <span data-ttu-id="7046c-373">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="7046c-373">Added commands for managing script actions</span></span>
* <span data-ttu-id="7046c-374">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="7046c-374">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="7046c-375">Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="7046c-375">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="7046c-376">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-376">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-377">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-377">Network</span></span>
* <span data-ttu-id="7046c-378">Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-378">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="7046c-379">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="7046c-379">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="7046c-380">Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-380">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="7046c-381">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-381">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="7046c-382">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-382">Role</span></span>
* <span data-ttu-id="7046c-383">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="7046c-383">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="7046c-384">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="7046c-384">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="7046c-385">Seguridad</span><span class="sxs-lookup"><span data-stu-id="7046c-385">Security</span></span>
* <span data-ttu-id="7046c-386">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="7046c-386">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-387">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-387">Storage</span></span>
* <span data-ttu-id="7046c-388">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="7046c-388">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="7046c-389">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="7046c-389">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="7046c-390">Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="7046c-390">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="7046c-391">Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="7046c-391">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="7046c-392">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="7046c-392">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-393">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-393">VM</span></span>
* <span data-ttu-id="7046c-394">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="7046c-394">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="7046c-395">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-395">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7046c-396">Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="7046c-396">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="7046c-397">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="7046c-397">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="7046c-398">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="7046c-398">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="7046c-399">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="7046c-399">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="7046c-400">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-400">December 20, 2018</span></span>

<span data-ttu-id="7046c-401">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="7046c-401">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="7046c-402">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-402">Appservice</span></span>
* <span data-ttu-id="7046c-403">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="7046c-403">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="7046c-404">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="7046c-404">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="7046c-405">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="7046c-405">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7046c-406">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="7046c-406">IoTCentral</span></span>
* <span data-ttu-id="7046c-407">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="7046c-407">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="7046c-408">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-408">Role</span></span>
* <span data-ttu-id="7046c-409">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7046c-409">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-410">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-410">SQL</span></span>
* <span data-ttu-id="7046c-411">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="7046c-411">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-412">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-412">VM</span></span>
* <span data-ttu-id="7046c-413">Se ha agregado el parámetro `---os-type` a `disk create`</span><span class="sxs-lookup"><span data-stu-id="7046c-413">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="7046c-414">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-414">December 18, 2018</span></span>

<span data-ttu-id="7046c-415">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="7046c-415">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="7046c-416">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-416">ACR</span></span>
* <span data-ttu-id="7046c-417">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="7046c-417">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="7046c-418">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="7046c-418">Condensed the table layout for task list</span></span>
* <span data-ttu-id="7046c-419">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="7046c-419">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-420">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-420">ACS</span></span>
* <span data-ttu-id="7046c-421">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="7046c-421">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7046c-422">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-422">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="7046c-423">[EN DESUSO] Se han dejado de utilizar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="7046c-423">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="7046c-424">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="7046c-424">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="7046c-425">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="7046c-425">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="7046c-426">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="7046c-426">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-427">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-427">Appservice</span></span>
* <span data-ttu-id="7046c-428">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="7046c-428">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="7046c-429">Botservice</span><span class="sxs-lookup"><span data-stu-id="7046c-429">Botservice</span></span>
* <span data-ttu-id="7046c-430">Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-430">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="7046c-431">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="7046c-431">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="7046c-432">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="7046c-432">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="7046c-433">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="7046c-433">Reduced Kudu network calls</span></span>
* <span data-ttu-id="7046c-434">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="7046c-434">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="7046c-435">Consumo</span><span class="sxs-lookup"><span data-stu-id="7046c-435">Consumption</span></span>
* <span data-ttu-id="7046c-436">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="7046c-436">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-437">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-437">CosmosDB</span></span>
* <span data-ttu-id="7046c-438">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="7046c-438">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="7046c-439">Mapas</span><span class="sxs-lookup"><span data-stu-id="7046c-439">Maps</span></span>
* <span data-ttu-id="7046c-440">Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-440">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-441">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-441">Network</span></span>
* <span data-ttu-id="7046c-442">Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="7046c-442">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="7046c-443">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="7046c-443">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-444">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-444">Resource</span></span>
* <span data-ttu-id="7046c-445">Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-445">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="7046c-446">Se ha agregado un nuevo comando `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-446">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-447">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-447">Storage</span></span>
*  <span data-ttu-id="7046c-448">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-448">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-449">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-449">VM</span></span>
* <span data-ttu-id="7046c-450">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="7046c-450">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="7046c-451">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-451">December 4, 2018</span></span>

<span data-ttu-id="7046c-452">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="7046c-452">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="7046c-453">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-453">Core</span></span>
* <span data-ttu-id="7046c-454">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="7046c-454">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="7046c-455">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="7046c-455">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-456">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-456">Appservice</span></span>
* <span data-ttu-id="7046c-457">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="7046c-457">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="7046c-458">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="7046c-458">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="7046c-459">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-459">Network</span></span>
* <span data-ttu-id="7046c-460">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="7046c-460">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="7046c-461">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-461">Role</span></span>
* <span data-ttu-id="7046c-462">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="7046c-462">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="7046c-463">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-463">VM</span></span>
* <span data-ttu-id="7046c-464">[EN DESUSO] El parámetro `vm extension [show|wait] --expand` está en desuso</span><span class="sxs-lookup"><span data-stu-id="7046c-464">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="7046c-465">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="7046c-465">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="7046c-466">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="7046c-466">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="7046c-467">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="7046c-467">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="7046c-468">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-468">November 20, 2018</span></span>

<span data-ttu-id="7046c-469">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="7046c-469">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="7046c-470">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-470">Core</span></span>
* <span data-ttu-id="7046c-471">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="7046c-471">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-472">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-472">ACR</span></span>
* <span data-ttu-id="7046c-473">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="7046c-473">Added context token to task step</span></span>
* <span data-ttu-id="7046c-474">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="7046c-474">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="7046c-475">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="7046c-475">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-476">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-476">Appservice</span></span>
* <span data-ttu-id="7046c-477">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="7046c-477">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="7046c-478">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="7046c-478">Updated the default `node_version`.</span></span> <span data-ttu-id="7046c-479">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="7046c-479">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="7046c-480">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="7046c-480">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="7046c-481">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="7046c-481">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7046c-482">IotCentral</span><span class="sxs-lookup"><span data-stu-id="7046c-482">IotCentral</span></span>
* <span data-ttu-id="7046c-483">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7046c-483">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-484">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7046c-484">KeyVault</span></span>
* <span data-ttu-id="7046c-485">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="7046c-485">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="7046c-486">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-486">Network</span></span>
* <span data-ttu-id="7046c-487">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="7046c-487">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="7046c-488">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="7046c-488">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="7046c-489">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="7046c-489">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="7046c-490">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="7046c-490">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-491">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7046c-491">Rdbms</span></span>
* <span data-ttu-id="7046c-492">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="7046c-492">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="7046c-493">Rbac</span><span class="sxs-lookup"><span data-stu-id="7046c-493">Rbac</span></span>
* <span data-ttu-id="7046c-494">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-494">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="7046c-495">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="7046c-495">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="7046c-496">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-496">Storage</span></span>
* <span data-ttu-id="7046c-497">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="7046c-497">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="7046c-498">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="7046c-498">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="7046c-499">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="7046c-499">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="7046c-500">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7046c-500">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-501">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-501">VM</span></span>
* <span data-ttu-id="7046c-502">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="7046c-502">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="7046c-503">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="7046c-503">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="7046c-504">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="7046c-504">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="7046c-505">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="7046c-505">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="7046c-506">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-506">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="7046c-507">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-507">Added `snapshot wait` command</span></span>
* <span data-ttu-id="7046c-508">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="7046c-508">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="7046c-509">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-509">November 6, 2018</span></span>

<span data-ttu-id="7046c-510">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="7046c-510">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="7046c-511">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-511">Core</span></span>
* <span data-ttu-id="7046c-512">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="7046c-512">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-513">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-513">ACR</span></span>
* <span data-ttu-id="7046c-514">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="7046c-514">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="7046c-515">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="7046c-515">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-516">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-516">ACS</span></span>
* <span data-ttu-id="7046c-517">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7046c-517">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="7046c-518">Advisor</span><span class="sxs-lookup"><span data-stu-id="7046c-518">Advisor</span></span>
* <span data-ttu-id="7046c-519">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="7046c-519">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="7046c-520">AMS</span><span class="sxs-lookup"><span data-stu-id="7046c-520">AMS</span></span>
* <span data-ttu-id="7046c-521">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="7046c-521">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="7046c-522">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="7046c-522">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="7046c-523">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="7046c-523">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="7046c-524">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-524">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="7046c-525">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="7046c-525">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="7046c-526">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="7046c-526">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="7046c-527">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="7046c-527">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="7046c-528">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="7046c-528">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="7046c-529">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="7046c-529">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="7046c-530">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="7046c-530">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="7046c-531">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="7046c-531">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="7046c-532">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="7046c-532">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="7046c-533">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="7046c-533">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="7046c-534">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="7046c-534">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="7046c-535">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="7046c-535">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="7046c-536">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="7046c-536">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="7046c-537">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="7046c-537">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-538">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-538">AppService</span></span>
* <span data-ttu-id="7046c-539">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="7046c-539">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="7046c-540">Configuración</span><span class="sxs-lookup"><span data-stu-id="7046c-540">Configure</span></span>
* <span data-ttu-id="7046c-541">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="7046c-541">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="7046c-542">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-542">Container</span></span>
* <span data-ttu-id="7046c-543">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="7046c-543">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="7046c-544">EventHub</span><span class="sxs-lookup"><span data-stu-id="7046c-544">EventHub</span></span>
* <span data-ttu-id="7046c-545">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-545">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-546">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-546">Interactive</span></span>
* <span data-ttu-id="7046c-547">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="7046c-547">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-548">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-548">Monitor</span></span>
* <span data-ttu-id="7046c-549">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-549">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-550">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-550">Network</span></span>
* <span data-ttu-id="7046c-551">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="7046c-551">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="7046c-552">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="7046c-552">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="7046c-553">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7046c-553">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="7046c-554">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-554">Profile</span></span>
* <span data-ttu-id="7046c-555">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="7046c-555">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-556">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7046c-556">RDBMS</span></span>
* <span data-ttu-id="7046c-557">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="7046c-557">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-558">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-558">Resource</span></span>
* <span data-ttu-id="7046c-559">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="7046c-559">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="7046c-560">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-560">Role</span></span>
* <span data-ttu-id="7046c-561">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="7046c-561">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="7046c-562">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="7046c-562">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="7046c-563">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="7046c-563">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-564">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-564">Storage</span></span>
* <span data-ttu-id="7046c-565">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="7046c-565">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-566">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-566">VM</span></span>
* <span data-ttu-id="7046c-567">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="7046c-567">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="7046c-568">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="7046c-568">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="7046c-569">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="7046c-569">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="7046c-570">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="7046c-570">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="7046c-571">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="7046c-571">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="7046c-572">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="7046c-572">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="7046c-573">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-573">October 23, 2018</span></span>

<span data-ttu-id="7046c-574">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="7046c-574">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="7046c-575">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-575">Core</span></span>
* <span data-ttu-id="7046c-576">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="7046c-576">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="7046c-577">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="7046c-577">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-578">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-578">ACR</span></span>
* <span data-ttu-id="7046c-579">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="7046c-579">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="7046c-580">CDN</span><span class="sxs-lookup"><span data-stu-id="7046c-580">CDN</span></span>
* <span data-ttu-id="7046c-581">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="7046c-581">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7046c-582">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="7046c-582">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="7046c-583">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-583">Container</span></span>
* <span data-ttu-id="7046c-584">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="7046c-584">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="7046c-585">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-585">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="7046c-586">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="7046c-586">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="7046c-587">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-587">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="7046c-588">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="7046c-588">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="7046c-589">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="7046c-589">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="7046c-590">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="7046c-590">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-591">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-591">CosmosDB</span></span>
* <span data-ttu-id="7046c-592">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="7046c-592">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-593">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-593">Interactive</span></span>
* <span data-ttu-id="7046c-594">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="7046c-594">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="7046c-595">IoT Central</span><span class="sxs-lookup"><span data-stu-id="7046c-595">IoT Central</span></span>
* <span data-ttu-id="7046c-596">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7046c-596">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="7046c-597">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="7046c-597">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-598">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-598">Monitor</span></span>
* <span data-ttu-id="7046c-599">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="7046c-599">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="7046c-600">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="7046c-600">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="7046c-601">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="7046c-601">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7046c-602">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="7046c-602">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="7046c-603">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="7046c-603">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="7046c-604">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="7046c-604">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="7046c-605">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="7046c-605">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="7046c-606">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="7046c-606">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7046c-607">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="7046c-607">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="7046c-608">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7046c-608">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-609">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-609">Network</span></span>
* <span data-ttu-id="7046c-610">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="7046c-610">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="7046c-611">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="7046c-611">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="7046c-612">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7046c-612">ServiceBus</span></span>
* <span data-ttu-id="7046c-613">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="7046c-613">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-614">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-614">SQL</span></span>
* <span data-ttu-id="7046c-615">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="7046c-615">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-616">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-616">Storage</span></span>
* <span data-ttu-id="7046c-617">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="7046c-617">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="7046c-618">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="7046c-618">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-619">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-619">VM</span></span>
* <span data-ttu-id="7046c-620">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7046c-620">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="7046c-621">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7046c-621">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="7046c-622">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="7046c-622">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="7046c-623">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-623">October 16, 2018</span></span>

<span data-ttu-id="7046c-624">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="7046c-624">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-625">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-625">VM</span></span>
* <span data-ttu-id="7046c-626">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="7046c-626">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="7046c-627">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-627">October 9, 2018</span></span>

<span data-ttu-id="7046c-628">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="7046c-628">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="7046c-629">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-629">Core</span></span>
* <span data-ttu-id="7046c-630">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="7046c-630">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-631">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-631">ACR</span></span>
* <span data-ttu-id="7046c-632">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="7046c-632">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-633">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-633">ACS</span></span>
* <span data-ttu-id="7046c-634">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="7046c-634">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="7046c-635">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="7046c-635">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="7046c-636">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="7046c-636">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="7046c-637">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="7046c-637">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="7046c-638">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-638">Container</span></span>
* <span data-ttu-id="7046c-639">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="7046c-639">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="7046c-640">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="7046c-640">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="7046c-641">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="7046c-641">Event Hub</span></span>
* <span data-ttu-id="7046c-642">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="7046c-642">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="7046c-643">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="7046c-643">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="7046c-644">Extensiones</span><span class="sxs-lookup"><span data-stu-id="7046c-644">Extensions</span></span>
* <span data-ttu-id="7046c-645">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="7046c-645">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7046c-646">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7046c-646">HDInsight</span></span>
* <span data-ttu-id="7046c-647">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7046c-647">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-648">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-648">IoT</span></span>
* <span data-ttu-id="7046c-649">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="7046c-649">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-650">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7046c-650">KeyVault</span></span>
* <span data-ttu-id="7046c-651">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="7046c-651">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="7046c-652">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-652">Network</span></span>
* <span data-ttu-id="7046c-653">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7046c-653">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="7046c-654">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="7046c-654">See #6052</span></span>
* <span data-ttu-id="7046c-655">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="7046c-655">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="7046c-656">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="7046c-656">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="7046c-657">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7046c-657">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="7046c-658">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7046c-658">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="7046c-659">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="7046c-659">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="7046c-660">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="7046c-660">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="7046c-661">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-661">Role</span></span>
* <span data-ttu-id="7046c-662">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="7046c-662">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="7046c-663">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="7046c-663">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="7046c-664">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="7046c-664">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="7046c-665">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="7046c-665">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="7046c-666">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="7046c-666">Service Bus</span></span>
* <span data-ttu-id="7046c-667">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="7046c-667">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-668">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-668">VM</span></span>
* <span data-ttu-id="7046c-669">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="7046c-669">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="7046c-670">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="7046c-670">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="7046c-671">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="7046c-671">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="7046c-672">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="7046c-672">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="7046c-673">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="7046c-673">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="7046c-674">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="7046c-674">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="7046c-675">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-675">September 21, 2018</span></span>

<span data-ttu-id="7046c-676">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="7046c-676">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-677">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-677">ACR</span></span>
* <span data-ttu-id="7046c-678">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-678">Added ACR Task commands</span></span>
* <span data-ttu-id="7046c-679">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="7046c-679">Added quick run command</span></span>
* <span data-ttu-id="7046c-680">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="7046c-680">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="7046c-681">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-681">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="7046c-682">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="7046c-682">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="7046c-683">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="7046c-683">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-684">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-684">ACS</span></span>
* <span data-ttu-id="7046c-685">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="7046c-685">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="7046c-686">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="7046c-686">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-687">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-687">AppService</span></span>

* <span data-ttu-id="7046c-688">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="7046c-688">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="7046c-689">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="7046c-689">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="7046c-690">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="7046c-690">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="7046c-691">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="7046c-691">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-692">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-692">Batch</span></span>
* <span data-ttu-id="7046c-693">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="7046c-693">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="7046c-694">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="7046c-694">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="7046c-695">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="7046c-695">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="7046c-696">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="7046c-696">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7046c-697">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7046c-697">Batch AI</span></span> 
* <span data-ttu-id="7046c-698">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="7046c-698">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7046c-699">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7046c-699">Cognitive Services</span></span>
* <span data-ttu-id="7046c-700">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="7046c-700">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="7046c-701">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="7046c-701">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="7046c-702">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="7046c-702">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="7046c-703">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="7046c-703">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="7046c-704">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-704">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="7046c-705">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="7046c-705">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="7046c-706">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-706">Container</span></span>
* <span data-ttu-id="7046c-707">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="7046c-707">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="7046c-708">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="7046c-708">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="7046c-709">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-709">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="7046c-710">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-710">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="7046c-711">DataLake</span><span class="sxs-lookup"><span data-stu-id="7046c-711">Datalake</span></span>
* <span data-ttu-id="7046c-712">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-712">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="7046c-713">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="7046c-713">Interactive Shell</span></span>
* <span data-ttu-id="7046c-714">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="7046c-714">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="7046c-715">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="7046c-715">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-716">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-716">IoT</span></span>
* <span data-ttu-id="7046c-717">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-717">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="7046c-718">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7046c-718">Key Vault</span></span>
* <span data-ttu-id="7046c-719">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="7046c-719">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="7046c-720">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-720">Network</span></span>
* <span data-ttu-id="7046c-721">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="7046c-721">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="7046c-722">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="7046c-722">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="7046c-723">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="7046c-723">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="7046c-724">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="7046c-724">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="7046c-725">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="7046c-725">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="7046c-726">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="7046c-726">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="7046c-727">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="7046c-727">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="7046c-728">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="7046c-728">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="7046c-729">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="7046c-729">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="7046c-730">`network express-route create/update`: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="7046c-730">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="7046c-731">`network vnet subnet create/update`: Se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="7046c-731">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="7046c-732">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="7046c-732">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="7046c-733">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="7046c-733">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="7046c-734">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="7046c-734">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="7046c-735">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="7046c-735">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="7046c-736">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="7046c-736">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="7046c-737">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="7046c-737">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="7046c-738">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="7046c-738">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-739">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7046c-739">RDBMS</span></span>
* <span data-ttu-id="7046c-740">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="7046c-740">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="7046c-741">Reserva</span><span class="sxs-lookup"><span data-stu-id="7046c-741">Reservation</span></span>
* <span data-ttu-id="7046c-742">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="7046c-742">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="7046c-743">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="7046c-743">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="7046c-744">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="7046c-744">Manage App</span></span>
* <span data-ttu-id="7046c-745">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="7046c-745">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="7046c-746">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="7046c-746">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="7046c-747">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-747">Role</span></span>
* <span data-ttu-id="7046c-748">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="7046c-748">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="7046c-749">SignalR</span><span class="sxs-lookup"><span data-stu-id="7046c-749">SignalR</span></span>
* <span data-ttu-id="7046c-750">Primera versión</span><span class="sxs-lookup"><span data-stu-id="7046c-750">First release</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-751">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-751">Storage</span></span>
* <span data-ttu-id="7046c-752">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="7046c-752">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="7046c-753">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="7046c-753">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-754">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-754">VM</span></span>
* <span data-ttu-id="7046c-755">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="7046c-755">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="7046c-756">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="7046c-756">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="7046c-757">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-757">August 28, 2018</span></span>

<span data-ttu-id="7046c-758">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="7046c-758">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="7046c-759">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-759">Core</span></span>

* <span data-ttu-id="7046c-760">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="7046c-760">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="7046c-761">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7046c-761">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-762">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-762">ACR</span></span>

* <span data-ttu-id="7046c-763">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="7046c-763">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="7046c-764">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="7046c-764">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-765">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-765">ACS</span></span>

* <span data-ttu-id="7046c-766">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="7046c-766">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="7046c-767">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="7046c-767">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-768">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-768">AppService</span></span>

* <span data-ttu-id="7046c-769">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="7046c-769">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="7046c-770">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-770">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="7046c-771">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-771">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="7046c-772">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7046c-772">Backup</span></span>

* <span data-ttu-id="7046c-773">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-773">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="7046c-774">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="7046c-774">Bot Service</span></span>

* <span data-ttu-id="7046c-775">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="7046c-775">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7046c-776">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7046c-776">Cognitive Services</span></span>

* <span data-ttu-id="7046c-777">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="7046c-777">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-778">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-778">IoT</span></span>

* <span data-ttu-id="7046c-779">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="7046c-779">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-780">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-780">Monitor</span></span>

* <span data-ttu-id="7046c-781">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="7046c-781">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="7046c-782">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="7046c-782">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7046c-783">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-783">Network</span></span>

* <span data-ttu-id="7046c-784">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-784">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-785">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-785">Resource</span></span>

* <span data-ttu-id="7046c-786">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-786">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-787">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-787">Storage</span></span>

* <span data-ttu-id="7046c-788">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-788">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-789">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-789">VM</span></span>

* <span data-ttu-id="7046c-790">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-790">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="7046c-791">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7046c-791">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="7046c-792">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-792">Auguest 14, 2018</span></span>

<span data-ttu-id="7046c-793">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="7046c-793">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="7046c-794">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-794">Core</span></span>

* <span data-ttu-id="7046c-795">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="7046c-795">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="7046c-796">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="7046c-796">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="7046c-797">Telemetría</span><span class="sxs-lookup"><span data-stu-id="7046c-797">Telemetry</span></span>

* <span data-ttu-id="7046c-798">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="7046c-798">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-799">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-799">ACR</span></span>

* <span data-ttu-id="7046c-800">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="7046c-800">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="7046c-801">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="7046c-801">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-802">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-802">ACS</span></span>

* <span data-ttu-id="7046c-803">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="7046c-803">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="7046c-804">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="7046c-804">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="7046c-805">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="7046c-805">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="7046c-806">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="7046c-806">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="7046c-807">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="7046c-807">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="7046c-808">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-808">AppService</span></span>

* <span data-ttu-id="7046c-809">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7046c-809">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="7046c-810">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="7046c-810">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="7046c-811">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7046c-811">BatchAI</span></span>

* <span data-ttu-id="7046c-812">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="7046c-812">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="7046c-813">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-813">Container</span></span>

* <span data-ttu-id="7046c-814">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-814">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="7046c-815">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-815">IoT</span></span>

* <span data-ttu-id="7046c-816">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="7046c-816">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="7046c-817">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="7046c-817">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="7046c-818">Iot Central</span><span class="sxs-lookup"><span data-stu-id="7046c-818">Iot Central</span></span>

* <span data-ttu-id="7046c-819">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7046c-819">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-820">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7046c-820">KeyVault</span></span>


* <span data-ttu-id="7046c-821">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="7046c-821">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="7046c-822">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="7046c-822">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="7046c-823">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="7046c-823">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="7046c-824">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="7046c-824">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="7046c-825">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="7046c-825">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="7046c-826">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="7046c-826">Relay</span></span>

* <span data-ttu-id="7046c-827">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7046c-827">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-828">Sql</span><span class="sxs-lookup"><span data-stu-id="7046c-828">Sql</span></span>

* <span data-ttu-id="7046c-829">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="7046c-829">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-830">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-830">Storage</span></span>

* <span data-ttu-id="7046c-831">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="7046c-831">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="7046c-832">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="7046c-832">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="7046c-833">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="7046c-833">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="7046c-834">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="7046c-834">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="7046c-835">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-835">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-836">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-836">VM</span></span>

* <span data-ttu-id="7046c-837">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="7046c-837">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="7046c-838">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-838">July 31, 2018</span></span>

<span data-ttu-id="7046c-839">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="7046c-839">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-840">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-840">ACR</span></span>

* <span data-ttu-id="7046c-841">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-841">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="7046c-842">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="7046c-842">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-843">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-843">ACS</span></span>

* <span data-ttu-id="7046c-844">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="7046c-844">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-845">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-845">Batch</span></span>

* <span data-ttu-id="7046c-846">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="7046c-846">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="7046c-847">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-847">Container</span></span>

* <span data-ttu-id="7046c-848">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="7046c-848">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="7046c-849">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-849">Network</span></span>

* <span data-ttu-id="7046c-850">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7046c-850">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="7046c-851">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-851">Resource</span></span>

* <span data-ttu-id="7046c-852">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="7046c-852">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="7046c-853">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="7046c-853">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="7046c-854">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-854">Role</span></span>

* <span data-ttu-id="7046c-855">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="7046c-855">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="7046c-856">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="7046c-856">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="7046c-857">Search</span><span class="sxs-lookup"><span data-stu-id="7046c-857">Search</span></span>

* <span data-ttu-id="7046c-858">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="7046c-858">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="7046c-859">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="7046c-859">Service Bus</span></span>

* <span data-ttu-id="7046c-860">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="7046c-860">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="7046c-861">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="7046c-861">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="7046c-862">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="7046c-862">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="7046c-863">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="7046c-863">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-864">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-864">Storage</span></span>

* <span data-ttu-id="7046c-865">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="7046c-865">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="7046c-866">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="7046c-866">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-867">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-867">VM</span></span>

* <span data-ttu-id="7046c-868">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="7046c-868">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="7046c-869">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="7046c-869">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="7046c-870">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="7046c-870">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="7046c-871">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="7046c-871">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="7046c-872">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-872">July 18, 2018</span></span>

<span data-ttu-id="7046c-873">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="7046c-873">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="7046c-874">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-874">Core</span></span>

* <span data-ttu-id="7046c-875">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="7046c-875">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="7046c-876">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="7046c-876">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="7046c-877">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-877">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-878">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-878">ACR</span></span>

* <span data-ttu-id="7046c-879">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="7046c-879">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="7046c-880">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="7046c-880">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="7046c-881">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="7046c-881">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="7046c-882">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="7046c-882">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-883">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-883">ACS</span></span>

* <span data-ttu-id="7046c-884">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="7046c-884">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-885">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-885">AppService</span></span>

* <span data-ttu-id="7046c-886">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="7046c-886">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-887">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-887">Batch</span></span>

* <span data-ttu-id="7046c-888">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="7046c-888">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="7046c-889">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7046c-889">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7046c-890">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7046c-890">Batch AI</span></span>

* <span data-ttu-id="7046c-891">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="7046c-891">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="7046c-892">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-892">Container</span></span>

* <span data-ttu-id="7046c-893">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="7046c-893">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="7046c-894">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="7046c-894">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="7046c-895">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-895">Network</span></span>

* <span data-ttu-id="7046c-896">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="7046c-896">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="7046c-897">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-897">Added `network nic wait`</span></span>
* <span data-ttu-id="7046c-898">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="7046c-898">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="7046c-899">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="7046c-899">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="7046c-900">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-900">Resource</span></span>

* <span data-ttu-id="7046c-901">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7046c-901">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="7046c-902">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7046c-902">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="7046c-903">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-903">Added `deployment wait` command</span></span>
* <span data-ttu-id="7046c-904">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="7046c-904">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-905">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-905">SQL</span></span>

* <span data-ttu-id="7046c-906">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="7046c-906">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="7046c-907">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="7046c-907">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="7046c-908">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="7046c-908">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-909">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-909">Storage</span></span>

* <span data-ttu-id="7046c-910">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="7046c-910">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-911">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-911">VM</span></span>

* <span data-ttu-id="7046c-912">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="7046c-912">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="7046c-913">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="7046c-913">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="7046c-914">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-914">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7046c-915">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-915">July 3, 2018</span></span>

<span data-ttu-id="7046c-916">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="7046c-916">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="7046c-917">AKS</span><span class="sxs-lookup"><span data-stu-id="7046c-917">AKS</span></span>

* <span data-ttu-id="7046c-918">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="7046c-918">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7046c-919">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-919">July 3, 2018</span></span>

<span data-ttu-id="7046c-920">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="7046c-920">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="7046c-921">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-921">Core</span></span>

* <span data-ttu-id="7046c-922">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="7046c-922">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-923">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-923">ACR</span></span>

* <span data-ttu-id="7046c-924">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="7046c-924">Added polling build status</span></span>
* <span data-ttu-id="7046c-925">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="7046c-925">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="7046c-926">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="7046c-926">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-927">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-927">ACS</span></span>

* <span data-ttu-id="7046c-928">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7046c-928">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="7046c-929">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="7046c-929">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="7046c-930">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="7046c-930">Updated options for `aks browse` command.</span></span> <span data-ttu-id="7046c-931">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="7046c-931">Added `--listen-port` support</span></span>
* <span data-ttu-id="7046c-932">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="7046c-932">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="7046c-933">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="7046c-933">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="7046c-934">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="7046c-934">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-935">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-935">AppService</span></span>

* <span data-ttu-id="7046c-936">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="7046c-936">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="7046c-937">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="7046c-937">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="7046c-938">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7046c-938">Backup</span></span>

* <span data-ttu-id="7046c-939">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="7046c-939">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="7046c-940">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7046c-940">BatchAI</span></span>

* <span data-ttu-id="7046c-941">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="7046c-941">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="7046c-942">Nube</span><span class="sxs-lookup"><span data-stu-id="7046c-942">Cloud</span></span>

* <span data-ttu-id="7046c-943">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="7046c-943">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="7046c-944">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-944">Container</span></span>

* <span data-ttu-id="7046c-945">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="7046c-945">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="7046c-946">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="7046c-946">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="7046c-947">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="7046c-947">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-948">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-948">Extension</span></span>

* <span data-ttu-id="7046c-949">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="7046c-949">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="7046c-950">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-950">Network</span></span>

* <span data-ttu-id="7046c-951">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="7046c-951">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-952">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7046c-952">Rdbms</span></span>

* <span data-ttu-id="7046c-953">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="7046c-953">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-954">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-954">Resource</span></span>

* <span data-ttu-id="7046c-955">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="7046c-955">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-956">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-956">VM</span></span>

* <span data-ttu-id="7046c-957">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="7046c-957">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="7046c-958">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-958">June 25, 2018</span></span>

<span data-ttu-id="7046c-959">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="7046c-959">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="7046c-960">CLI</span><span class="sxs-lookup"><span data-stu-id="7046c-960">CLI</span></span>

* <span data-ttu-id="7046c-961">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-961">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="7046c-962">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-962">June 19, 2018</span></span>

<span data-ttu-id="7046c-963">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="7046c-963">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="7046c-964">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-964">Core</span></span>

* <span data-ttu-id="7046c-965">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-965">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-966">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-966">ACR</span></span>

* <span data-ttu-id="7046c-967">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="7046c-967">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="7046c-968">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="7046c-968">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-969">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-969">ACS</span></span>

* <span data-ttu-id="7046c-970">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="7046c-970">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="7046c-971">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="7046c-971">Added `--update` support</span></span>
* <span data-ttu-id="7046c-972">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="7046c-972">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="7046c-973">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="7046c-973">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="7046c-974">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="7046c-974">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="7046c-975">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="7046c-975">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="7046c-976">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7046c-976">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="7046c-977">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7046c-977">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-978">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-978">AppService</span></span>

* <span data-ttu-id="7046c-979">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="7046c-979">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="7046c-980">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7046c-980">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-981">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-981">Batch</span></span>

* <span data-ttu-id="7046c-982">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="7046c-982">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7046c-983">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7046c-983">Batch AI</span></span>

* <span data-ttu-id="7046c-984">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="7046c-984">Added support for workspaces.</span></span> <span data-ttu-id="7046c-985">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="7046c-985">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="7046c-986">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="7046c-986">Added support for experiments.</span></span> <span data-ttu-id="7046c-987">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="7046c-987">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="7046c-988">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="7046c-988">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="7046c-989">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="7046c-989">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="7046c-990">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="7046c-990">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="7046c-991">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="7046c-991">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="7046c-992">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="7046c-992">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="7046c-993">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="7046c-993">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="7046c-994">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-994">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="7046c-995">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="7046c-995">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="7046c-996">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-996">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="7046c-997">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="7046c-997">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="7046c-998">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="7046c-998">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="7046c-999">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="7046c-999">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="7046c-1000">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1000">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="7046c-1001">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="7046c-1001">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="7046c-1002">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="7046c-1002">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="7046c-1003">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7046c-1003">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7046c-1004">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7046c-1004">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7046c-1005">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="7046c-1005">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="7046c-1006">Mapas</span><span class="sxs-lookup"><span data-stu-id="7046c-1006">Maps</span></span>

* <span data-ttu-id="7046c-1007">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1007">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1008">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1008">Network</span></span>

* <span data-ttu-id="7046c-1009">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="7046c-1009">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="7046c-1010">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7046c-1010">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="7046c-1011">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="7046c-1011">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="7046c-1012">Reservations</span><span class="sxs-lookup"><span data-stu-id="7046c-1012">Reservations</span></span>

* <span data-ttu-id="7046c-1013">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1013">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="7046c-1014">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1014">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="7046c-1015">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1015">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="7046c-1016">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1016">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="7046c-1017">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1017">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="7046c-1018">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1018">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="7046c-1019">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-1019">Role</span></span>

* <span data-ttu-id="7046c-1020">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="7046c-1020">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1021">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1021">SQL</span></span>

* <span data-ttu-id="7046c-1022">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="7046c-1022">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1023">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1023">Storage</span></span>

* <span data-ttu-id="7046c-1024">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="7046c-1024">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1025">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1025">VM</span></span>

* <span data-ttu-id="7046c-1026">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1026">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="7046c-1027">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="7046c-1027">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="7046c-1028">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="7046c-1028">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7046c-1029">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1029">June 13, 2018</span></span>

<span data-ttu-id="7046c-1030">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="7046c-1030">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1031">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1031">Core</span></span>

* <span data-ttu-id="7046c-1032">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="7046c-1032">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7046c-1033">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1033">June 13, 2018</span></span>

<span data-ttu-id="7046c-1034">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="7046c-1034">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="7046c-1035">AKS</span><span class="sxs-lookup"><span data-stu-id="7046c-1035">AKS</span></span>

* <span data-ttu-id="7046c-1036">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1036">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="7046c-1037">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="7046c-1037">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="7046c-1038">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1038">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="7046c-1039">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1039">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="7046c-1040">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1040">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1041">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-1041">AppService</span></span>

* <span data-ttu-id="7046c-1042">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="7046c-1042">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7046c-1043">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1043">June 5, 2018</span></span>

<span data-ttu-id="7046c-1044">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="7046c-1044">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1045">Interactive</span></span>

* <span data-ttu-id="7046c-1046">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="7046c-1046">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7046c-1047">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1047">June 5, 2018</span></span>

<span data-ttu-id="7046c-1048">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="7046c-1048">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1049">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1049">Core</span></span>

* <span data-ttu-id="7046c-1050">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="7046c-1050">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="7046c-1051">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="7046c-1051">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1052">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1052">ACR</span></span>

* <span data-ttu-id="7046c-1053">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="7046c-1053">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="7046c-1054">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1054">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="7046c-1055">AKS</span><span class="sxs-lookup"><span data-stu-id="7046c-1055">AKS</span></span>

* <span data-ttu-id="7046c-1056">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="7046c-1056">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-1057">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1057">Batch</span></span>

* <span data-ttu-id="7046c-1058">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="7046c-1058">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-1059">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-1059">IOT</span></span>

* <span data-ttu-id="7046c-1060">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="7046c-1060">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1061">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1061">Network</span></span>

* <span data-ttu-id="7046c-1062">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="7046c-1062">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7046c-1063">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="7046c-1063">Policy Insights</span></span>

* <span data-ttu-id="7046c-1064">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="7046c-1064">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="7046c-1065">ARM</span><span class="sxs-lookup"><span data-stu-id="7046c-1065">ARM</span></span>

* <span data-ttu-id="7046c-1066">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1066">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1067">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1067">SQL</span></span>

* <span data-ttu-id="7046c-1068">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="7046c-1068">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="7046c-1069">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="7046c-1069">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="7046c-1070">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1070">Storage</span></span>

* <span data-ttu-id="7046c-1071">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="7046c-1071">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1072">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1072">VM</span></span>

* <span data-ttu-id="7046c-1073">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="7046c-1073">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="7046c-1074">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1074">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="7046c-1075">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1075">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="7046c-1076">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1076">May 22, 2018</span></span>

<span data-ttu-id="7046c-1077">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="7046c-1077">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1078">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1078">Core</span></span>

* <span data-ttu-id="7046c-1079">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="7046c-1079">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1080">ACS</span></span>

* <span data-ttu-id="7046c-1081">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="7046c-1081">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="7046c-1082">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="7046c-1082">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-1083">AppService</span></span>

* <span data-ttu-id="7046c-1084">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="7046c-1084">Improved generic update commands</span></span>
* <span data-ttu-id="7046c-1085">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="7046c-1085">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1086">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1086">Container</span></span>

* <span data-ttu-id="7046c-1087">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="7046c-1087">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="7046c-1088">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-1088">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1089">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1089">Extension</span></span>

* <span data-ttu-id="7046c-1090">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="7046c-1090">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1091">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1091">Interactive</span></span>

* <span data-ttu-id="7046c-1092">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="7046c-1092">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="7046c-1093">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="7046c-1093">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-1094">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7046c-1094">KeyVault</span></span>

* <span data-ttu-id="7046c-1095">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="7046c-1095">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1096">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1096">Network</span></span>

* <span data-ttu-id="7046c-1097">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="7046c-1097">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="7046c-1098">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="7046c-1098">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1099">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1099">SQL</span></span>

* <span data-ttu-id="7046c-1100">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="7046c-1100">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="7046c-1101">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="7046c-1101">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="7046c-1102">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="7046c-1102">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="7046c-1103">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="7046c-1103">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="7046c-1104">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="7046c-1104">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="7046c-1105">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1105">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="7046c-1106">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="7046c-1106">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="7046c-1107">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1107">`edition`.</span></span> <span data-ttu-id="7046c-1108">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="7046c-1108">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="7046c-1109">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1109">`elasticPoolName`.</span></span> <span data-ttu-id="7046c-1110">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="7046c-1110">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="7046c-1111">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="7046c-1111">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="7046c-1112">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1112">`edition`.</span></span> <span data-ttu-id="7046c-1113">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="7046c-1113">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="7046c-1114">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1114">`dtu`.</span></span> <span data-ttu-id="7046c-1115">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="7046c-1115">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="7046c-1116">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1116">`databaseDtuMin`.</span></span> <span data-ttu-id="7046c-1117">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="7046c-1117">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="7046c-1118">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1118">`databaseDtuMax`.</span></span> <span data-ttu-id="7046c-1119">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="7046c-1119">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="7046c-1120">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1120">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="7046c-1121">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1121">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1122">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1122">Storage</span></span>

* <span data-ttu-id="7046c-1123">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="7046c-1123">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="7046c-1124">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="7046c-1124">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1125">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1125">VM</span></span>

* <span data-ttu-id="7046c-1126">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1126">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="7046c-1127">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="7046c-1127">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="7046c-1128">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="7046c-1128">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="7046c-1129">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="7046c-1129">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="7046c-1130">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1130">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="7046c-1131">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1131">May 7, 2018</span></span>

<span data-ttu-id="7046c-1132">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="7046c-1132">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1133">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1133">Core</span></span>

* <span data-ttu-id="7046c-1134">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="7046c-1134">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="7046c-1135">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="7046c-1135">Added limited support for positional arguments</span></span>
* <span data-ttu-id="7046c-1136">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1136">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="7046c-1137">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="7046c-1137">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="7046c-1138">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1138">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="7046c-1139">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="7046c-1139">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="7046c-1140">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1140">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="7046c-1141">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="7046c-1141">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="7046c-1142">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1142">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1143">ACR</span></span>

* <span data-ttu-id="7046c-1144">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="7046c-1144">Added ACR Build commands</span></span>
* <span data-ttu-id="7046c-1145">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="7046c-1145">Improved resource not found error messages</span></span>
* <span data-ttu-id="7046c-1146">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="7046c-1146">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="7046c-1147">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="7046c-1147">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="7046c-1148">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="7046c-1148">Improved repository commands error messages</span></span>
* <span data-ttu-id="7046c-1149">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="7046c-1149">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1150">ACS</span></span>

* <span data-ttu-id="7046c-1151">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-1151">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="7046c-1152">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="7046c-1152">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="7046c-1153">AMS</span><span class="sxs-lookup"><span data-stu-id="7046c-1153">AMS</span></span>

* <span data-ttu-id="7046c-1154">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="7046c-1154">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1155">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1155">Appservice</span></span>

* <span data-ttu-id="7046c-1156">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="7046c-1156">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="7046c-1157">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1157">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="7046c-1158">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="7046c-1158">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="7046c-1159">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-1159">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7046c-1160">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7046c-1160">Batch AI</span></span>

* <span data-ttu-id="7046c-1161">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="7046c-1161">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7046c-1162">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7046c-1162">Cognitive Services</span></span>

* <span data-ttu-id="7046c-1163">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="7046c-1163">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="7046c-1164">Consumo</span><span class="sxs-lookup"><span data-stu-id="7046c-1164">Consumption</span></span>

* <span data-ttu-id="7046c-1165">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="7046c-1165">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1166">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1166">Container</span></span>

* <span data-ttu-id="7046c-1167">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="7046c-1167">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7046c-1168">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7046c-1168">Cosmos DB</span></span>

* <span data-ttu-id="7046c-1169">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7046c-1169">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="7046c-1170">DMS</span><span class="sxs-lookup"><span data-stu-id="7046c-1170">DMS</span></span>

* <span data-ttu-id="7046c-1171">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1171">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1172">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1172">Extension</span></span>

* <span data-ttu-id="7046c-1173">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="7046c-1173">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1174">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1174">Interactive</span></span>

* <span data-ttu-id="7046c-1175">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="7046c-1175">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="7046c-1176">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="7046c-1176">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="7046c-1177">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="7046c-1177">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="7046c-1178">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1178">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="7046c-1179">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-1179">Lab</span></span>

* <span data-ttu-id="7046c-1180">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="7046c-1180">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1181">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1181">Network</span></span>

* <span data-ttu-id="7046c-1182">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="7046c-1182">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="7046c-1183">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1183">Profile</span></span>

* <span data-ttu-id="7046c-1184">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1184">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="7046c-1185">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="7046c-1185">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="7046c-1186">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="7046c-1186">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="7046c-1187">Redis</span><span class="sxs-lookup"><span data-stu-id="7046c-1187">Redis</span></span>

* <span data-ttu-id="7046c-1188">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="7046c-1188">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="7046c-1189">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1189">Deprecated `redis list-all`.</span></span> <span data-ttu-id="7046c-1190">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="7046c-1190">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="7046c-1191">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="7046c-1191">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="7046c-1192">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1192">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="7046c-1193">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-1193">Role</span></span>

* <span data-ttu-id="7046c-1194">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="7046c-1194">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1195">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1195">Storage</span></span>

* <span data-ttu-id="7046c-1196">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="7046c-1196">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="7046c-1197">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="7046c-1197">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="7046c-1198">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="7046c-1198">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="7046c-1199">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="7046c-1199">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="7046c-1200">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="7046c-1200">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1201">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1201">VM</span></span>

* <span data-ttu-id="7046c-1202">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="7046c-1202">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="7046c-1203">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="7046c-1203">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="7046c-1204">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="7046c-1204">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="7046c-1205">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="7046c-1205">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="7046c-1206">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="7046c-1206">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="7046c-1207">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="7046c-1207">Added write accelerator support</span></span>
* <span data-ttu-id="7046c-1208">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1208">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="7046c-1209">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="7046c-1209">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="7046c-1210">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="7046c-1210">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="7046c-1211">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1211">April 10, 2018</span></span>

<span data-ttu-id="7046c-1212">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="7046c-1212">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1213">ACR</span></span>

* <span data-ttu-id="7046c-1214">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="7046c-1214">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1215">ACS</span></span>

* <span data-ttu-id="7046c-1216">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="7046c-1216">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1217">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1217">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="7046c-1219">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="7046c-1219">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="7046c-1220">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7046c-1220">BatchAI</span></span>

* <span data-ttu-id="7046c-1221">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="7046c-1221">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="7046c-1222">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="7046c-1222">Job level mounting</span></span>
  - <span data-ttu-id="7046c-1223">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="7046c-1223">Environment variables with secret values</span></span>
  - <span data-ttu-id="7046c-1224">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1224">Performance counters settings</span></span>
  - <span data-ttu-id="7046c-1225">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="7046c-1225">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="7046c-1226">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="7046c-1226">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="7046c-1227">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="7046c-1227">Usage and limits reporting</span></span>
  - <span data-ttu-id="7046c-1228">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="7046c-1228">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="7046c-1229">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="7046c-1229">Support for custom images</span></span>
  - <span data-ttu-id="7046c-1230">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="7046c-1230">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="7046c-1231">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="7046c-1231">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="7046c-1232">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="7046c-1232">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="7046c-1233">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="7046c-1233">National clouds are supported</span></span>
* <span data-ttu-id="7046c-1234">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="7046c-1234">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="7046c-1235">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="7046c-1235">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="7046c-1236">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="7046c-1236">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="7046c-1237">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="7046c-1237">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="7046c-1238">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="7046c-1238">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="7046c-1239">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="7046c-1239">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="7046c-1240">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1240">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="7046c-1241">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="7046c-1241">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="7046c-1242">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="7046c-1242">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="7046c-1243">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1243">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="7046c-1244">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1244">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="7046c-1245">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="7046c-1245">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="7046c-1246">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1246">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="7046c-1247">Facturación</span><span class="sxs-lookup"><span data-stu-id="7046c-1247">Billing</span></span>

* <span data-ttu-id="7046c-1248">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="7046c-1248">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="7046c-1249">Consumo</span><span class="sxs-lookup"><span data-stu-id="7046c-1249">Consumption</span></span>

* <span data-ttu-id="7046c-1250">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1250">Added `marketplace` commands</span></span>
* <span data-ttu-id="7046c-1251">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7046c-1251">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="7046c-1252">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="7046c-1252">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="7046c-1253">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="7046c-1253">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="7046c-1254">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7046c-1254">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="7046c-1255">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="7046c-1255">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1256">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1256">Container</span></span>

* <span data-ttu-id="7046c-1257">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="7046c-1257">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="7046c-1258">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="7046c-1258">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1259">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1259">Extension</span></span>

* <span data-ttu-id="7046c-1260">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="7046c-1260">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1261">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1261">Interactive</span></span>

* <span data-ttu-id="7046c-1262">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="7046c-1262">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="7046c-1263">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1263">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="7046c-1264">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="7046c-1264">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1265">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1265">Network</span></span>

* <span data-ttu-id="7046c-1266">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1266">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="7046c-1267">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1267">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="7046c-1268">4910</span><span class="sxs-lookup"><span data-stu-id="7046c-1268">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="7046c-1269">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="7046c-1269">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="7046c-1270">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="7046c-1270">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="7046c-1271">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1271">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="7046c-1272">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1272">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="7046c-1273">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="7046c-1273">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-1274">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1274">Profile</span></span>

* <span data-ttu-id="7046c-1275">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="7046c-1275">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="7046c-1276">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="7046c-1276">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-1277">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7046c-1277">RDBMS</span></span>

* <span data-ttu-id="7046c-1278">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1278">Added `georestore` command</span></span>
* <span data-ttu-id="7046c-1279">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1279">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1280">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1280">Resource</span></span>

* <span data-ttu-id="7046c-1281">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1281">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="7046c-1282">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1282">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1283">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1283">SQL</span></span>

* <span data-ttu-id="7046c-1284">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="7046c-1284">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1285">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1285">Storage</span></span>

* <span data-ttu-id="7046c-1286">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="7046c-1286">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1287">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1287">VM</span></span>

* <span data-ttu-id="7046c-1288">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1288">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="7046c-1289">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="7046c-1289">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="7046c-1291">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1291">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="7046c-1292">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="7046c-1292">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="7046c-1293">5718</span><span class="sxs-lookup"><span data-stu-id="7046c-1293">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="7046c-1294">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="7046c-1294">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="7046c-1295">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1295">March 27, 2018</span></span>

<span data-ttu-id="7046c-1296">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="7046c-1296">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1297">Core</span></span>

* <span data-ttu-id="7046c-1298">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="7046c-1298">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1299">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1299">ACS</span></span>

* <span data-ttu-id="7046c-1300">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7046c-1300">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1301">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1301">Appservice</span></span>

* <span data-ttu-id="7046c-1302">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1302">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="7046c-1303">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1303">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7046c-1304">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7046c-1304">Backup</span></span>

* <span data-ttu-id="7046c-1305">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1305">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="7046c-1306">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1306">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="7046c-1307">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="7046c-1307">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* <span data-ttu-id="7046c-1308">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="7046c-1308">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1309">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1309">Container</span></span>

* <span data-ttu-id="7046c-1310">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1310">Added `container exec` command.</span></span> <span data-ttu-id="7046c-1311">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="7046c-1311">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="7046c-1312">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-1312">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1313">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1313">Extension</span></span>

* <span data-ttu-id="7046c-1314">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-1314">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="7046c-1315">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="7046c-1315">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="7046c-1316">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7046c-1316">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1317">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1317">Interactive</span></span>

* <span data-ttu-id="7046c-1318">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1318">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="7046c-1319">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="7046c-1319">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="7046c-1320">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1320">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="7046c-1321">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="7046c-1321">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="7046c-1322">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-1322">Lab</span></span>

* <span data-ttu-id="7046c-1323">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="7046c-1323">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-1324">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1324">Monitor</span></span>

* <span data-ttu-id="7046c-1325">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7046c-1325">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="7046c-1326">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="7046c-1326">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="7046c-1327">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7046c-1327">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1328">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1328">Network</span></span>

* <span data-ttu-id="7046c-1329">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="7046c-1329">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-1330">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1330">Profile</span></span>

* <span data-ttu-id="7046c-1331">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="7046c-1331">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-1332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7046c-1332">RDBMS</span></span>

* <span data-ttu-id="7046c-1333">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="7046c-1333">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1334">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1334">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="7046c-1336">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-1336">Role</span></span>

* <span data-ttu-id="7046c-1337">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1337">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="7046c-1338">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="7046c-1338">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="7046c-1339">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1339">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="7046c-1340">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1340">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="7046c-1341">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="7046c-1341">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1342">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1342">Storage</span></span>

* <span data-ttu-id="7046c-1343">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="7046c-1343">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="7046c-1344">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="7046c-1344">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1345">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1345">VM</span></span>

* <span data-ttu-id="7046c-1346">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="7046c-1346">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="7046c-1347">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1347">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="7046c-1348">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="7046c-1348">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="7046c-1349">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="7046c-1349">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="7046c-1350">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1350">March 13, 2018</span></span>

<span data-ttu-id="7046c-1351">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="7046c-1351">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1352">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1352">ACR</span></span>

* <span data-ttu-id="7046c-1353">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1353">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="7046c-1354">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-1354">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="7046c-1355">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="7046c-1355">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1356">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1356">ACS</span></span>

* <span data-ttu-id="7046c-1357">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="7046c-1357">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="7046c-1358">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="7046c-1358">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="7046c-1359">Advisor</span><span class="sxs-lookup"><span data-stu-id="7046c-1359">Advisor</span></span>

* <span data-ttu-id="7046c-1360">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="7046c-1360">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="7046c-1361">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1361">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="7046c-1362">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="7046c-1362">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="7046c-1363">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="7046c-1363">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="7046c-1364">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1364">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1365">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1365">Appservice</span></span>

* <span data-ttu-id="7046c-1366">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-1366">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="7046c-1367">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1367">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7046c-1368">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="7046c-1368">Eventhubs</span></span>

* <span data-ttu-id="7046c-1369">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7046c-1369">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1370">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1370">Extension</span></span>

* <span data-ttu-id="7046c-1371">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="7046c-1371">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1372">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1372">Interactive</span></span>

* <span data-ttu-id="7046c-1373">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="7046c-1373">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="7046c-1374">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="7046c-1374">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="7046c-1375">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="7046c-1375">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="7046c-1376">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="7046c-1376">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-1377">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1377">Monitor</span></span>

* <span data-ttu-id="7046c-1378">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-1378">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="7046c-1379">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1379">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="7046c-1380">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1380">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="7046c-1381">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1381">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1382">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1382">Network</span></span>

* <span data-ttu-id="7046c-1383">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1383">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="7046c-1384">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="7046c-1384">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="7046c-1385">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1385">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="7046c-1386">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1386">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-1387">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1387">Profile</span></span>

* <span data-ttu-id="7046c-1388">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-1388">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="7046c-1389">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1389">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-1390">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7046c-1390">RDBMS</span></span>

* <span data-ttu-id="7046c-1391">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="7046c-1391">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="7046c-1392">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="7046c-1392">Service Bus</span></span>

* <span data-ttu-id="7046c-1393">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7046c-1393">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1394">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1394">Storage</span></span>

* <span data-ttu-id="7046c-1395">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="7046c-1395">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="7046c-1396">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="7046c-1396">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1397">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1397">VM</span></span>

* <span data-ttu-id="7046c-1398">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="7046c-1398">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="7046c-1399">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-1399">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="7046c-1400">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-1400">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="7046c-1401">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="7046c-1401">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="7046c-1402">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1402">February 27, 2018</span></span>

<span data-ttu-id="7046c-1403">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="7046c-1403">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1404">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1404">Core</span></span>

* <span data-ttu-id="7046c-1405">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="7046c-1405">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="7046c-1406">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="7046c-1406">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="7046c-1407">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="7046c-1407">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1408">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1408">ACS</span></span>

* <span data-ttu-id="7046c-1409">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7046c-1409">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="7046c-1410">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="7046c-1410">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="7046c-1411">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7046c-1411">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="7046c-1412">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="7046c-1412">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1413">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1413">Appservice</span></span>

* <span data-ttu-id="7046c-1414">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="7046c-1414">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="7046c-1415">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="7046c-1415">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7046c-1416">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7046c-1416">Cognitive Services</span></span>

* <span data-ttu-id="7046c-1417">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7046c-1417">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="7046c-1418">Consumo</span><span class="sxs-lookup"><span data-stu-id="7046c-1418">Consumption</span></span>

* <span data-ttu-id="7046c-1419">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="7046c-1419">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="7046c-1420">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="7046c-1420">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1421">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1421">Container</span></span>

* <span data-ttu-id="7046c-1422">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="7046c-1422">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1423">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1423">Network</span></span>

* <span data-ttu-id="7046c-1424">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="7046c-1424">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1425">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1425">Resource</span></span>

* <span data-ttu-id="7046c-1426">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="7046c-1426">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="7046c-1427">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-1427">Role</span></span>

* <span data-ttu-id="7046c-1428">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="7046c-1428">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1429">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1429">SQL</span></span>

* <span data-ttu-id="7046c-1430">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="7046c-1430">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1431">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1431">Storage</span></span>

* <span data-ttu-id="7046c-1432">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1432">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1433">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1433">VM</span></span>

* <span data-ttu-id="7046c-1434">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="7046c-1434">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="7046c-1435">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1435">February 13, 2018</span></span>

<span data-ttu-id="7046c-1436">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="7046c-1436">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1437">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1437">Core</span></span>

* <span data-ttu-id="7046c-1438">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="7046c-1438">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1439">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1439">ACS</span></span>

* <span data-ttu-id="7046c-1440">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1440">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="7046c-1441">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1441">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="7046c-1442">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7046c-1442">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="7046c-1443">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="7046c-1443">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="7046c-1444">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="7046c-1444">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="7046c-1445">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="7046c-1445">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="7046c-1446">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7046c-1446">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="7046c-1447">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="7046c-1447">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1448">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1448">Appservice</span></span>

* <span data-ttu-id="7046c-1449">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="7046c-1449">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="7046c-1450">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="7046c-1450">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="7046c-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="7046c-1451">CDN</span></span>

* <span data-ttu-id="7046c-1452">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1452">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1453">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1453">Container</span></span>

* <span data-ttu-id="7046c-1454">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="7046c-1454">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="7046c-1455">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-1455">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-1456">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-1456">CosmosDB</span></span>

* <span data-ttu-id="7046c-1457">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="7046c-1457">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1458">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1458">Extension</span></span>

* <span data-ttu-id="7046c-1459">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1459">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="7046c-1460">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1460">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="7046c-1461">Comentarios</span><span class="sxs-lookup"><span data-stu-id="7046c-1461">Feedback</span></span>

* <span data-ttu-id="7046c-1462">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="7046c-1462">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1463">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1463">Interactive</span></span>

* <span data-ttu-id="7046c-1464">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7046c-1464">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="7046c-1465">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="7046c-1465">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-1466">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-1466">IoT</span></span>

* <span data-ttu-id="7046c-1467">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="7046c-1467">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7046c-1468">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="7046c-1468">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7046c-1469">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1469">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="7046c-1470">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="7046c-1470">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-1471">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1471">Monitor</span></span>

* <span data-ttu-id="7046c-1472">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1472">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1473">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1473">Network</span></span>

* <span data-ttu-id="7046c-1474">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="7046c-1474">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="7046c-1475">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1475">Profile</span></span>

* <span data-ttu-id="7046c-1476">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="7046c-1476">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1477">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1477">Resource</span></span>

* <span data-ttu-id="7046c-1478">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="7046c-1478">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="7046c-1479">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-1479">Role</span></span>

* <span data-ttu-id="7046c-1480">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1480">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1481">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1481">SQL</span></span>

* <span data-ttu-id="7046c-1482">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1482">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="7046c-1483">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1483">Added `sql db rename`</span></span>
* <span data-ttu-id="7046c-1484">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="7046c-1484">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1485">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1485">Storage</span></span>

* <span data-ttu-id="7046c-1486">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="7046c-1486">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1487">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1487">VM</span></span>

* <span data-ttu-id="7046c-1488">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="7046c-1488">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="7046c-1489">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="7046c-1489">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="7046c-1490">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="7046c-1490">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="7046c-1491">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1491">January 31, 2018</span></span>

<span data-ttu-id="7046c-1492">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="7046c-1492">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1493">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1493">Core</span></span>

* <span data-ttu-id="7046c-1494">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="7046c-1494">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="7046c-1495">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="7046c-1495">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="7046c-1496">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="7046c-1496">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="7046c-1497">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="7046c-1497">Use `--verbose` to see</span></span>
* <span data-ttu-id="7046c-1498">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="7046c-1498">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1499">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1499">ACS</span></span>

* <span data-ttu-id="7046c-1500">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="7046c-1500">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="7046c-1501">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="7046c-1501">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1502">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1502">Appservice</span></span>

* <span data-ttu-id="7046c-1503">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="7046c-1503">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="7046c-1504">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="7046c-1504">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="7046c-1505">CDN</span><span class="sxs-lookup"><span data-stu-id="7046c-1505">CDN</span></span>

* <span data-ttu-id="7046c-1506">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1506">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-1507">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-1507">CosmosDB</span></span>

* <span data-ttu-id="7046c-1508">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="7046c-1508">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1509">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1509">Interactive</span></span>

* <span data-ttu-id="7046c-1510">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="7046c-1510">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1511">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1511">Network</span></span>

* <span data-ttu-id="7046c-1512">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1512">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="7046c-1513">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="7046c-1513">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="7046c-1514">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1514">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="7046c-1515">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1515">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="7046c-1516">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="7046c-1516">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="7046c-1517">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="7046c-1517">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="7046c-1518">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="7046c-1518">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="7046c-1519">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="7046c-1519">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="7046c-1520">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="7046c-1520">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="7046c-1521">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="7046c-1521">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-1522">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1522">Profile</span></span>

* <span data-ttu-id="7046c-1523">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="7046c-1523">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1524">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1524">Resource</span></span>

* <span data-ttu-id="7046c-1525">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="7046c-1525">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1526">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1526">Storage</span></span>

* <span data-ttu-id="7046c-1527">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="7046c-1527">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="7046c-1528">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="7046c-1528">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="7046c-1529">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="7046c-1529">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="7046c-1530">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1530">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="7046c-1531">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="7046c-1531">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1532">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1532">VM</span></span>

* <span data-ttu-id="7046c-1533">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="7046c-1533">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="7046c-1534">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="7046c-1534">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="7046c-1535">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="7046c-1535">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="7046c-1536">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1536">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="7046c-1537">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="7046c-1537">January 17, 2018</span></span>

<span data-ttu-id="7046c-1538">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="7046c-1538">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1539">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1539">ACR</span></span>

* <span data-ttu-id="7046c-1540">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="7046c-1540">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="7046c-1541">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="7046c-1541">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1542">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1542">ACS</span></span>

* <span data-ttu-id="7046c-1543">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="7046c-1543">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="7046c-1544">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="7046c-1544">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1545">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1545">Appservice</span></span>

* <span data-ttu-id="7046c-1546">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="7046c-1546">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="7046c-1547">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="7046c-1547">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="7046c-1548">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="7046c-1548">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="7046c-1549">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7046c-1549">Backup</span></span>

* <span data-ttu-id="7046c-1550">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="7046c-1550">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="7046c-1551">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="7046c-1551">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="7046c-1552">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="7046c-1552">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="7046c-1553">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="7046c-1553">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="7046c-1554">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7046c-1554">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-1555">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1555">Batch</span></span>

* <span data-ttu-id="7046c-1556">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="7046c-1556">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="7046c-1557">Nube</span><span class="sxs-lookup"><span data-stu-id="7046c-1557">Cloud</span></span>

* <span data-ttu-id="7046c-1558">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="7046c-1558">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="7046c-1559">Consumo</span><span class="sxs-lookup"><span data-stu-id="7046c-1559">Consumption</span></span>

* <span data-ttu-id="7046c-1560">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="7046c-1560">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="7046c-1561">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7046c-1561">Event Grid</span></span>

* <span data-ttu-id="7046c-1562">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7046c-1562">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7046c-1563">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7046c-1563">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7046c-1564">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1564">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="7046c-1565">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="7046c-1565">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="7046c-1566">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1566">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="7046c-1567">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1567">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="7046c-1568">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="7046c-1568">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="7046c-1569">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="7046c-1569">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-1570">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-1570">Interactive</span></span>

* <span data-ttu-id="7046c-1571">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="7046c-1571">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="7046c-1572">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="7046c-1572">Fixed errors on startup</span></span>
* <span data-ttu-id="7046c-1573">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="7046c-1573">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-1574">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-1574">IoT</span></span>

* <span data-ttu-id="7046c-1575">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7046c-1575">Added support for device provisioning service</span></span>
* <span data-ttu-id="7046c-1576">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1576">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="7046c-1577">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-1577">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-1578">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1578">Monitor</span></span>

* <span data-ttu-id="7046c-1579">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="7046c-1579">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="7046c-1580">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1580">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="7046c-1581">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="7046c-1581">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1582">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1582">Network</span></span>

* <span data-ttu-id="7046c-1583">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1583">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="7046c-1584">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1584">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-1585">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1585">Profile</span></span>

* <span data-ttu-id="7046c-1586">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="7046c-1586">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="7046c-1587">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-1587">Role</span></span>

* <span data-ttu-id="7046c-1588">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="7046c-1588">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7046c-1589">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7046c-1589">Service Fabric</span></span>

* <span data-ttu-id="7046c-1590">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="7046c-1590">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="7046c-1591">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="7046c-1591">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1592">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1592">VM</span></span>

* <span data-ttu-id="7046c-1593">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="7046c-1593">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="7046c-1594">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="7046c-1594">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="7046c-1595">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="7046c-1595">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="7046c-1596">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="7046c-1596">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="7046c-1597">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="7046c-1597">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="7046c-1598">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1598">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7046c-1599">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1599">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="7046c-1600">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="7046c-1600">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="7046c-1601">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1601">December 19, 2017</span></span>

<span data-ttu-id="7046c-1602">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="7046c-1602">Version 2.0.23</span></span>

* <span data-ttu-id="7046c-1603">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="7046c-1603">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1604">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1604">Container</span></span>

* <span data-ttu-id="7046c-1605">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1605">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1606">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1606">Network</span></span>

* <span data-ttu-id="7046c-1607">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1607">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="7046c-1608">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1608">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1609">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1609">Storage</span></span>

* <span data-ttu-id="7046c-1610">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="7046c-1610">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1611">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1611">VM</span></span>

* <span data-ttu-id="7046c-1612">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="7046c-1612">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="7046c-1613">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1613">December 5, 2017</span></span>

<span data-ttu-id="7046c-1614">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="7046c-1614">Version 2.0.22</span></span>

* <span data-ttu-id="7046c-1615">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1615">Removed `az component` commands.</span></span> <span data-ttu-id="7046c-1616">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="7046c-1616">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1617">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1617">Core</span></span>
* <span data-ttu-id="7046c-1618">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="7046c-1618">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="7046c-1619">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="7046c-1619">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1620">ACS</span></span>

* <span data-ttu-id="7046c-1621">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="7046c-1621">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="7046c-1622">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1622">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="7046c-1623">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="7046c-1623">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="7046c-1624">Advisor</span><span class="sxs-lookup"><span data-stu-id="7046c-1624">Advisor</span></span>

* <span data-ttu-id="7046c-1625">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7046c-1625">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1626">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1626">Appservice</span></span>

* <span data-ttu-id="7046c-1627">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="7046c-1627">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="7046c-1628">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="7046c-1628">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="7046c-1629">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="7046c-1629">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="7046c-1630">Consumo</span><span class="sxs-lookup"><span data-stu-id="7046c-1630">Consumption</span></span>

* <span data-ttu-id="7046c-1631">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="7046c-1631">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1632">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1632">Container</span></span>

* <span data-ttu-id="7046c-1633">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="7046c-1633">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-1634">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1634">Monitor</span></span>

* <span data-ttu-id="7046c-1635">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="7046c-1635">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1636">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1636">Resource</span></span>

* <span data-ttu-id="7046c-1637">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="7046c-1637">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="7046c-1638">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-1638">Role</span></span>

* <span data-ttu-id="7046c-1639">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="7046c-1639">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="7046c-1640">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="7046c-1640">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="7046c-1641">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7046c-1641">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1642">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1642">SQL</span></span>

* <span data-ttu-id="7046c-1643">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="7046c-1643">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="7046c-1644">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1644">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1645">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1645">VM</span></span>

* <span data-ttu-id="7046c-1646">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="7046c-1646">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="7046c-1647">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1647">November 14, 2017</span></span>

<span data-ttu-id="7046c-1648">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="7046c-1648">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1649">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1649">ACR</span></span>

* <span data-ttu-id="7046c-1650">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="7046c-1650">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="7046c-1651">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1651">ACS</span></span>

* <span data-ttu-id="7046c-1652">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="7046c-1652">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="7046c-1653">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1653">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="7046c-1654">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="7046c-1654">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="7046c-1655">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="7046c-1655">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="7046c-1656">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="7046c-1656">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1657">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1657">Appservice</span></span>

* <span data-ttu-id="7046c-1658">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="7046c-1658">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="7046c-1659">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7046c-1659">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="7046c-1660">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7046c-1660">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="7046c-1661">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="7046c-1661">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="7046c-1662">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="7046c-1662">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="7046c-1663">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="7046c-1663">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-1664">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1664">Batch</span></span>

* <span data-ttu-id="7046c-1665">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="7046c-1665">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="7046c-1666">Batchai</span><span class="sxs-lookup"><span data-stu-id="7046c-1666">Batchai</span></span>

* <span data-ttu-id="7046c-1667">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1667">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="7046c-1668">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1668">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="7046c-1669">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="7046c-1669">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="7046c-1670">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1670">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="7046c-1671">Nube</span><span class="sxs-lookup"><span data-stu-id="7046c-1671">Cloud</span></span>

* <span data-ttu-id="7046c-1672">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="7046c-1672">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1673">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1673">Container</span></span>

* <span data-ttu-id="7046c-1674">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="7046c-1674">Added support to open multiple ports</span></span>
* <span data-ttu-id="7046c-1675">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7046c-1675">Added container group restart policy</span></span>
* <span data-ttu-id="7046c-1676">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="7046c-1676">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="7046c-1677">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="7046c-1677">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7046c-1678">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7046c-1678">Data Lake Analytics</span></span>

* <span data-ttu-id="7046c-1679">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="7046c-1679">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7046c-1680">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7046c-1680">Data Lake Store</span></span>

* <span data-ttu-id="7046c-1681">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="7046c-1681">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1682">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1682">Extension</span></span>

* <span data-ttu-id="7046c-1683">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="7046c-1683">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="7046c-1684">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="7046c-1684">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-1685">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-1685">IoT</span></span>

* <span data-ttu-id="7046c-1686">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="7046c-1686">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-1687">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1687">Monitor</span></span>

* <span data-ttu-id="7046c-1688">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1688">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1689">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1689">Network</span></span>

* <span data-ttu-id="7046c-1690">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="7046c-1690">Added support for CAA DNS records</span></span>
* <span data-ttu-id="7046c-1691">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1691">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="7046c-1692">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1692">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="7046c-1693">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="7046c-1693">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="7046c-1694">Reservations</span><span class="sxs-lookup"><span data-stu-id="7046c-1694">Reservations</span></span>

* <span data-ttu-id="7046c-1695">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="7046c-1695">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1696">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1696">Resource</span></span>

* <span data-ttu-id="7046c-1697">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1697">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1698">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1698">SQL</span></span>

* <span data-ttu-id="7046c-1699">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1699">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1700">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1700">Storage</span></span>

* <span data-ttu-id="7046c-1701">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="7046c-1701">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="7046c-1702">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="7046c-1702">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="7046c-1703">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="7046c-1703">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="7046c-1704">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="7046c-1704">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="7046c-1705">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1705">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="7046c-1706">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="7046c-1706">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="7046c-1707">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="7046c-1707">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1708">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1708">VM</span></span>

* <span data-ttu-id="7046c-1709">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="7046c-1709">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="7046c-1710">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="7046c-1710">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="7046c-1711">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="7046c-1711">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="7046c-1712">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1712">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="7046c-1713">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7046c-1713">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="7046c-1714">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1714">October 24, 2017</span></span>

<span data-ttu-id="7046c-1715">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="7046c-1715">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1716">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1716">Core</span></span>

* <span data-ttu-id="7046c-1717">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="7046c-1717">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1718">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1718">ACR</span></span>

* <span data-ttu-id="7046c-1719">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="7046c-1719">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="7046c-1720">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="7046c-1720">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="7046c-1721">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="7046c-1721">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1722">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1722">ACS</span></span>

* <span data-ttu-id="7046c-1723">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="7046c-1723">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="7046c-1724">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7046c-1724">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1725">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1725">Appservice</span></span>

* <span data-ttu-id="7046c-1726">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="7046c-1726">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="7046c-1727">Componente</span><span class="sxs-lookup"><span data-stu-id="7046c-1727">Component</span></span>

* <span data-ttu-id="7046c-1728">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="7046c-1728">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-1729">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-1729">Monitor</span></span>

* <span data-ttu-id="7046c-1730">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1730">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1731">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1731">Resource</span></span>

* <span data-ttu-id="7046c-1732">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="7046c-1732">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="7046c-1733">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="7046c-1733">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1734">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1734">VM</span></span>

* <span data-ttu-id="7046c-1735">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1735">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="7046c-1736">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1736">October 9, 2017</span></span>

<span data-ttu-id="7046c-1737">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="7046c-1737">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1738">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1738">Core</span></span>

* <span data-ttu-id="7046c-1739">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7046c-1739">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1740">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1740">Appservice</span></span>

* <span data-ttu-id="7046c-1741">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1741">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-1742">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1742">Batch</span></span>

* <span data-ttu-id="7046c-1743">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="7046c-1743">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="7046c-1744">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="7046c-1744">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="7046c-1745">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1745">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="7046c-1746">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="7046c-1746">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="7046c-1747">Batchai</span><span class="sxs-lookup"><span data-stu-id="7046c-1747">Batchai</span></span>

* <span data-ttu-id="7046c-1748">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1748">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-1749">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7046c-1749">Keyvault</span></span>

* <span data-ttu-id="7046c-1750">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7046c-1750">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="7046c-1751">(#4448)</span><span class="sxs-lookup"><span data-stu-id="7046c-1751">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="7046c-1752">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1752">Network</span></span>

* <span data-ttu-id="7046c-1753">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="7046c-1753">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="7046c-1754">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="7046c-1754">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1755">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1755">Resource</span></span>

* <span data-ttu-id="7046c-1756">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1756">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="7046c-1757">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="7046c-1757">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="7046c-1758">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="7046c-1758">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="7046c-1759">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1759">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1760">Sql</span><span class="sxs-lookup"><span data-stu-id="7046c-1760">Sql</span></span>

* <span data-ttu-id="7046c-1761">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="7046c-1761">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="7046c-1762">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="7046c-1762">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="7046c-1763">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="7046c-1763">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1764">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1764">Storage</span></span>

* <span data-ttu-id="7046c-1765">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="7046c-1765">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1766">Vm</span><span class="sxs-lookup"><span data-stu-id="7046c-1766">Vm</span></span>

* <span data-ttu-id="7046c-1767">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="7046c-1767">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="7046c-1768">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1768">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="7046c-1769">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7046c-1769">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="7046c-1770">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1770">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="7046c-1771">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1771">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="7046c-1772">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1772">September 22, 2017</span></span>

<span data-ttu-id="7046c-1773">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="7046c-1773">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1774">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1774">Resource</span></span>

* <span data-ttu-id="7046c-1775">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="7046c-1775">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="7046c-1776">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="7046c-1776">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="7046c-1777">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1777">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="7046c-1778">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="7046c-1778">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1779">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1779">Network</span></span>

* <span data-ttu-id="7046c-1780">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="7046c-1780">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="7046c-1781">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="7046c-1781">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="7046c-1782">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="7046c-1782">Added `asg` application security group commands</span></span>
* <span data-ttu-id="7046c-1783">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1783">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="7046c-1784">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1784">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7046c-1785">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1785">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="7046c-1786">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1786">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1787">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1787">Storage</span></span>

* <span data-ttu-id="7046c-1788">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="7046c-1788">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7046c-1789">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="7046c-1789">Eventgrid</span></span>

* <span data-ttu-id="7046c-1790">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="7046c-1790">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1791">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1791">SQL</span></span>

* <span data-ttu-id="7046c-1792">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="7046c-1792">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="7046c-1793">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="7046c-1793">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="7046c-1794">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1794">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-1795">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7046c-1795">Keyvault</span></span>

* <span data-ttu-id="7046c-1796">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="7046c-1796">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1797">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1797">VM</span></span>

* <span data-ttu-id="7046c-1798">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1798">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="7046c-1799">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="7046c-1799">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="7046c-1800">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1800">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="7046c-1801">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="7046c-1801">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="7046c-1802">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="7046c-1802">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="7046c-1803">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="7046c-1803">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1804">ACS</span></span>

* <span data-ttu-id="7046c-1805">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1805">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1806">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1806">Appservice</span></span>

* <span data-ttu-id="7046c-1807">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1807">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7046c-1808">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7046c-1808">Backup</span></span>

* <span data-ttu-id="7046c-1809">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-1809">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="7046c-1810">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1810">September 11, 2017</span></span>

<span data-ttu-id="7046c-1811">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="7046c-1811">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="7046c-1812">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1812">Core</span></span>

* <span data-ttu-id="7046c-1813">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="7046c-1813">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="7046c-1814">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="7046c-1814">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1815">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1815">Acs</span></span>

* <span data-ttu-id="7046c-1816">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1816">Added `acs list-locations` command</span></span>
* <span data-ttu-id="7046c-1817">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="7046c-1817">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1818">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1818">Appservice</span></span>

* <span data-ttu-id="7046c-1819">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="7046c-1819">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="7046c-1820">CDN</span><span class="sxs-lookup"><span data-stu-id="7046c-1820">CDN</span></span>

* <span data-ttu-id="7046c-1821">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7046c-1821">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="7046c-1822">Extensión</span><span class="sxs-lookup"><span data-stu-id="7046c-1822">Extension</span></span>

* <span data-ttu-id="7046c-1823">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="7046c-1823">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-1824">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7046c-1824">Keyvault</span></span>

* <span data-ttu-id="7046c-1825">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="7046c-1825">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1826">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1826">Network</span></span>

* <span data-ttu-id="7046c-1827">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1827">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7046c-1828">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1828">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="7046c-1829">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1829">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="7046c-1830">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1830">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7046c-1831">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1831">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-1832">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-1832">Resource</span></span>

* <span data-ttu-id="7046c-1833">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1833">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="7046c-1834">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1834">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="7046c-1835">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="7046c-1835">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="7046c-1836">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="7046c-1836">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-1837">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-1837">SQL</span></span>

* <span data-ttu-id="7046c-1838">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1838">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1839">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1839">VM</span></span>

* <span data-ttu-id="7046c-1840">Problema corregido: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1840">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="7046c-1841">Problema corregido: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="7046c-1841">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="7046c-1842">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1842">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="7046c-1843">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="7046c-1843">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="7046c-1844">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="7046c-1844">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="7046c-1845">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1845">August 31, 2017</span></span>

<span data-ttu-id="7046c-1846">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="7046c-1846">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-1847">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7046c-1847">Keyvault</span></span>

* <span data-ttu-id="7046c-1848">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1848">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="7046c-1849">Sf</span><span class="sxs-lookup"><span data-stu-id="7046c-1849">Sf</span></span>

* <span data-ttu-id="7046c-1850">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="7046c-1850">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1851">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1851">Storage</span></span>

* <span data-ttu-id="7046c-1852">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="7046c-1852">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="7046c-1853">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="7046c-1853">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="7046c-1854">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1854">August 28, 2017</span></span>

<span data-ttu-id="7046c-1855">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="7046c-1855">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="7046c-1856">CLI</span><span class="sxs-lookup"><span data-stu-id="7046c-1856">CLI</span></span>

* <span data-ttu-id="7046c-1857">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="7046c-1857">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1858">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1858">ACS</span></span>

* <span data-ttu-id="7046c-1859">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-1859">Corrected preview regions</span></span>
* <span data-ttu-id="7046c-1860">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="7046c-1860">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="7046c-1861">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="7046c-1861">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1862">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1862">Appservice</span></span>

* <span data-ttu-id="7046c-1863">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1863">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="7046c-1864">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1864">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="7046c-1865">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1865">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="7046c-1866">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="7046c-1866">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="7046c-1867">Problema corregido: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="7046c-1867">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-1868">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-1868">IoT</span></span>

* <span data-ttu-id="7046c-1869">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="7046c-1869">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1870">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1870">Network</span></span>

* <span data-ttu-id="7046c-1871">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="7046c-1871">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7046c-1872">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7046c-1872">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="7046c-1873">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1873">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7046c-1874">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1874">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7046c-1875">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1875">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-1876">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1876">Profile</span></span>

* <span data-ttu-id="7046c-1877">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="7046c-1877">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7046c-1878">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7046c-1878">Service Fabric</span></span>

* <span data-ttu-id="7046c-1879">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-1879">Preview release</span></span>
* <span data-ttu-id="7046c-1880">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="7046c-1880">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="7046c-1881">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="7046c-1881">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="7046c-1882">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1882">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1883">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1883">Storage</span></span>

* <span data-ttu-id="7046c-1884">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="7046c-1884">Enabled setting blob tier</span></span>
* <span data-ttu-id="7046c-1885">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="7046c-1885">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="7046c-1886">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1886">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="7046c-1887">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="7046c-1887">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="7046c-1888">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="7046c-1888">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="7046c-1889">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="7046c-1889">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1890">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1890">VM</span></span>

* <span data-ttu-id="7046c-1891">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1891">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="7046c-1892">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1892">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="7046c-1893">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1893">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="7046c-1894">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="7046c-1894">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="7046c-1895">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="7046c-1895">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="7046c-1896">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1896">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="7046c-1897">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1897">August 15, 2017</span></span>

<span data-ttu-id="7046c-1898">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="7046c-1898">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1899">ACS</span></span>

* <span data-ttu-id="7046c-1900">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7046c-1900">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1901">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1901">Appservice</span></span>

* <span data-ttu-id="7046c-1902">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="7046c-1902">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="7046c-1903">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7046c-1903">Event Grid</span></span>

* <span data-ttu-id="7046c-1904">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="7046c-1904">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="7046c-1905">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1905">August 11, 2017</span></span>

<span data-ttu-id="7046c-1906">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="7046c-1906">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1907">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1907">ACS</span></span>

* <span data-ttu-id="7046c-1908">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-1908">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-1909">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1909">Batch</span></span>

* <span data-ttu-id="7046c-1910">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="7046c-1910">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="7046c-1911">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="7046c-1911">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="7046c-1912">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="7046c-1912">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="7046c-1913">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="7046c-1913">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="7046c-1914">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="7046c-1914">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="7046c-1915">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="7046c-1915">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="7046c-1916">Componente</span><span class="sxs-lookup"><span data-stu-id="7046c-1916">Component</span></span>

* <span data-ttu-id="7046c-1917">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="7046c-1917">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="7046c-1918">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7046c-1918">Container</span></span>

* <span data-ttu-id="7046c-1919">`create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="7046c-1919">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="7046c-1920">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7046c-1920">Data Lake Store</span></span>

* <span data-ttu-id="7046c-1921">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="7046c-1921">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="7046c-1922">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7046c-1922">Event Grid</span></span>

* <span data-ttu-id="7046c-1923">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7046c-1923">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="7046c-1924">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-1924">Network</span></span>

* <span data-ttu-id="7046c-1925">`lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="7046c-1925">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="7046c-1926">`application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1926">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="7046c-1927">`application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="7046c-1927">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="7046c-1928">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1928">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-1929">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-1929">Profile</span></span>

* <span data-ttu-id="7046c-1930">`account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="7046c-1930">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-1931">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-1931">Storage</span></span>

* <span data-ttu-id="7046c-1932">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="7046c-1932">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-1933">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-1933">VM</span></span>

* <span data-ttu-id="7046c-1934">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="7046c-1934">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="7046c-1935">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1935">Exposed `list-skus` command</span></span>
* <span data-ttu-id="7046c-1936">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="7046c-1936">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="7046c-1937">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="7046c-1937">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="7046c-1938">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="7046c-1938">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="7046c-1939">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-1939">July 28, 2017</span></span>

<span data-ttu-id="7046c-1940">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="7046c-1940">Version 2.0.12</span></span>

* <span data-ttu-id="7046c-1941">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="7046c-1941">Added container commands</span></span>
* <span data-ttu-id="7046c-1942">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="7046c-1942">Added billing and consumption modules</span></span>

```text
azure-cli (2.0.12)

acr (2.0.9)
acs (2.0.11)
appservice (0.1.11)
batch (3.0.3)
billing (0.1.3)
cdn (0.0.6)
cloud (2.0.7)
cognitiveservices (0.1.6)
command-modules-nspkg (2.0.1)
component (2.0.6)
configure (2.0.10)
consumption (0.1.3)
container (0.1.7)
core (2.0.12)
cosmosdb (0.1.11)
dla (0.0.10)
dls (0.0.11)
feedback (2.0.6)
find (0.2.6)
interactive (0.3.7)
iot (0.1.10)
keyvault (2.0.8)
lab (0.0.9)
monitor (0.0.8)
network (2.0.11)
nspkg (3.0.1)
profile (2.0.9)
rdbms (0.0.5)
redis (0.2.7)
resource (2.0.11)
role (2.0.9)
sf (1.0.5)
sql (2.0.8)
storage (2.0.11)
vm (2.0.11)
```

### <a name="core"></a><span data-ttu-id="7046c-1943">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-1943">Core</span></span>

* <span data-ttu-id="7046c-1944">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="7046c-1944">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="7046c-1945">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="7046c-1945">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="7046c-1946">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="7046c-1946">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="7046c-1947">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="7046c-1947">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="7046c-1948">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="7046c-1948">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="7046c-1949">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="7046c-1949">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="7046c-1950">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="7046c-1950">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7046c-1951">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="7046c-1951">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="7046c-1952">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="7046c-1952">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="7046c-1953">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="7046c-1953">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="7046c-1954">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="7046c-1954">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="7046c-1955">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="7046c-1955">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="7046c-1956">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7046c-1956">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="7046c-1957">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7046c-1957">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="7046c-1958">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7046c-1958">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="7046c-1959">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="7046c-1959">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="7046c-1960">ACR</span><span class="sxs-lookup"><span data-stu-id="7046c-1960">ACR</span></span>

* <span data-ttu-id="7046c-1961">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="7046c-1961">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="7046c-1962">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="7046c-1962">Support SKU update for managed registries</span></span>
* <span data-ttu-id="7046c-1963">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="7046c-1963">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="7046c-1964">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="7046c-1964">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="7046c-1965">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="7046c-1965">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="7046c-1966">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="7046c-1966">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-1967">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-1967">ACS</span></span>

* <span data-ttu-id="7046c-1968">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="7046c-1968">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-1969">Appservice</span><span class="sxs-lookup"><span data-stu-id="7046c-1969">Appservice</span></span>

* <span data-ttu-id="7046c-1970">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="7046c-1970">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="7046c-1971">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="7046c-1971">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="7046c-1972">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1972">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="7046c-1973">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="7046c-1973">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="7046c-1974">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="7046c-1974">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="7046c-1975">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="7046c-1975">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="7046c-1976">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="7046c-1976">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="7046c-1977">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="7046c-1977">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="7046c-1978">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="7046c-1978">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="7046c-1979">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="7046c-1979">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="7046c-1980">Batch</span><span class="sxs-lookup"><span data-stu-id="7046c-1980">Batch</span></span>

* <span data-ttu-id="7046c-1981">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="7046c-1981">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="7046c-1982">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1982">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="7046c-1983">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1983">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="7046c-1984">CDN</span><span class="sxs-lookup"><span data-stu-id="7046c-1984">CDN</span></span>

* <span data-ttu-id="7046c-1985">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="7046c-1985">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="7046c-1986">Nube</span><span class="sxs-lookup"><span data-stu-id="7046c-1986">Cloud</span></span>

* <span data-ttu-id="7046c-1987">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7046c-1987">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="7046c-1988">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="7046c-1988">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="7046c-1989">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="7046c-1989">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="7046c-1990">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="7046c-1990">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="7046c-1991">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1991">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-1992">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-1992">CosmosDB</span></span>

* <span data-ttu-id="7046c-1993">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="7046c-1993">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="7046c-1994">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="7046c-1994">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7046c-1995">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7046c-1995">Data Lake Analytics</span></span>

* <span data-ttu-id="7046c-1996">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1996">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="7046c-1997">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1997">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="7046c-1998">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="7046c-1998">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7046c-1999">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7046c-1999">Data Lake Store</span></span>

* <span data-ttu-id="7046c-2000">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2000">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="7046c-2001">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="7046c-2001">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="7046c-2002">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2002">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="7046c-2003">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7046c-2003">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="7046c-2004">Interactive</span><span class="sxs-lookup"><span data-stu-id="7046c-2004">Interactive</span></span>

* <span data-ttu-id="7046c-2005">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="7046c-2005">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="7046c-2006">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="7046c-2006">Increased test coverage</span></span>
* <span data-ttu-id="7046c-2007">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="7046c-2007">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="7046c-2008">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="7046c-2008">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="7046c-2009">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="7046c-2009">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="7046c-2010">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="7046c-2010">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="7046c-2011">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="7046c-2011">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7046c-2012">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2012">Added `--progress` flag</span></span>
* <span data-ttu-id="7046c-2013">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="7046c-2013">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="7046c-2014">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="7046c-2014">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="7046c-2015">IoT</span><span class="sxs-lookup"><span data-stu-id="7046c-2015">IoT</span></span>

* <span data-ttu-id="7046c-2016">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="7046c-2016">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="7046c-2017">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="7046c-2017">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="7046c-2018">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="7046c-2018">Key vault</span></span>

* <span data-ttu-id="7046c-2019">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="7046c-2019">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="7046c-2020">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7046c-2020">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="7046c-2021">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7046c-2021">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7046c-2022">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7046c-2022">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7046c-2023">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7046c-2023">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="7046c-2024">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="7046c-2024">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="7046c-2025">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="7046c-2025">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="7046c-2026">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="7046c-2026">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="7046c-2027">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-2027">Lab</span></span>

* <span data-ttu-id="7046c-2028">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2028">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="7046c-2029">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2029">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-2030">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-2030">Monitor</span></span>

* <span data-ttu-id="7046c-2031">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="7046c-2031">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="7046c-2032">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2032">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="7046c-2033">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2033">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="7046c-2034">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2034">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="7046c-2035">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2035">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="7046c-2036">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="7046c-2036">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="7046c-2037">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="7046c-2037">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="7046c-2038">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="7046c-2038">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="7046c-2039">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="7046c-2039">`location` no longer required</span></span>
  * <span data-ttu-id="7046c-2040">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="7046c-2040">Add name and ID support for target</span></span>
  * <span data-ttu-id="7046c-2041">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2041">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="7046c-2042">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="7046c-2042">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="7046c-2043">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="7046c-2043">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="7046c-2044">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="7046c-2044">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="7046c-2045">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2045">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="7046c-2046">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="7046c-2046">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="7046c-2047">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-2047">Network</span></span>

* <span data-ttu-id="7046c-2048">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2048">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="7046c-2049">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2049">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="7046c-2050">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="7046c-2050">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="7046c-2051">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="7046c-2051">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="7046c-2052">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2052">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="7046c-2053">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2053">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="7046c-2054">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="7046c-2054">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="7046c-2055">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="7046c-2055">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="7046c-2056">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="7046c-2056">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="7046c-2057">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7046c-2057">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="7046c-2058">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="7046c-2058">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="7046c-2059">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2059">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="7046c-2060">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="7046c-2060">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="7046c-2061">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2061">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="7046c-2062">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2062">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="7046c-2063">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2063">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="7046c-2064">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="7046c-2064">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="7046c-2065">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2065">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="7046c-2066">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2066">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="7046c-2067">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2067">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="7046c-2068">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2068">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="7046c-2069">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2069">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="7046c-2070">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2070">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="7046c-2071">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="7046c-2071">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="7046c-2072">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="7046c-2072">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="7046c-2073">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="7046c-2073">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="7046c-2074">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="7046c-2074">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-2075">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-2075">Profile</span></span>

* <span data-ttu-id="7046c-2076">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="7046c-2076">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="7046c-2077">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="7046c-2077">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="7046c-2078">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="7046c-2078">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="7046c-2079">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="7046c-2079">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="7046c-2080">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="7046c-2080">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="7046c-2081">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7046c-2081">RDBMS</span></span>

* <span data-ttu-id="7046c-2082">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="7046c-2082">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="7046c-2083">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="7046c-2083">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="7046c-2084">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="7046c-2084">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="7046c-2085">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="7046c-2085">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-2086">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-2086">Resource</span></span>

* <span data-ttu-id="7046c-2087">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2087">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="7046c-2088">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2088">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="7046c-2089">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2089">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="7046c-2090">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2090">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="7046c-2091">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="7046c-2091">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="7046c-2092">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2092">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="7046c-2093">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="7046c-2093">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="7046c-2094">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2094">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="7046c-2095">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-2095">Role</span></span>

* <span data-ttu-id="7046c-2096">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="7046c-2096">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="7046c-2097">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="7046c-2097">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="7046c-2098">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2098">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="7046c-2099">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2099">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="7046c-2100">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2100">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7046c-2101">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7046c-2101">Service Fabric</span></span>
* <span data-ttu-id="7046c-2102">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="7046c-2102">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="7046c-2103">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="7046c-2103">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="7046c-2104">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="7046c-2104">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-2105">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-2105">SQL</span></span>

* <span data-ttu-id="7046c-2106">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="7046c-2106">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="7046c-2107">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2107">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="7046c-2108">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="7046c-2108">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-2109">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-2109">Storage</span></span>

* <span data-ttu-id="7046c-2110">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="7046c-2110">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="7046c-2111">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="7046c-2111">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="7046c-2112">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="7046c-2112">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="7046c-2113">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="7046c-2113">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="7046c-2114">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="7046c-2114">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="7046c-2115">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="7046c-2115">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-2116">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-2116">VM</span></span>

* <span data-ttu-id="7046c-2117">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="7046c-2117">Support configuring nsg</span></span>
* <span data-ttu-id="7046c-2118">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="7046c-2118">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="7046c-2119">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="7046c-2119">Support managed service identities</span></span>
* <span data-ttu-id="7046c-2120">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="7046c-2120">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="7046c-2121">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="7046c-2121">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="7046c-2122">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-2122">May 10, 2017</span></span>

<span data-ttu-id="7046c-2123">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="7046c-2123">Version 2.0.6</span></span>

* <span data-ttu-id="7046c-2124">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="7046c-2124">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="7046c-2125">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="7046c-2125">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="7046c-2126">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7046c-2126">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="7046c-2127">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7046c-2127">Include Cognitive Services module</span></span>
* <span data-ttu-id="7046c-2128">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7046c-2128">Include Service Fabric module</span></span>
* <span data-ttu-id="7046c-2129">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="7046c-2129">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="7046c-2130">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="7046c-2130">Add support for CDN commands</span></span>
* <span data-ttu-id="7046c-2131">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="7046c-2131">Remove Container module</span></span>
* <span data-ttu-id="7046c-2132">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="7046c-2132">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="7046c-2133">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="7046c-2133">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```text
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a><span data-ttu-id="7046c-2134">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-2134">Core</span></span>

* <span data-ttu-id="7046c-2135">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="7046c-2135">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="7046c-2136">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="7046c-2136">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="7046c-2137">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="7046c-2137">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="7046c-2138">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="7046c-2138">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="7046c-2139">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="7046c-2139">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="7046c-2140">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="7046c-2140">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="7046c-2141">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="7046c-2141">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="7046c-2142">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="7046c-2142">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="7046c-2143">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="7046c-2143">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="7046c-2144">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="7046c-2144">core: Improved performance</span></span>
* <span data-ttu-id="7046c-2145">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="7046c-2145">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="7046c-2146">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="7046c-2146">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-2147">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-2147">ACS</span></span>

* <span data-ttu-id="7046c-2148">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="7046c-2148">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="7046c-2149">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="7046c-2149">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="7046c-2150">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="7046c-2150">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="7046c-2151">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="7046c-2151">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-2152">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-2152">AppService</span></span>

* <span data-ttu-id="7046c-2153">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="7046c-2153">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="7046c-2154">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="7046c-2154">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="7046c-2155">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="7046c-2155">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="7046c-2156">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="7046c-2156">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="7046c-2157">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="7046c-2157">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="7046c-2158">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="7046c-2158">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="7046c-2159">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7046c-2159">support slot swap with preview</span></span>
* <span data-ttu-id="7046c-2160">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="7046c-2160">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="7046c-2161">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="7046c-2161">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7046c-2162">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-2162">CosmosDB</span></span>

* <span data-ttu-id="7046c-2163">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7046c-2163">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="7046c-2164">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="7046c-2164">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="7046c-2165">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="7046c-2165">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="7046c-2166">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="7046c-2166">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7046c-2167">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7046c-2167">Data Lake Analytics</span></span>

* <span data-ttu-id="7046c-2168">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="7046c-2168">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="7046c-2169">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="7046c-2169">Add support for new catalog item type: package.</span></span> <span data-ttu-id="7046c-2170">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="7046c-2170">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="7046c-2171">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="7046c-2171">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="7046c-2172">Tabla</span><span class="sxs-lookup"><span data-stu-id="7046c-2172">Table</span></span>
  * <span data-ttu-id="7046c-2173">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="7046c-2173">Table valued function</span></span>
  * <span data-ttu-id="7046c-2174">Ver</span><span class="sxs-lookup"><span data-stu-id="7046c-2174">View</span></span>
  * <span data-ttu-id="7046c-2175">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="7046c-2175">Table Statistics.</span></span> <span data-ttu-id="7046c-2176">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="7046c-2176">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7046c-2177">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7046c-2177">Data Lake Store</span></span>

* <span data-ttu-id="7046c-2178">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="7046c-2178">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="7046c-2179">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="7046c-2179">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="7046c-2180">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="7046c-2180">missed help for access show.</span></span> <span data-ttu-id="7046c-2181">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="7046c-2181">adding it.</span></span> <span data-ttu-id="7046c-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="7046c-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="7046c-2183">Buscar</span><span class="sxs-lookup"><span data-stu-id="7046c-2183">Find</span></span>

* <span data-ttu-id="7046c-2184">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="7046c-2184">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="7046c-2185">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7046c-2185">KeyVault</span></span>

* <span data-ttu-id="7046c-2186">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="7046c-2186">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="7046c-2187">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="7046c-2187">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="7046c-2188">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="7046c-2188">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="7046c-2189">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="7046c-2189">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="7046c-2190">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="7046c-2190">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="7046c-2191">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-2191">Lab</span></span>

* <span data-ttu-id="7046c-2192">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-2192">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="7046c-2193">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-2193">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="7046c-2194">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-2194">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="7046c-2195">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-2195">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="7046c-2196">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="7046c-2196">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="7046c-2197">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7046c-2197">Monitor</span></span>

* <span data-ttu-id="7046c-2198">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="7046c-2198">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="7046c-2199">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="7046c-2199">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="7046c-2200">Red</span><span class="sxs-lookup"><span data-stu-id="7046c-2200">Network</span></span>

* <span data-ttu-id="7046c-2201">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="7046c-2201">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="7046c-2202">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="7046c-2202">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="7046c-2203">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="7046c-2203">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="7046c-2204">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="7046c-2204">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="7046c-2205">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="7046c-2205">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="7046c-2206">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7046c-2206">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="7046c-2207">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="7046c-2207">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="7046c-2208">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="7046c-2208">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="7046c-2209">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="7046c-2209">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="7046c-2210">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="7046c-2210">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="7046c-2211">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="7046c-2211">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="7046c-2212">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7046c-2212">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="7046c-2213">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="7046c-2213">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="7046c-2214">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="7046c-2214">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="7046c-2215">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="7046c-2215">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="7046c-2216">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="7046c-2216">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="7046c-2217">Perfil</span><span class="sxs-lookup"><span data-stu-id="7046c-2217">Profile</span></span>

* <span data-ttu-id="7046c-2218">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="7046c-2218">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="7046c-2219">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="7046c-2219">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="7046c-2220">Redis</span><span class="sxs-lookup"><span data-stu-id="7046c-2220">Redis</span></span>

* <span data-ttu-id="7046c-2221">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="7046c-2221">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="7046c-2222">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="7046c-2222">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="7046c-2223">Recurso</span><span class="sxs-lookup"><span data-stu-id="7046c-2223">Resource</span></span>

* <span data-ttu-id="7046c-2224">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="7046c-2224">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="7046c-2225">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="7046c-2225">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="7046c-2226">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="7046c-2226">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="7046c-2227">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="7046c-2227">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="7046c-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="7046c-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="7046c-2229">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="7046c-2229">Add docs for az lock update.</span></span> <span data-ttu-id="7046c-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="7046c-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="7046c-2231">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="7046c-2231">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="7046c-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="7046c-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="7046c-2233">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="7046c-2233">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="7046c-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="7046c-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="7046c-2235">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="7046c-2235">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="7046c-2236">Rol</span><span class="sxs-lookup"><span data-stu-id="7046c-2236">Role</span></span>

* <span data-ttu-id="7046c-2237">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="7046c-2237">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="7046c-2238">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="7046c-2238">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="7046c-2239">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="7046c-2239">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="7046c-2240">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="7046c-2240">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="7046c-2241">SQL</span><span class="sxs-lookup"><span data-stu-id="7046c-2241">SQL</span></span>

* <span data-ttu-id="7046c-2242">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="7046c-2242">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="7046c-2243">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="7046c-2243">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="7046c-2244">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-2244">Storage</span></span>

* <span data-ttu-id="7046c-2245">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="7046c-2245">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="7046c-2246">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="7046c-2246">Add support for incremental blob copy</span></span>
* <span data-ttu-id="7046c-2247">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="7046c-2247">Add support for large block blob upload</span></span>
* <span data-ttu-id="7046c-2248">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="7046c-2248">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-2249">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-2249">VM</span></span>

* <span data-ttu-id="7046c-2250">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="7046c-2250">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="7046c-2251">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="7046c-2251">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="7046c-2252">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="7046c-2252">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="7046c-2253">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="7046c-2253">az vm/vmss disk</span></span>
  3. <span data-ttu-id="7046c-2254">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="7046c-2254">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="7046c-2255">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="7046c-2255">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="7046c-2256">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="7046c-2256">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="7046c-2257">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-2257">April 3, 2017</span></span>

<span data-ttu-id="7046c-2258">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="7046c-2258">Version 2.0.2</span></span>

<span data-ttu-id="7046c-2259">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="7046c-2259">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```text
azure-cli (2.0.2)

acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a><span data-ttu-id="7046c-2260">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7046c-2260">Core</span></span>

* <span data-ttu-id="7046c-2261">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="7046c-2261">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="7046c-2262">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="7046c-2262">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="7046c-2263">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="7046c-2263">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="7046c-2264">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7046c-2264">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7046c-2265">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="7046c-2265">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="7046c-2266">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="7046c-2266">Add prompting for missing template parameters.</span></span> <span data-ttu-id="7046c-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="7046c-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="7046c-2268">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="7046c-2268">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="7046c-2269">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="7046c-2269">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="7046c-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="7046c-2270">ACS</span></span>

* <span data-ttu-id="7046c-2271">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="7046c-2271">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="7046c-2272">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="7046c-2272">Add support for ssh key password prompting.</span></span> <span data-ttu-id="7046c-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="7046c-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="7046c-2274">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="7046c-2274">Add support for windows clusters.</span></span> <span data-ttu-id="7046c-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="7046c-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="7046c-2276">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="7046c-2276">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="7046c-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="7046c-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="7046c-2278">AppService</span><span class="sxs-lookup"><span data-stu-id="7046c-2278">AppService</span></span>

* <span data-ttu-id="7046c-2279">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="7046c-2279">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="7046c-2280">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="7046c-2280">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="7046c-2281">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="7046c-2281">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="7046c-2282">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="7046c-2282">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="7046c-2283">DataLake</span><span class="sxs-lookup"><span data-stu-id="7046c-2283">DataLake</span></span>

* <span data-ttu-id="7046c-2284">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7046c-2284">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="7046c-2285">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7046c-2285">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="7046c-2286">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="7046c-2286">DocuemntDB</span></span>

* <span data-ttu-id="7046c-2287">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="7046c-2287">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="7046c-2288">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7046c-2288">VM</span></span>

* <span data-ttu-id="7046c-2289">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="7046c-2289">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="7046c-2290">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="7046c-2290">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="7046c-2291">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="7046c-2291">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="7046c-2292">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7046c-2292">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7046c-2293">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="7046c-2293">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="7046c-2294">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="7046c-2294">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="7046c-2295">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="7046c-2295">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="7046c-2296">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="7046c-2296">February 27, 2017</span></span>

<span data-ttu-id="7046c-2297">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7046c-2297">Version 2.0.0</span></span>

<span data-ttu-id="7046c-2298">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="7046c-2298">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="7046c-2299">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="7046c-2299">Container Service (acs)</span></span>
- <span data-ttu-id="7046c-2300">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="7046c-2300">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="7046c-2301">Redes</span><span class="sxs-lookup"><span data-stu-id="7046c-2301">Networking</span></span>
- <span data-ttu-id="7046c-2302">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7046c-2302">Storage</span></span>

<span data-ttu-id="7046c-2303">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7046c-2303">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="7046c-2304">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7046c-2304">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="7046c-2305">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="7046c-2305">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```text
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)

Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32)
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> <span data-ttu-id="7046c-2306">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="7046c-2306">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="7046c-2307">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="7046c-2307">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="7046c-2308">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="7046c-2308">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="7046c-2309">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="7046c-2309">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="7046c-2310">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="7046c-2310">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="7046c-2311">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7046c-2311">Provide feedback from the command line with the `az feedback` command</span></span>

