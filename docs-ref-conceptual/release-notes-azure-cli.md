---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4337f2203841d6247e4b487d245138424c63e448
ms.sourcegitcommit: 71c0ccd475524cf4d6db45bba8139fef3262d764
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2019
ms.locfileid: "58175140"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="7fad9-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7fad9-103">Azure CLI release notes</span></span>
## <a name="march-12-2019"></a><span data-ttu-id="7fad9-104">12 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="7fad9-104">March 12, 2019</span></span>

<span data-ttu-id="7fad9-105">Versión 2.0.60</span><span class="sxs-lookup"><span data-stu-id="7fad9-105">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-106">Core</span></span>

* <span data-ttu-id="7fad9-107">Se ha corregido un error incorrecto en `cloud set` sobre la suscripción no encontrada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-107">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-108">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-108">ACR</span></span>

* <span data-ttu-id="7fad9-109">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="7fad9-109">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-110">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-110">ACS</span></span>

* <span data-ttu-id="7fad9-111">Se ha cambiado para ignorar el argumento `--listen-address` a `aks browse` si `kubectl` no lo admite.</span><span class="sxs-lookup"><span data-stu-id="7fad9-111">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-112">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-112">AppService</span></span>

* <span data-ttu-id="7fad9-113">Se ha agregado `[webapp|functionapp] deployment list-publishing-credentials` para obtener la dirección URL y sus credenciales de publicación de Kudu.</span><span class="sxs-lookup"><span data-stu-id="7fad9-113">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="7fad9-114">Se ha quitado la instrucción de impresión errónea para `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-114">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="7fad9-115">Se ha corregido `functionapp` para establecer la imagen correcta en el entorno de ejecución en los planes de App Service de Linux</span><span class="sxs-lookup"><span data-stu-id="7fad9-115">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="7fad9-116">Se ha quitado la etiqueta de versión preliminar para `webapp up` y se han agregado mejoras al comando.</span><span class="sxs-lookup"><span data-stu-id="7fad9-116">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="7fad9-117">Botservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-117">Botservice</span></span>

* <span data-ttu-id="7fad9-118">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="7fad9-118">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7fad9-119">Se han agregado `Microsoft-BotFramework-AppId` y `Microsoft-BotFramework-AppPassword` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web</span><span class="sxs-lookup"><span data-stu-id="7fad9-119">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7fad9-120">Se han quitado las comillas simples de la salida del comando `bot publish` al final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-120">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="7fad9-121">Se ha cambiado `bot publish` para que sea asincrónico.</span><span class="sxs-lookup"><span data-stu-id="7fad9-121">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-122">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-122">Container</span></span>

* <span data-ttu-id="7fad9-123">Se agregó el argumento `--no-wait` a `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-123">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="7fad9-124">EventHub</span><span class="sxs-lookup"><span data-stu-id="7fad9-124">EventHub</span></span>

* <span data-ttu-id="7fad9-125">Se ha agregado la marca `--skip-empty-archives` a `eventhub create|update` para admitir archivos vacíos en la captura.</span><span class="sxs-lookup"><span data-stu-id="7fad9-125">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="7fad9-126">Buscar</span><span class="sxs-lookup"><span data-stu-id="7fad9-126">Find</span></span>

* <span data-ttu-id="7fad9-127">Actualización de la funcionalidad principal</span><span class="sxs-lookup"><span data-stu-id="7fad9-127">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7fad9-128">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7fad9-128">HDInsight</span></span>

* <span data-ttu-id="7fad9-129">Se ha agregado el parámetro `--storage-account-managed-identity` a `hdinsight create` para admitir MSI de ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="7fad9-129">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-130">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-130">Network</span></span>

* <span data-ttu-id="7fad9-131">Se ha corregido un problema con `vpn-connection update` por el que no se podía actualizar una conexión VPN entre pasarelas de diferentes suscripciones.</span><span class="sxs-lookup"><span data-stu-id="7fad9-131">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-132">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7fad9-132">Rdbms</span></span>

* <span data-ttu-id="7fad9-133">Correcciones menores para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="7fad9-133">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-134">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-134">Role</span></span>

* <span data-ttu-id="7fad9-135">Se ha corregido `role definition update` para usar el identificador para resolver la definición correctamente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-135">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="7fad9-136">Se ha cambiado `ad app credential reset` para eliminar la suposición de que la entidad de servicio de la aplicación siempre existe.</span><span class="sxs-lookup"><span data-stu-id="7fad9-136">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7fad9-137">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7fad9-137">Service Fabric</span></span>

* <span data-ttu-id="7fad9-138">Se ha corregido un problema con `sf cluster list` que no se podía iterar.</span><span class="sxs-lookup"><span data-stu-id="7fad9-138">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="7fad9-139">26 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="7fad9-139">February 26, 2019</span></span>

<span data-ttu-id="7fad9-140">Versión 2.0.59</span><span class="sxs-lookup"><span data-stu-id="7fad9-140">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-141">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-141">Core</span></span>

* <span data-ttu-id="7fad9-142">Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.</span><span class="sxs-lookup"><span data-stu-id="7fad9-142">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-143">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-143">ACR</span></span>

* <span data-ttu-id="7fad9-144">Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-144">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="7fad9-145">Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.</span><span class="sxs-lookup"><span data-stu-id="7fad9-145">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-146">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-146">ACS</span></span>

* <span data-ttu-id="7fad9-147">Se agregó la opción `--listen-address` a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="7fad9-147">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-148">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-148">AppService</span></span>

* <span data-ttu-id="7fad9-149">Se agregó el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-149">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-150">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-150">Batch</span></span>
* <span data-ttu-id="7fad9-151">[CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-151">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="7fad9-152">[CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-152">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="7fad9-153">Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="7fad9-153">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="7fad9-154">[CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-154">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="7fad9-155">Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.</span><span class="sxs-lookup"><span data-stu-id="7fad9-155">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="7fad9-156">Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.</span><span class="sxs-lookup"><span data-stu-id="7fad9-156">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-157">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-157">CosmosDB</span></span>

* <span data-ttu-id="7fad9-158">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="7fad9-158">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="7fad9-159">Kusto</span><span class="sxs-lookup"><span data-stu-id="7fad9-159">Kusto</span></span>

* <span data-ttu-id="7fad9-160">[CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.</span><span class="sxs-lookup"><span data-stu-id="7fad9-160">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-161">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-161">Network</span></span>

* <span data-ttu-id="7fad9-162">Se agregó el argumento `--express-route-gateway-bypass` a `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-162">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="7fad9-163">Se han agregado grupos de comandos desde extensiones `express-route`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-163">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="7fad9-164">Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-164">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="7fad9-165">Se agregó el argumento `--legacy-mode` a `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-165">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="7fad9-166">Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-166">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="7fad9-167">Se agregó el argumento `--gateway-default-site` a `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-167">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="7fad9-168">Se han agregado comandos `ipsec-policy` a `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-168">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-169">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-169">Resource</span></span>

* <span data-ttu-id="7fad9-170">Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-170">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="7fad9-171">Se ha agregado compatibilidad para el archivo de parámetros basado en URI a `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-171">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="7fad9-172">Se ha agregado compatibilidad para definiciones y parámetros basados en URI para `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-172">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="7fad9-173">Se ha corregido el control de parámetros y reglas para `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-173">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="7fad9-174">Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.</span><span class="sxs-lookup"><span data-stu-id="7fad9-174">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-175">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-175">Role</span></span>

* <span data-ttu-id="7fad9-176">Se ha agregado compatibilidad con roles de aplicación a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-176">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-177">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-177">VM</span></span>

* <span data-ttu-id="7fad9-178">Se ha corregido un problema con `vm create where `--acelerated-networking\` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="7fad9-178">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="7fad9-179">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="7fad9-179">February 12, 2019</span></span>

<span data-ttu-id="7fad9-180">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="7fad9-180">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-181">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-181">Core</span></span>

* <span data-ttu-id="7fad9-182">`az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="7fad9-182">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="7fad9-183">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="7fad9-183">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-184">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-184">ACR</span></span>
* <span data-ttu-id="7fad9-185">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-185">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="7fad9-186">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-186">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-187">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-187">ACS</span></span>
* <span data-ttu-id="7fad9-188">Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.</span><span class="sxs-lookup"><span data-stu-id="7fad9-188">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="7fad9-189">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-189">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="7fad9-190">Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-190">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="7fad9-191">AMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-191">AMS</span></span>
* <span data-ttu-id="7fad9-192">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-192">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="7fad9-193">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-193">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-194">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-194">Appservice</span></span>
* <span data-ttu-id="7fad9-195">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="7fad9-195">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="7fad9-196">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="7fad9-196">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="7fad9-197">Se ha mejorado la ayuda de `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-197">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="7fad9-198">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="7fad9-198">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="7fad9-199">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="7fad9-199">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="7fad9-200">Botservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-200">Botservice</span></span>
* <span data-ttu-id="7fad9-201">Se ha mejorado la experiencia de usuario de `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-201">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="7fad9-202">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-202">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="7fad9-203">Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-203">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="7fad9-204">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="7fad9-204">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="7fad9-205">[EN DESUSO] Se ha dejado de usar el argumento `--proj-name` en favor de `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-205">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="7fad9-206">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="7fad9-206">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="7fad9-207">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="7fad9-207">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="7fad9-208">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="7fad9-208">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="7fad9-209">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="7fad9-209">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="7fad9-210">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="7fad9-210">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="7fad9-211">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7fad9-211">Key Vault</span></span>
* <span data-ttu-id="7fad9-212">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-212">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-213">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-213">Monitor</span></span>
* <span data-ttu-id="7fad9-214">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-214">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-215">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-215">Network</span></span>
* <span data-ttu-id="7fad9-216">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-216">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="7fad9-217">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="7fad9-217">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="7fad9-218">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="7fad9-218">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="7fad9-219">Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-219">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7fad9-220">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="7fad9-220">Policy Insights</span></span>
* <span data-ttu-id="7fad9-221">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-221">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-222">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-222">RDBMS</span></span>
* <span data-ttu-id="7fad9-223">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="7fad9-223">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="7fad9-224">Redis</span><span class="sxs-lookup"><span data-stu-id="7fad9-224">Redis</span></span>
* <span data-ttu-id="7fad9-225">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="7fad9-225">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="7fad9-226">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="7fad9-226">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="7fad9-227">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="7fad9-227">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="7fad9-228">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="7fad9-228">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="7fad9-229">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-229">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="7fad9-230">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="7fad9-230">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="7fad9-231">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-231">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-232">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-232">Role</span></span>
* <span data-ttu-id="7fad9-233">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-233">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="7fad9-234">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-234">SQL VM</span></span>
* <span data-ttu-id="7fad9-235">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="7fad9-235">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-236">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-236">VM</span></span>
* <span data-ttu-id="7fad9-237">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-237">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="7fad9-238">Se agregó `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-238">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="7fad9-239">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-239">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="7fad9-240">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-240">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="7fad9-241">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="7fad9-241">January 31, 2019</span></span>

<span data-ttu-id="7fad9-242">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="7fad9-242">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-243">Core</span></span>

* <span data-ttu-id="7fad9-244">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="7fad9-244">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="7fad9-245">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="7fad9-245">January 28, 2019</span></span>

<span data-ttu-id="7fad9-246">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="7fad9-246">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-247">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-247">ACR</span></span>
* <span data-ttu-id="7fad9-248">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="7fad9-248">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-249">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-249">ACS</span></span>
* <span data-ttu-id="7fad9-250">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="7fad9-250">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7fad9-251">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="7fad9-251">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="7fad9-252">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-252">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="7fad9-253">AMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-253">AMS</span></span>
* <span data-ttu-id="7fad9-254">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="7fad9-254">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="7fad9-255">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="7fad9-255">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-256">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-256">Appservice</span></span>
* <span data-ttu-id="7fad9-257">Se ha agregado compatibilidad para App Insights en `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-257">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="7fad9-258">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="7fad9-258">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="7fad9-259">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="7fad9-259">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-260">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-260">Container</span></span>
* <span data-ttu-id="7fad9-261">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-261">Added `container start` command</span></span>
* <span data-ttu-id="7fad9-262">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="7fad9-262">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7fad9-263">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7fad9-263">EventGrid</span></span>
* <span data-ttu-id="7fad9-264">Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-264">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="7fad9-265">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="7fad9-265">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="7fad9-266">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-266">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="7fad9-267">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-267">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="7fad9-268">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="7fad9-268">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7fad9-269">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7fad9-269">HDInsight</span></span>
* <span data-ttu-id="7fad9-270">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-270">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="7fad9-271">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="7fad9-271">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="7fad9-272">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-272">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="7fad9-273">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-273">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="7fad9-274">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-274">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="7fad9-275">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-275">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-276">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-276">IoT</span></span>
* <span data-ttu-id="7fad9-277">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="7fad9-277">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="7fad9-278">Kusto</span><span class="sxs-lookup"><span data-stu-id="7fad9-278">Kusto</span></span>
* <span data-ttu-id="7fad9-279">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-279">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-280">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-280">Monitor</span></span>
* <span data-ttu-id="7fad9-281">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-281">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-282">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-282">Profile</span></span>
* <span data-ttu-id="7fad9-283">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-283">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-284">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-284">Network</span></span>
* <span data-ttu-id="7fad9-285">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-285">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="7fad9-286">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="7fad9-286">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-287">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-287">Resource</span></span>
* <span data-ttu-id="7fad9-288">Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-288">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="7fad9-289">Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-289">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="7fad9-290">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-290">SQL Virtual Machine</span></span>
* <span data-ttu-id="7fad9-291">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-291">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-292">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-292">Storage</span></span>
* <span data-ttu-id="7fad9-293">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="7fad9-293">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="7fad9-294">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="7fad9-294">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-295">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-295">VM</span></span>
* <span data-ttu-id="7fad9-296">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="7fad9-296">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="7fad9-297">Se ha agregado la marca `--force` a `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-297">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="7fad9-298">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="7fad9-298">January 15, 2019</span></span>

<span data-ttu-id="7fad9-299">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="7fad9-299">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-300">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-300">ACR</span></span>
* <span data-ttu-id="7fad9-301">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="7fad9-301">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="7fad9-302">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="7fad9-302">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="7fad9-303">[EN DESUSO] El parámetro `--resource-group` está en desuso en los comandos:</span><span class="sxs-lookup"><span data-stu-id="7fad9-303">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="7fad9-304">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-304">ACS</span></span>
* <span data-ttu-id="7fad9-305">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="7fad9-305">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-306">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-306">Appservice</span></span>
* <span data-ttu-id="7fad9-307">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="7fad9-307">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="7fad9-308">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="7fad9-308">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="7fad9-309">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="7fad9-309">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="7fad9-310">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-310">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="7fad9-311">Botservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-311">Botservice</span></span>
* <span data-ttu-id="7fad9-312">Se han agregado actualizaciones al estado de implementación a `bot create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-312">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="7fad9-313">Configuración</span><span class="sxs-lookup"><span data-stu-id="7fad9-313">Configure</span></span>
* <span data-ttu-id="7fad9-314">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="7fad9-314">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-315">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-315">CosmosDB</span></span>
* <span data-ttu-id="7fad9-316">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="7fad9-316">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7fad9-317">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7fad9-317">HDInsight</span></span>
* <span data-ttu-id="7fad9-318">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="7fad9-318">Added commands for managing applications</span></span>
* <span data-ttu-id="7fad9-319">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="7fad9-319">Added commands for managing script actions</span></span>
* <span data-ttu-id="7fad9-320">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="7fad9-320">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="7fad9-321">Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-321">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="7fad9-322">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-322">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-323">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-323">Network</span></span>
* <span data-ttu-id="7fad9-324">Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-324">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="7fad9-325">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="7fad9-325">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="7fad9-326">Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-326">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="7fad9-327">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-327">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-328">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-328">Role</span></span>
* <span data-ttu-id="7fad9-329">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-329">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="7fad9-330">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="7fad9-330">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="7fad9-331">Seguridad</span><span class="sxs-lookup"><span data-stu-id="7fad9-331">Security</span></span>
* <span data-ttu-id="7fad9-332">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="7fad9-332">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-333">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-333">Storage</span></span>
* <span data-ttu-id="7fad9-334">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="7fad9-334">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="7fad9-335">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="7fad9-335">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="7fad9-336">Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-336">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="7fad9-337">Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-337">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="7fad9-338">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-338">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-339">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-339">VM</span></span>
* <span data-ttu-id="7fad9-340">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="7fad9-340">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="7fad9-341">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-341">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7fad9-342">Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-342">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="7fad9-343">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="7fad9-343">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="7fad9-344">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="7fad9-344">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="7fad9-345">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-345">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="7fad9-346">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-346">December 20, 2018</span></span>

<span data-ttu-id="7fad9-347">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="7fad9-347">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="7fad9-348">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-348">Appservice</span></span>
* <span data-ttu-id="7fad9-349">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="7fad9-349">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="7fad9-350">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="7fad9-350">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="7fad9-351">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="7fad9-351">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7fad9-352">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="7fad9-352">IoTCentral</span></span>
* <span data-ttu-id="7fad9-353">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="7fad9-353">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-354">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-354">Role</span></span>
* <span data-ttu-id="7fad9-355">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-355">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-356">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-356">SQL</span></span>
* <span data-ttu-id="7fad9-357">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-357">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-358">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-358">VM</span></span>
* <span data-ttu-id="7fad9-359">Se ha agregado el parámetro `---os-type` a `disk create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-359">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="7fad9-360">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-360">December 18, 2018</span></span>

<span data-ttu-id="7fad9-361">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="7fad9-361">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="7fad9-362">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-362">ACR</span></span>
* <span data-ttu-id="7fad9-363">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-363">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="7fad9-364">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-364">Condensed the table layout for task list</span></span>
* <span data-ttu-id="7fad9-365">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="7fad9-365">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-366">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-366">ACS</span></span>
* <span data-ttu-id="7fad9-367">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="7fad9-367">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7fad9-368">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-368">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="7fad9-369">[EN DESUSO] Se han dejado de utilizar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-369">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="7fad9-370">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="7fad9-370">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="7fad9-371">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="7fad9-371">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="7fad9-372">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="7fad9-372">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-373">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-373">Appservice</span></span>
* <span data-ttu-id="7fad9-374">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-374">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="7fad9-375">Botservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-375">Botservice</span></span>
* <span data-ttu-id="7fad9-376">Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-376">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="7fad9-377">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="7fad9-377">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="7fad9-378">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-378">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="7fad9-379">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="7fad9-379">Reduced Kudu network calls</span></span>
* <span data-ttu-id="7fad9-380">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="7fad9-380">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="7fad9-381">Consumo</span><span class="sxs-lookup"><span data-stu-id="7fad9-381">Consumption</span></span>
* <span data-ttu-id="7fad9-382">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="7fad9-382">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-383">CosmosDB</span></span>
* <span data-ttu-id="7fad9-384">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="7fad9-384">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="7fad9-385">Mapas</span><span class="sxs-lookup"><span data-stu-id="7fad9-385">Maps</span></span>
* <span data-ttu-id="7fad9-386">Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-386">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-387">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-387">Network</span></span>
* <span data-ttu-id="7fad9-388">Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="7fad9-388">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="7fad9-389">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="7fad9-389">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-390">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-390">Resource</span></span>
* <span data-ttu-id="7fad9-391">Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-391">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="7fad9-392">Se ha agregado un nuevo comando `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-392">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-393">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-393">Storage</span></span>
*  <span data-ttu-id="7fad9-394">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-394">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-395">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-395">VM</span></span>
* <span data-ttu-id="7fad9-396">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-396">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="7fad9-397">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-397">December 4, 2018</span></span>

<span data-ttu-id="7fad9-398">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="7fad9-398">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="7fad9-399">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-399">Core</span></span>
* <span data-ttu-id="7fad9-400">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="7fad9-400">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="7fad9-401">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="7fad9-401">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-402">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-402">Appservice</span></span>
* <span data-ttu-id="7fad9-403">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="7fad9-403">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="7fad9-404">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="7fad9-404">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-405">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-405">Network</span></span>
* <span data-ttu-id="7fad9-406">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="7fad9-406">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-407">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-407">Role</span></span>
* <span data-ttu-id="7fad9-408">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="7fad9-408">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="7fad9-409">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-409">VM</span></span>
* <span data-ttu-id="7fad9-410">[EN DESUSO] El parámetro `vm extension [show|wait] --expand` está en desuso</span><span class="sxs-lookup"><span data-stu-id="7fad9-410">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="7fad9-411">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="7fad9-411">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="7fad9-412">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="7fad9-412">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="7fad9-413">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="7fad9-413">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="7fad9-414">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-414">November 20, 2018</span></span>

<span data-ttu-id="7fad9-415">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="7fad9-415">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="7fad9-416">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-416">Core</span></span>
* <span data-ttu-id="7fad9-417">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="7fad9-417">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-418">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-418">ACR</span></span>
* <span data-ttu-id="7fad9-419">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="7fad9-419">Added context token to task step</span></span>
* <span data-ttu-id="7fad9-420">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="7fad9-420">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="7fad9-421">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-421">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-422">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-422">Appservice</span></span>
* <span data-ttu-id="7fad9-423">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="7fad9-423">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="7fad9-424">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-424">Updated the default `node_version`.</span></span> <span data-ttu-id="7fad9-425">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="7fad9-425">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="7fad9-426">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="7fad9-426">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="7fad9-427">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="7fad9-427">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7fad9-428">IotCentral</span><span class="sxs-lookup"><span data-stu-id="7fad9-428">IotCentral</span></span>
* <span data-ttu-id="7fad9-429">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7fad9-429">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-430">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7fad9-430">KeyVault</span></span>
* <span data-ttu-id="7fad9-431">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="7fad9-431">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-432">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-432">Network</span></span>
* <span data-ttu-id="7fad9-433">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="7fad9-433">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="7fad9-434">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="7fad9-434">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="7fad9-435">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="7fad9-435">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="7fad9-436">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-436">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-437">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7fad9-437">Rdbms</span></span>
* <span data-ttu-id="7fad9-438">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="7fad9-438">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="7fad9-439">Rbac</span><span class="sxs-lookup"><span data-stu-id="7fad9-439">Rbac</span></span>
* <span data-ttu-id="7fad9-440">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-440">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="7fad9-441">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-441">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="7fad9-442">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-442">Storage</span></span>
* <span data-ttu-id="7fad9-443">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="7fad9-443">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="7fad9-444">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-444">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="7fad9-445">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="7fad9-445">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="7fad9-446">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-446">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-447">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-447">VM</span></span>
* <span data-ttu-id="7fad9-448">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-448">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="7fad9-449">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-449">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="7fad9-450">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-450">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="7fad9-451">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-451">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="7fad9-452">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-452">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="7fad9-453">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-453">Added `snapshot wait` command</span></span>
* <span data-ttu-id="7fad9-454">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-454">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="7fad9-455">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-455">November 6, 2018</span></span>

<span data-ttu-id="7fad9-456">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="7fad9-456">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-457">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-457">Core</span></span>
* <span data-ttu-id="7fad9-458">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="7fad9-458">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-459">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-459">ACR</span></span>
* <span data-ttu-id="7fad9-460">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="7fad9-460">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="7fad9-461">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="7fad9-461">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-462">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-462">ACS</span></span>
* <span data-ttu-id="7fad9-463">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7fad9-463">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="7fad9-464">Advisor</span><span class="sxs-lookup"><span data-stu-id="7fad9-464">Advisor</span></span>
* <span data-ttu-id="7fad9-465">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="7fad9-465">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="7fad9-466">AMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-466">AMS</span></span>
* <span data-ttu-id="7fad9-467">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="7fad9-467">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="7fad9-468">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="7fad9-468">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="7fad9-469">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-469">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="7fad9-470">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-470">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="7fad9-471">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="7fad9-471">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="7fad9-472">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="7fad9-472">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="7fad9-473">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="7fad9-473">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="7fad9-474">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="7fad9-474">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="7fad9-475">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="7fad9-475">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="7fad9-476">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="7fad9-476">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="7fad9-477">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="7fad9-477">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="7fad9-478">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-478">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="7fad9-479">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="7fad9-479">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="7fad9-480">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="7fad9-480">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="7fad9-481">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-481">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="7fad9-482">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="7fad9-482">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="7fad9-483">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="7fad9-483">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-484">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-484">AppService</span></span>
* <span data-ttu-id="7fad9-485">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="7fad9-485">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="7fad9-486">Configuración</span><span class="sxs-lookup"><span data-stu-id="7fad9-486">Configure</span></span>
* <span data-ttu-id="7fad9-487">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="7fad9-487">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-488">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-488">Container</span></span>
* <span data-ttu-id="7fad9-489">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="7fad9-489">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="7fad9-490">EventHub</span><span class="sxs-lookup"><span data-stu-id="7fad9-490">EventHub</span></span>
* <span data-ttu-id="7fad9-491">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-491">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-492">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-492">Interactive</span></span>
* <span data-ttu-id="7fad9-493">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="7fad9-493">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-494">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-494">Monitor</span></span>
* <span data-ttu-id="7fad9-495">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-495">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-496">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-496">Network</span></span>
* <span data-ttu-id="7fad9-497">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="7fad9-497">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="7fad9-498">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="7fad9-498">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="7fad9-499">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-499">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="7fad9-500">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-500">Profile</span></span>
* <span data-ttu-id="7fad9-501">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="7fad9-501">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-502">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-502">RDBMS</span></span>
* <span data-ttu-id="7fad9-503">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="7fad9-503">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-504">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-504">Resource</span></span>
* <span data-ttu-id="7fad9-505">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="7fad9-505">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-506">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-506">Role</span></span>
* <span data-ttu-id="7fad9-507">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="7fad9-507">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="7fad9-508">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="7fad9-508">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="7fad9-509">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="7fad9-509">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-510">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-510">Storage</span></span>
* <span data-ttu-id="7fad9-511">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="7fad9-511">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-512">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-512">VM</span></span>
* <span data-ttu-id="7fad9-513">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="7fad9-513">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="7fad9-514">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="7fad9-514">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="7fad9-515">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="7fad9-515">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="7fad9-516">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="7fad9-516">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="7fad9-517">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="7fad9-517">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="7fad9-518">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="7fad9-518">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="7fad9-519">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-519">October 23, 2018</span></span>

<span data-ttu-id="7fad9-520">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="7fad9-520">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-521">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-521">Core</span></span>
* <span data-ttu-id="7fad9-522">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="7fad9-522">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="7fad9-523">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="7fad9-523">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-524">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-524">ACR</span></span>
* <span data-ttu-id="7fad9-525">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="7fad9-525">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="7fad9-526">CDN</span><span class="sxs-lookup"><span data-stu-id="7fad9-526">CDN</span></span>
* <span data-ttu-id="7fad9-527">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="7fad9-527">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7fad9-528">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="7fad9-528">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-529">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-529">Container</span></span>
* <span data-ttu-id="7fad9-530">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="7fad9-530">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="7fad9-531">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-531">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="7fad9-532">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="7fad9-532">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="7fad9-533">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-533">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="7fad9-534">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="7fad9-534">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="7fad9-535">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="7fad9-535">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="7fad9-536">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="7fad9-536">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-537">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-537">CosmosDB</span></span>
* <span data-ttu-id="7fad9-538">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-538">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-539">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-539">Interactive</span></span>
* <span data-ttu-id="7fad9-540">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="7fad9-540">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="7fad9-541">IoT Central</span><span class="sxs-lookup"><span data-stu-id="7fad9-541">IoT Central</span></span>
* <span data-ttu-id="7fad9-542">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7fad9-542">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="7fad9-543">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="7fad9-543">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-544">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-544">Monitor</span></span>
* <span data-ttu-id="7fad9-545">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="7fad9-545">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="7fad9-546">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="7fad9-546">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="7fad9-547">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="7fad9-547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7fad9-548">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="7fad9-548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="7fad9-549">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="7fad9-549">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="7fad9-550">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="7fad9-550">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="7fad9-551">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="7fad9-551">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="7fad9-552">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="7fad9-552">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7fad9-553">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="7fad9-553">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="7fad9-554">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-554">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-555">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-555">Network</span></span>
* <span data-ttu-id="7fad9-556">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="7fad9-556">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="7fad9-557">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="7fad9-557">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="7fad9-558">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7fad9-558">ServiceBus</span></span>
* <span data-ttu-id="7fad9-559">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="7fad9-559">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-560">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-560">SQL</span></span>
* <span data-ttu-id="7fad9-561">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="7fad9-561">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-562">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-562">Storage</span></span>
* <span data-ttu-id="7fad9-563">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="7fad9-563">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="7fad9-564">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="7fad9-564">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-565">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-565">VM</span></span>
* <span data-ttu-id="7fad9-566">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-566">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="7fad9-567">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-567">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="7fad9-568">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-568">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="7fad9-569">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-569">October 16, 2018</span></span>

<span data-ttu-id="7fad9-570">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="7fad9-570">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-571">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-571">VM</span></span>
* <span data-ttu-id="7fad9-572">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="7fad9-572">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="7fad9-573">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-573">October 9, 2018</span></span>

<span data-ttu-id="7fad9-574">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="7fad9-574">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-575">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-575">Core</span></span>
* <span data-ttu-id="7fad9-576">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="7fad9-576">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-577">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-577">ACR</span></span>
* <span data-ttu-id="7fad9-578">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="7fad9-578">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-579">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-579">ACS</span></span>
* <span data-ttu-id="7fad9-580">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="7fad9-580">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="7fad9-581">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="7fad9-581">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="7fad9-582">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="7fad9-582">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="7fad9-583">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="7fad9-583">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-584">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-584">Container</span></span>
* <span data-ttu-id="7fad9-585">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="7fad9-585">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="7fad9-586">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="7fad9-586">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="7fad9-587">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="7fad9-587">Event Hub</span></span>
* <span data-ttu-id="7fad9-588">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-588">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="7fad9-589">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="7fad9-589">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="7fad9-590">Extensiones</span><span class="sxs-lookup"><span data-stu-id="7fad9-590">Extensions</span></span>
* <span data-ttu-id="7fad9-591">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="7fad9-591">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7fad9-592">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7fad9-592">HDInsight</span></span>
* <span data-ttu-id="7fad9-593">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7fad9-593">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-594">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-594">IoT</span></span>
* <span data-ttu-id="7fad9-595">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="7fad9-595">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-596">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7fad9-596">KeyVault</span></span>
* <span data-ttu-id="7fad9-597">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="7fad9-597">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-598">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-598">Network</span></span>
* <span data-ttu-id="7fad9-599">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-599">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="7fad9-600">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="7fad9-600">See #6052</span></span>
* <span data-ttu-id="7fad9-601">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-601">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="7fad9-602">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="7fad9-602">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="7fad9-603">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7fad9-603">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="7fad9-604">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7fad9-604">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="7fad9-605">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="7fad9-605">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="7fad9-606">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-606">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-607">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-607">Role</span></span>
* <span data-ttu-id="7fad9-608">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="7fad9-608">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="7fad9-609">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="7fad9-609">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="7fad9-610">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="7fad9-610">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="7fad9-611">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="7fad9-611">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="7fad9-612">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="7fad9-612">Service Bus</span></span>
* <span data-ttu-id="7fad9-613">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="7fad9-613">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-614">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-614">VM</span></span>
* <span data-ttu-id="7fad9-615">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="7fad9-615">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="7fad9-616">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="7fad9-616">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="7fad9-617">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="7fad9-617">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="7fad9-618">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="7fad9-618">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="7fad9-619">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="7fad9-619">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="7fad9-620">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="7fad9-620">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="7fad9-621">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-621">September 21, 2018</span></span>

<span data-ttu-id="7fad9-622">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="7fad9-622">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-623">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-623">ACR</span></span>
* <span data-ttu-id="7fad9-624">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-624">Added ACR Task commands</span></span>
* <span data-ttu-id="7fad9-625">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="7fad9-625">Added quick run command</span></span>
* <span data-ttu-id="7fad9-626">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="7fad9-626">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="7fad9-627">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-627">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="7fad9-628">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="7fad9-628">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="7fad9-629">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="7fad9-629">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-630">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-630">ACS</span></span>
* <span data-ttu-id="7fad9-631">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="7fad9-631">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="7fad9-632">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="7fad9-632">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-633">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-633">AppService</span></span>

* <span data-ttu-id="7fad9-634">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="7fad9-634">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="7fad9-635">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="7fad9-635">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="7fad9-636">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="7fad9-636">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="7fad9-637">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="7fad9-637">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-638">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-638">Batch</span></span>
* <span data-ttu-id="7fad9-639">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="7fad9-639">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="7fad9-640">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="7fad9-640">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="7fad9-641">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-641">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="7fad9-642">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="7fad9-642">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7fad9-643">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7fad9-643">Batch AI</span></span> 
* <span data-ttu-id="7fad9-644">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-644">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7fad9-645">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7fad9-645">Cognitive Services</span></span>
* <span data-ttu-id="7fad9-646">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="7fad9-646">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="7fad9-647">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="7fad9-647">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="7fad9-648">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="7fad9-648">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="7fad9-649">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-649">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="7fad9-650">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-650">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="7fad9-651">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="7fad9-651">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-652">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-652">Container</span></span>
* <span data-ttu-id="7fad9-653">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="7fad9-653">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="7fad9-654">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="7fad9-654">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="7fad9-655">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-655">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="7fad9-656">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-656">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="7fad9-657">DataLake</span><span class="sxs-lookup"><span data-stu-id="7fad9-657">Datalake</span></span>
* <span data-ttu-id="7fad9-658">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-658">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="7fad9-659">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="7fad9-659">Interactive Shell</span></span>
* <span data-ttu-id="7fad9-660">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="7fad9-660">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="7fad9-661">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="7fad9-661">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-662">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-662">IoT</span></span>
* <span data-ttu-id="7fad9-663">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-663">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="7fad9-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7fad9-664">Key Vault</span></span>
* <span data-ttu-id="7fad9-665">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="7fad9-665">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-666">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-666">Network</span></span>
* <span data-ttu-id="7fad9-667">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="7fad9-667">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="7fad9-668">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="7fad9-668">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="7fad9-669">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="7fad9-669">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="7fad9-670">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="7fad9-670">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="7fad9-671">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-671">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="7fad9-672">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-672">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="7fad9-673">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="7fad9-673">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="7fad9-674">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="7fad9-674">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="7fad9-675">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="7fad9-675">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="7fad9-676">`network express-route create/update`: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="7fad9-676">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="7fad9-677">`network vnet subnet create/update`: Se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="7fad9-677">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="7fad9-678">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-678">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="7fad9-679">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="7fad9-679">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="7fad9-680">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="7fad9-680">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="7fad9-681">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="7fad9-681">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="7fad9-682">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="7fad9-682">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="7fad9-683">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="7fad9-683">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="7fad9-684">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="7fad9-684">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-685">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-685">RDBMS</span></span>
* <span data-ttu-id="7fad9-686">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-686">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="7fad9-687">Reserva</span><span class="sxs-lookup"><span data-stu-id="7fad9-687">Reservation</span></span>
* <span data-ttu-id="7fad9-688">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="7fad9-688">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="7fad9-689">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-689">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="7fad9-690">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="7fad9-690">Manage App</span></span>
* <span data-ttu-id="7fad9-691">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="7fad9-691">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="7fad9-692">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="7fad9-692">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-693">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-693">Role</span></span>
* <span data-ttu-id="7fad9-694">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="7fad9-694">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="7fad9-695">SignalR</span><span class="sxs-lookup"><span data-stu-id="7fad9-695">SignalR</span></span>
* <span data-ttu-id="7fad9-696">Primera versión</span><span class="sxs-lookup"><span data-stu-id="7fad9-696">First release</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-697">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-697">Storage</span></span>
* <span data-ttu-id="7fad9-698">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="7fad9-698">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="7fad9-699">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="7fad9-699">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-700">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-700">VM</span></span>
* <span data-ttu-id="7fad9-701">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="7fad9-701">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="7fad9-702">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="7fad9-702">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="7fad9-703">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-703">August 28, 2018</span></span>

<span data-ttu-id="7fad9-704">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="7fad9-704">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-705">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-705">Core</span></span>

* <span data-ttu-id="7fad9-706">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="7fad9-706">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="7fad9-707">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7fad9-707">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-708">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-708">ACR</span></span>

* <span data-ttu-id="7fad9-709">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="7fad9-709">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="7fad9-710">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="7fad9-710">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-711">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-711">ACS</span></span>

* <span data-ttu-id="7fad9-712">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="7fad9-712">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="7fad9-713">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="7fad9-713">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-714">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-714">AppService</span></span>

* <span data-ttu-id="7fad9-715">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="7fad9-715">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="7fad9-716">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-716">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="7fad9-717">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-717">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="7fad9-718">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7fad9-718">Backup</span></span>

* <span data-ttu-id="7fad9-719">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-719">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="7fad9-720">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="7fad9-720">Bot Service</span></span>

* <span data-ttu-id="7fad9-721">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="7fad9-721">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7fad9-722">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7fad9-722">Cognitive Services</span></span>

* <span data-ttu-id="7fad9-723">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="7fad9-723">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-724">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-724">IoT</span></span>

* <span data-ttu-id="7fad9-725">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="7fad9-725">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-726">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-726">Monitor</span></span>

* <span data-ttu-id="7fad9-727">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="7fad9-727">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="7fad9-728">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="7fad9-728">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-729">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-729">Network</span></span>

* <span data-ttu-id="7fad9-730">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-730">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-731">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-731">Resource</span></span>

* <span data-ttu-id="7fad9-732">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-732">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-733">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-733">Storage</span></span>

* <span data-ttu-id="7fad9-734">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-734">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-735">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-735">VM</span></span>

* <span data-ttu-id="7fad9-736">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-736">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="7fad9-737">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-737">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="7fad9-738">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-738">Auguest 14, 2018</span></span>

<span data-ttu-id="7fad9-739">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="7fad9-739">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-740">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-740">Core</span></span>

* <span data-ttu-id="7fad9-741">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="7fad9-741">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="7fad9-742">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="7fad9-742">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="7fad9-743">Telemetría</span><span class="sxs-lookup"><span data-stu-id="7fad9-743">Telemetry</span></span>

* <span data-ttu-id="7fad9-744">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="7fad9-744">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-745">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-745">ACR</span></span>

* <span data-ttu-id="7fad9-746">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-746">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="7fad9-747">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="7fad9-747">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-748">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-748">ACS</span></span>

* <span data-ttu-id="7fad9-749">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="7fad9-749">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="7fad9-750">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="7fad9-750">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="7fad9-751">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="7fad9-751">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="7fad9-752">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="7fad9-752">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="7fad9-753">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="7fad9-753">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="7fad9-754">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-754">AppService</span></span>

* <span data-ttu-id="7fad9-755">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7fad9-755">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="7fad9-756">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="7fad9-756">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="7fad9-757">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7fad9-757">BatchAI</span></span>

* <span data-ttu-id="7fad9-758">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="7fad9-758">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="7fad9-759">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-759">Container</span></span>

* <span data-ttu-id="7fad9-760">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-760">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="7fad9-761">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-761">IoT</span></span>

* <span data-ttu-id="7fad9-762">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="7fad9-762">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="7fad9-763">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="7fad9-763">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="7fad9-764">Iot Central</span><span class="sxs-lookup"><span data-stu-id="7fad9-764">Iot Central</span></span>

* <span data-ttu-id="7fad9-765">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7fad9-765">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-766">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7fad9-766">KeyVault</span></span>


* <span data-ttu-id="7fad9-767">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="7fad9-767">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="7fad9-768">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="7fad9-768">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="7fad9-769">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="7fad9-769">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="7fad9-770">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="7fad9-770">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="7fad9-771">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="7fad9-771">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="7fad9-772">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-772">Relay</span></span>

* <span data-ttu-id="7fad9-773">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7fad9-773">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-774">Sql</span><span class="sxs-lookup"><span data-stu-id="7fad9-774">Sql</span></span>

* <span data-ttu-id="7fad9-775">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-775">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-776">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-776">Storage</span></span>

* <span data-ttu-id="7fad9-777">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="7fad9-777">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="7fad9-778">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="7fad9-778">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="7fad9-779">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="7fad9-779">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="7fad9-780">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="7fad9-780">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="7fad9-781">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-781">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-782">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-782">VM</span></span>

* <span data-ttu-id="7fad9-783">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="7fad9-783">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="7fad9-784">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-784">July 31, 2018</span></span>

<span data-ttu-id="7fad9-785">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="7fad9-785">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-786">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-786">ACR</span></span>

* <span data-ttu-id="7fad9-787">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-787">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="7fad9-788">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-788">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-789">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-789">ACS</span></span>

* <span data-ttu-id="7fad9-790">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="7fad9-790">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-791">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-791">Batch</span></span>

* <span data-ttu-id="7fad9-792">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="7fad9-792">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-793">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-793">Container</span></span>

* <span data-ttu-id="7fad9-794">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="7fad9-794">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-795">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-795">Network</span></span>

* <span data-ttu-id="7fad9-796">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7fad9-796">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="7fad9-797">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-797">Resource</span></span>

* <span data-ttu-id="7fad9-798">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="7fad9-798">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="7fad9-799">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="7fad9-799">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-800">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-800">Role</span></span>

* <span data-ttu-id="7fad9-801">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="7fad9-801">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="7fad9-802">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-802">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="7fad9-803">Search</span><span class="sxs-lookup"><span data-stu-id="7fad9-803">Search</span></span>

* <span data-ttu-id="7fad9-804">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="7fad9-804">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="7fad9-805">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="7fad9-805">Service Bus</span></span>

* <span data-ttu-id="7fad9-806">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="7fad9-806">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="7fad9-807">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="7fad9-807">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="7fad9-808">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="7fad9-808">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="7fad9-809">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="7fad9-809">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-810">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-810">Storage</span></span>

* <span data-ttu-id="7fad9-811">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="7fad9-811">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="7fad9-812">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-812">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-813">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-813">VM</span></span>

* <span data-ttu-id="7fad9-814">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="7fad9-814">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="7fad9-815">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="7fad9-815">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="7fad9-816">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="7fad9-816">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="7fad9-817">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="7fad9-817">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="7fad9-818">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-818">July 18, 2018</span></span>

<span data-ttu-id="7fad9-819">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="7fad9-819">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-820">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-820">Core</span></span>

* <span data-ttu-id="7fad9-821">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="7fad9-821">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="7fad9-822">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="7fad9-822">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="7fad9-823">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-823">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-824">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-824">ACR</span></span>

* <span data-ttu-id="7fad9-825">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="7fad9-825">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="7fad9-826">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="7fad9-826">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="7fad9-827">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="7fad9-827">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="7fad9-828">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="7fad9-828">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-829">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-829">ACS</span></span>

* <span data-ttu-id="7fad9-830">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="7fad9-830">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-831">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-831">AppService</span></span>

* <span data-ttu-id="7fad9-832">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="7fad9-832">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-833">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-833">Batch</span></span>

* <span data-ttu-id="7fad9-834">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="7fad9-834">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="7fad9-835">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7fad9-835">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7fad9-836">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7fad9-836">Batch AI</span></span>

* <span data-ttu-id="7fad9-837">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="7fad9-837">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-838">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-838">Container</span></span>

* <span data-ttu-id="7fad9-839">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="7fad9-839">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="7fad9-840">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="7fad9-840">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-841">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-841">Network</span></span>

* <span data-ttu-id="7fad9-842">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-842">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="7fad9-843">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-843">Added `network nic wait`</span></span>
* <span data-ttu-id="7fad9-844">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="7fad9-844">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="7fad9-845">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-845">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="7fad9-846">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-846">Resource</span></span>

* <span data-ttu-id="7fad9-847">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7fad9-847">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="7fad9-848">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7fad9-848">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="7fad9-849">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-849">Added `deployment wait` command</span></span>
* <span data-ttu-id="7fad9-850">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="7fad9-850">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-851">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-851">SQL</span></span>

* <span data-ttu-id="7fad9-852">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-852">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="7fad9-853">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="7fad9-853">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="7fad9-854">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="7fad9-854">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-855">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-855">Storage</span></span>

* <span data-ttu-id="7fad9-856">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="7fad9-856">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-857">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-857">VM</span></span>

* <span data-ttu-id="7fad9-858">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="7fad9-858">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="7fad9-859">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-859">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="7fad9-860">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-860">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7fad9-861">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-861">July 3, 2018</span></span>

<span data-ttu-id="7fad9-862">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="7fad9-862">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="7fad9-863">AKS</span><span class="sxs-lookup"><span data-stu-id="7fad9-863">AKS</span></span>

* <span data-ttu-id="7fad9-864">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="7fad9-864">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7fad9-865">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-865">July 3, 2018</span></span>

<span data-ttu-id="7fad9-866">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="7fad9-866">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-867">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-867">Core</span></span>

* <span data-ttu-id="7fad9-868">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="7fad9-868">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-869">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-869">ACR</span></span>

* <span data-ttu-id="7fad9-870">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="7fad9-870">Added polling build status</span></span>
* <span data-ttu-id="7fad9-871">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="7fad9-871">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="7fad9-872">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="7fad9-872">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-873">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-873">ACS</span></span>

* <span data-ttu-id="7fad9-874">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-874">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="7fad9-875">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="7fad9-875">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="7fad9-876">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-876">Updated options for `aks browse` command.</span></span> <span data-ttu-id="7fad9-877">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="7fad9-877">Added `--listen-port` support</span></span>
* <span data-ttu-id="7fad9-878">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-878">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="7fad9-879">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="7fad9-879">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="7fad9-880">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="7fad9-880">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-881">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-881">AppService</span></span>

* <span data-ttu-id="7fad9-882">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="7fad9-882">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="7fad9-883">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="7fad9-883">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="7fad9-884">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7fad9-884">Backup</span></span>

* <span data-ttu-id="7fad9-885">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="7fad9-885">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="7fad9-886">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7fad9-886">BatchAI</span></span>

* <span data-ttu-id="7fad9-887">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-887">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="7fad9-888">Nube</span><span class="sxs-lookup"><span data-stu-id="7fad9-888">Cloud</span></span>

* <span data-ttu-id="7fad9-889">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="7fad9-889">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-890">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-890">Container</span></span>

* <span data-ttu-id="7fad9-891">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="7fad9-891">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="7fad9-892">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="7fad9-892">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="7fad9-893">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="7fad9-893">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-894">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-894">Extension</span></span>

* <span data-ttu-id="7fad9-895">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="7fad9-895">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-896">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-896">Network</span></span>

* <span data-ttu-id="7fad9-897">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="7fad9-897">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7fad9-898">Rdbms</span></span>

* <span data-ttu-id="7fad9-899">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-899">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-900">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-900">Resource</span></span>

* <span data-ttu-id="7fad9-901">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="7fad9-901">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-902">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-902">VM</span></span>

* <span data-ttu-id="7fad9-903">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="7fad9-903">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="7fad9-904">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-904">June 25, 2018</span></span>

<span data-ttu-id="7fad9-905">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="7fad9-905">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="7fad9-906">CLI</span><span class="sxs-lookup"><span data-stu-id="7fad9-906">CLI</span></span>

* <span data-ttu-id="7fad9-907">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-907">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="7fad9-908">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-908">June 19, 2018</span></span>

<span data-ttu-id="7fad9-909">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="7fad9-909">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-910">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-910">Core</span></span>

* <span data-ttu-id="7fad9-911">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-911">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-912">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-912">ACR</span></span>

* <span data-ttu-id="7fad9-913">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="7fad9-913">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="7fad9-914">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="7fad9-914">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-915">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-915">ACS</span></span>

* <span data-ttu-id="7fad9-916">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-916">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="7fad9-917">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-917">Added `--update` support</span></span>
* <span data-ttu-id="7fad9-918">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="7fad9-918">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="7fad9-919">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="7fad9-919">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="7fad9-920">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="7fad9-920">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="7fad9-921">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="7fad9-921">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="7fad9-922">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7fad9-922">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="7fad9-923">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7fad9-923">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-924">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-924">AppService</span></span>

* <span data-ttu-id="7fad9-925">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="7fad9-925">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="7fad9-926">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7fad9-926">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-927">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-927">Batch</span></span>

* <span data-ttu-id="7fad9-928">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="7fad9-928">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7fad9-929">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7fad9-929">Batch AI</span></span>

* <span data-ttu-id="7fad9-930">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-930">Added support for workspaces.</span></span> <span data-ttu-id="7fad9-931">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="7fad9-931">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="7fad9-932">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-932">Added support for experiments.</span></span> <span data-ttu-id="7fad9-933">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="7fad9-933">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="7fad9-934">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="7fad9-934">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="7fad9-935">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-935">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="7fad9-936">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-936">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="7fad9-937">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-937">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="7fad9-938">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-938">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="7fad9-939">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-939">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="7fad9-940">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-940">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="7fad9-941">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-941">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="7fad9-942">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-942">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="7fad9-943">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-943">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="7fad9-944">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-944">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="7fad9-945">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-945">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="7fad9-946">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-946">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="7fad9-947">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="7fad9-947">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="7fad9-948">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="7fad9-948">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="7fad9-949">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7fad9-949">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7fad9-950">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7fad9-950">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7fad9-951">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="7fad9-951">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="7fad9-952">Mapas</span><span class="sxs-lookup"><span data-stu-id="7fad9-952">Maps</span></span>

* <span data-ttu-id="7fad9-953">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-953">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-954">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-954">Network</span></span>

* <span data-ttu-id="7fad9-955">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="7fad9-955">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="7fad9-956">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-956">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="7fad9-957">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="7fad9-957">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="7fad9-958">Reservations</span><span class="sxs-lookup"><span data-stu-id="7fad9-958">Reservations</span></span>

* <span data-ttu-id="7fad9-959">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-959">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="7fad9-960">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-960">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="7fad9-961">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-961">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="7fad9-962">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-962">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="7fad9-963">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-963">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="7fad9-964">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-964">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-965">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-965">Role</span></span>

* <span data-ttu-id="7fad9-966">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="7fad9-966">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-967">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-967">SQL</span></span>

* <span data-ttu-id="7fad9-968">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="7fad9-968">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-969">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-969">Storage</span></span>

* <span data-ttu-id="7fad9-970">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="7fad9-970">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-971">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-971">VM</span></span>

* <span data-ttu-id="7fad9-972">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-972">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="7fad9-973">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="7fad9-973">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="7fad9-974">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="7fad9-974">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7fad9-975">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-975">June 13, 2018</span></span>

<span data-ttu-id="7fad9-976">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="7fad9-976">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-977">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-977">Core</span></span>

* <span data-ttu-id="7fad9-978">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="7fad9-978">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7fad9-979">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-979">June 13, 2018</span></span>

<span data-ttu-id="7fad9-980">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="7fad9-980">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="7fad9-981">AKS</span><span class="sxs-lookup"><span data-stu-id="7fad9-981">AKS</span></span>

* <span data-ttu-id="7fad9-982">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-982">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="7fad9-983">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="7fad9-983">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="7fad9-984">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-984">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="7fad9-985">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-985">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="7fad9-986">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-986">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-987">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-987">AppService</span></span>

* <span data-ttu-id="7fad9-988">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="7fad9-988">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7fad9-989">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-989">June 5, 2018</span></span>

<span data-ttu-id="7fad9-990">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="7fad9-990">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-991">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-991">Interactive</span></span>

* <span data-ttu-id="7fad9-992">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="7fad9-992">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7fad9-993">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-993">June 5, 2018</span></span>

<span data-ttu-id="7fad9-994">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="7fad9-994">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-995">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-995">Core</span></span>

* <span data-ttu-id="7fad9-996">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="7fad9-996">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="7fad9-997">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="7fad9-997">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-998">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-998">ACR</span></span>

* <span data-ttu-id="7fad9-999">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="7fad9-999">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="7fad9-1000">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1000">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="7fad9-1001">AKS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1001">AKS</span></span>

* <span data-ttu-id="7fad9-1002">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1002">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-1003">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1003">Batch</span></span>

* <span data-ttu-id="7fad9-1004">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="7fad9-1004">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-1005">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-1005">IOT</span></span>

* <span data-ttu-id="7fad9-1006">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="7fad9-1006">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1007">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1007">Network</span></span>

* <span data-ttu-id="7fad9-1008">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1008">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7fad9-1009">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="7fad9-1009">Policy Insights</span></span>

* <span data-ttu-id="7fad9-1010">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="7fad9-1010">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="7fad9-1011">ARM</span><span class="sxs-lookup"><span data-stu-id="7fad9-1011">ARM</span></span>

* <span data-ttu-id="7fad9-1012">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1012">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1013">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1013">SQL</span></span>

* <span data-ttu-id="7fad9-1014">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1014">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="7fad9-1015">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1015">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="7fad9-1016">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1016">Storage</span></span>

* <span data-ttu-id="7fad9-1017">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1017">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1018">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1018">VM</span></span>

* <span data-ttu-id="7fad9-1019">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1019">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="7fad9-1020">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1020">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="7fad9-1021">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1021">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="7fad9-1022">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1022">May 22, 2018</span></span>

<span data-ttu-id="7fad9-1023">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="7fad9-1023">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1024">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1024">Core</span></span>

* <span data-ttu-id="7fad9-1025">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1025">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1026">ACS</span></span>

* <span data-ttu-id="7fad9-1027">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1027">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="7fad9-1028">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="7fad9-1028">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1029">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-1029">AppService</span></span>

* <span data-ttu-id="7fad9-1030">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1030">Improved generic update commands</span></span>
* <span data-ttu-id="7fad9-1031">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1031">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1032">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1032">Container</span></span>

* <span data-ttu-id="7fad9-1033">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="7fad9-1033">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="7fad9-1034">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-1034">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1035">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1035">Extension</span></span>

* <span data-ttu-id="7fad9-1036">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="7fad9-1036">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1037">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1037">Interactive</span></span>

* <span data-ttu-id="7fad9-1038">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="7fad9-1038">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="7fad9-1039">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="7fad9-1039">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-1040">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7fad9-1040">KeyVault</span></span>

* <span data-ttu-id="7fad9-1041">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="7fad9-1041">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1042">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1042">Network</span></span>

* <span data-ttu-id="7fad9-1043">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1043">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="7fad9-1044">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1044">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1045">SQL</span></span>

* <span data-ttu-id="7fad9-1046">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1046">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="7fad9-1047">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1047">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="7fad9-1048">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1048">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="7fad9-1049">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="7fad9-1049">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="7fad9-1050">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1050">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="7fad9-1051">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1051">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="7fad9-1052">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1052">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="7fad9-1053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1053">`edition`.</span></span> <span data-ttu-id="7fad9-1054">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1054">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="7fad9-1055">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1055">`elasticPoolName`.</span></span> <span data-ttu-id="7fad9-1056">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1056">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="7fad9-1057">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1057">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="7fad9-1058">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1058">`edition`.</span></span> <span data-ttu-id="7fad9-1059">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1059">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="7fad9-1060">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1060">`dtu`.</span></span> <span data-ttu-id="7fad9-1061">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1061">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="7fad9-1062">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1062">`databaseDtuMin`.</span></span> <span data-ttu-id="7fad9-1063">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1063">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="7fad9-1064">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1064">`databaseDtuMax`.</span></span> <span data-ttu-id="7fad9-1065">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1065">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="7fad9-1066">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1066">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="7fad9-1067">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1067">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1068">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1068">Storage</span></span>

* <span data-ttu-id="7fad9-1069">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1069">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="7fad9-1070">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1070">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1071">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1071">VM</span></span>

* <span data-ttu-id="7fad9-1072">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1072">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="7fad9-1073">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1073">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="7fad9-1074">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1074">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="7fad9-1075">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="7fad9-1075">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="7fad9-1076">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1076">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="7fad9-1077">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1077">May 7, 2018</span></span>

<span data-ttu-id="7fad9-1078">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="7fad9-1078">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1079">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1079">Core</span></span>

* <span data-ttu-id="7fad9-1080">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="7fad9-1080">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="7fad9-1081">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="7fad9-1081">Added limited support for positional arguments</span></span>
* <span data-ttu-id="7fad9-1082">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1082">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="7fad9-1083">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="7fad9-1083">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="7fad9-1084">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1084">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="7fad9-1085">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="7fad9-1085">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="7fad9-1086">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1086">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="7fad9-1087">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1087">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="7fad9-1088">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1088">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-1089">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-1089">ACR</span></span>

* <span data-ttu-id="7fad9-1090">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="7fad9-1090">Added ACR Build commands</span></span>
* <span data-ttu-id="7fad9-1091">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="7fad9-1091">Improved resource not found error messages</span></span>
* <span data-ttu-id="7fad9-1092">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="7fad9-1092">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="7fad9-1093">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1093">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="7fad9-1094">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-1094">Improved repository commands error messages</span></span>
* <span data-ttu-id="7fad9-1095">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="7fad9-1095">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1096">ACS</span></span>

* <span data-ttu-id="7fad9-1097">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1097">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="7fad9-1098">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1098">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="7fad9-1099">AMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1099">AMS</span></span>

* <span data-ttu-id="7fad9-1100">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="7fad9-1100">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1101">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1101">Appservice</span></span>

* <span data-ttu-id="7fad9-1102">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1102">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="7fad9-1103">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1103">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="7fad9-1104">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="7fad9-1104">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="7fad9-1105">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-1105">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7fad9-1106">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1106">Batch AI</span></span>

* <span data-ttu-id="7fad9-1107">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="7fad9-1107">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7fad9-1108">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7fad9-1108">Cognitive Services</span></span>

* <span data-ttu-id="7fad9-1109">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1109">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="7fad9-1110">Consumo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1110">Consumption</span></span>

* <span data-ttu-id="7fad9-1111">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1111">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1112">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1112">Container</span></span>

* <span data-ttu-id="7fad9-1113">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="7fad9-1113">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7fad9-1114">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7fad9-1114">Cosmos DB</span></span>

* <span data-ttu-id="7fad9-1115">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7fad9-1115">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="7fad9-1116">DMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1116">DMS</span></span>

* <span data-ttu-id="7fad9-1117">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1117">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1118">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1118">Extension</span></span>

* <span data-ttu-id="7fad9-1119">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="7fad9-1119">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1120">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1120">Interactive</span></span>

* <span data-ttu-id="7fad9-1121">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="7fad9-1121">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="7fad9-1122">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="7fad9-1122">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="7fad9-1123">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="7fad9-1123">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="7fad9-1124">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1124">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="7fad9-1125">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-1125">Lab</span></span>

* <span data-ttu-id="7fad9-1126">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="7fad9-1126">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1127">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1127">Network</span></span>

* <span data-ttu-id="7fad9-1128">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1128">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="7fad9-1129">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1129">Profile</span></span>

* <span data-ttu-id="7fad9-1130">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1130">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="7fad9-1131">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="7fad9-1131">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="7fad9-1132">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1132">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="7fad9-1133">Redis</span><span class="sxs-lookup"><span data-stu-id="7fad9-1133">Redis</span></span>

* <span data-ttu-id="7fad9-1134">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1134">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="7fad9-1135">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1135">Deprecated `redis list-all`.</span></span> <span data-ttu-id="7fad9-1136">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1136">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="7fad9-1137">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1137">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="7fad9-1138">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1138">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-1139">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-1139">Role</span></span>

* <span data-ttu-id="7fad9-1140">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1140">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1141">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1141">Storage</span></span>

* <span data-ttu-id="7fad9-1142">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="7fad9-1142">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="7fad9-1143">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="7fad9-1143">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="7fad9-1144">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1144">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="7fad9-1145">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="7fad9-1145">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="7fad9-1146">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="7fad9-1146">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1147">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1147">VM</span></span>

* <span data-ttu-id="7fad9-1148">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="7fad9-1148">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="7fad9-1149">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="7fad9-1149">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="7fad9-1150">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1150">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="7fad9-1151">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1151">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="7fad9-1152">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1152">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="7fad9-1153">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="7fad9-1153">Added write accelerator support</span></span>
* <span data-ttu-id="7fad9-1154">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1154">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="7fad9-1155">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="7fad9-1155">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="7fad9-1156">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="7fad9-1156">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="7fad9-1157">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1157">April 10, 2018</span></span>

<span data-ttu-id="7fad9-1158">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="7fad9-1158">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-1159">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-1159">ACR</span></span>

* <span data-ttu-id="7fad9-1160">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="7fad9-1160">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1161">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1161">ACS</span></span>

* <span data-ttu-id="7fad9-1162">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="7fad9-1162">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1163">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1163">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="7fad9-1165">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="7fad9-1165">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="7fad9-1166">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1166">BatchAI</span></span>

* <span data-ttu-id="7fad9-1167">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="7fad9-1167">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="7fad9-1168">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1168">Job level mounting</span></span>
  - <span data-ttu-id="7fad9-1169">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="7fad9-1169">Environment variables with secret values</span></span>
  - <span data-ttu-id="7fad9-1170">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1170">Performance counters settings</span></span>
  - <span data-ttu-id="7fad9-1171">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1171">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="7fad9-1172">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1172">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="7fad9-1173">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="7fad9-1173">Usage and limits reporting</span></span>
  - <span data-ttu-id="7fad9-1174">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1174">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="7fad9-1175">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1175">Support for custom images</span></span>
  - <span data-ttu-id="7fad9-1176">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1176">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="7fad9-1177">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1177">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="7fad9-1178">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="7fad9-1178">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="7fad9-1179">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="7fad9-1179">National clouds are supported</span></span>
* <span data-ttu-id="7fad9-1180">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="7fad9-1180">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="7fad9-1181">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="7fad9-1181">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="7fad9-1182">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1182">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="7fad9-1183">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1183">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="7fad9-1184">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1184">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="7fad9-1185">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1185">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="7fad9-1186">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1186">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="7fad9-1187">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1187">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="7fad9-1188">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="7fad9-1188">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="7fad9-1189">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1189">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="7fad9-1190">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1190">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="7fad9-1191">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1191">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="7fad9-1192">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1192">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="7fad9-1193">Facturación</span><span class="sxs-lookup"><span data-stu-id="7fad9-1193">Billing</span></span>

* <span data-ttu-id="7fad9-1194">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="7fad9-1194">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="7fad9-1195">Consumo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1195">Consumption</span></span>

* <span data-ttu-id="7fad9-1196">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1196">Added `marketplace` commands</span></span>
* <span data-ttu-id="7fad9-1197">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1197">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="7fad9-1198">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1198">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="7fad9-1199">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1199">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="7fad9-1200">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1200">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="7fad9-1201">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1201">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1202">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1202">Container</span></span>

* <span data-ttu-id="7fad9-1203">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1203">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="7fad9-1204">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="7fad9-1204">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1205">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1205">Extension</span></span>

* <span data-ttu-id="7fad9-1206">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="7fad9-1206">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1207">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1207">Interactive</span></span>

* <span data-ttu-id="7fad9-1208">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1208">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="7fad9-1209">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1209">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="7fad9-1210">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1210">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1211">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1211">Network</span></span>

* <span data-ttu-id="7fad9-1212">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1212">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="7fad9-1213">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1213">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="7fad9-1214">4910</span><span class="sxs-lookup"><span data-stu-id="7fad9-1214">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="7fad9-1215">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="7fad9-1215">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="7fad9-1216">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="7fad9-1216">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="7fad9-1217">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1217">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="7fad9-1218">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1218">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="7fad9-1219">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1219">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-1220">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1220">Profile</span></span>

* <span data-ttu-id="7fad9-1221">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1221">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="7fad9-1222">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1222">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-1223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1223">RDBMS</span></span>

* <span data-ttu-id="7fad9-1224">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1224">Added `georestore` command</span></span>
* <span data-ttu-id="7fad9-1225">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1225">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1226">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1226">Resource</span></span>

* <span data-ttu-id="7fad9-1227">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1227">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="7fad9-1228">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1228">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1229">SQL</span></span>

* <span data-ttu-id="7fad9-1230">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1230">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1231">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1231">Storage</span></span>

* <span data-ttu-id="7fad9-1232">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="7fad9-1232">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1233">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1233">VM</span></span>

* <span data-ttu-id="7fad9-1234">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1234">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="7fad9-1235">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="7fad9-1235">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="7fad9-1237">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1237">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="7fad9-1238">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1238">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="7fad9-1239">5718</span><span class="sxs-lookup"><span data-stu-id="7fad9-1239">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="7fad9-1240">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1240">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="7fad9-1241">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1241">March 27, 2018</span></span>

<span data-ttu-id="7fad9-1242">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="7fad9-1242">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1243">Core</span></span>

* <span data-ttu-id="7fad9-1244">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="7fad9-1244">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1245">ACS</span></span>

* <span data-ttu-id="7fad9-1246">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7fad9-1246">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1247">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1247">Appservice</span></span>

* <span data-ttu-id="7fad9-1248">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1248">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="7fad9-1249">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1249">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7fad9-1250">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7fad9-1250">Backup</span></span>

* <span data-ttu-id="7fad9-1251">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1251">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="7fad9-1252">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1252">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="7fad9-1253">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1253">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="7fad9-1254">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1254">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1255">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1255">Container</span></span>

* <span data-ttu-id="7fad9-1256">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1256">Added `container exec` command.</span></span> <span data-ttu-id="7fad9-1257">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="7fad9-1257">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="7fad9-1258">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-1258">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1259">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1259">Extension</span></span>

* <span data-ttu-id="7fad9-1260">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1260">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="7fad9-1261">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1261">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="7fad9-1262">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7fad9-1262">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1263">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1263">Interactive</span></span>

* <span data-ttu-id="7fad9-1264">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1264">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="7fad9-1265">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1265">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="7fad9-1266">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1266">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="7fad9-1267">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="7fad9-1267">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="7fad9-1268">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-1268">Lab</span></span>

* <span data-ttu-id="7fad9-1269">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1269">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1270">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1270">Monitor</span></span>

* <span data-ttu-id="7fad9-1271">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1271">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="7fad9-1272">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1272">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="7fad9-1273">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1273">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1274">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1274">Network</span></span>

* <span data-ttu-id="7fad9-1275">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1275">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-1276">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1276">Profile</span></span>

* <span data-ttu-id="7fad9-1277">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1277">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-1278">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1278">RDBMS</span></span>

* <span data-ttu-id="7fad9-1279">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="7fad9-1279">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1280">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1280">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="7fad9-1282">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-1282">Role</span></span>

* <span data-ttu-id="7fad9-1283">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1283">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="7fad9-1284">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="7fad9-1284">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="7fad9-1285">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1285">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="7fad9-1286">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1286">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="7fad9-1287">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1287">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1288">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1288">Storage</span></span>

* <span data-ttu-id="7fad9-1289">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="7fad9-1289">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="7fad9-1290">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="7fad9-1290">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1291">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1291">VM</span></span>

* <span data-ttu-id="7fad9-1292">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="7fad9-1292">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="7fad9-1293">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1293">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="7fad9-1294">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="7fad9-1294">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="7fad9-1295">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="7fad9-1295">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="7fad9-1296">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1296">March 13, 2018</span></span>

<span data-ttu-id="7fad9-1297">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="7fad9-1297">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-1298">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-1298">ACR</span></span>

* <span data-ttu-id="7fad9-1299">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1299">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="7fad9-1300">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1300">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="7fad9-1301">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1301">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1302">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1302">ACS</span></span>

* <span data-ttu-id="7fad9-1303">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1303">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="7fad9-1304">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1304">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="7fad9-1305">Advisor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1305">Advisor</span></span>

* <span data-ttu-id="7fad9-1306">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1306">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="7fad9-1307">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1307">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="7fad9-1308">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1308">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="7fad9-1309">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1309">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="7fad9-1310">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1310">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1311">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1311">Appservice</span></span>

* <span data-ttu-id="7fad9-1312">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1312">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="7fad9-1313">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1313">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7fad9-1314">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="7fad9-1314">Eventhubs</span></span>

* <span data-ttu-id="7fad9-1315">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1315">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1316">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1316">Extension</span></span>

* <span data-ttu-id="7fad9-1317">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1317">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1318">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1318">Interactive</span></span>

* <span data-ttu-id="7fad9-1319">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1319">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="7fad9-1320">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1320">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="7fad9-1321">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1321">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="7fad9-1322">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1322">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1323">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1323">Monitor</span></span>

* <span data-ttu-id="7fad9-1324">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1324">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="7fad9-1325">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1325">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="7fad9-1326">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1326">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="7fad9-1327">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1327">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1328">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1328">Network</span></span>

* <span data-ttu-id="7fad9-1329">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1329">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="7fad9-1330">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1330">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="7fad9-1331">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1331">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="7fad9-1332">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1332">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-1333">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1333">Profile</span></span>

* <span data-ttu-id="7fad9-1334">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1334">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="7fad9-1335">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1335">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-1336">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1336">RDBMS</span></span>

* <span data-ttu-id="7fad9-1337">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="7fad9-1337">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="7fad9-1338">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="7fad9-1338">Service Bus</span></span>

* <span data-ttu-id="7fad9-1339">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1339">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1340">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1340">Storage</span></span>

* <span data-ttu-id="7fad9-1341">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1341">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="7fad9-1342">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1342">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1343">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1343">VM</span></span>

* <span data-ttu-id="7fad9-1344">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1344">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="7fad9-1345">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1345">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="7fad9-1346">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1346">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="7fad9-1347">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1347">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="7fad9-1348">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1348">February 27, 2018</span></span>

<span data-ttu-id="7fad9-1349">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="7fad9-1349">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1350">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1350">Core</span></span>

* <span data-ttu-id="7fad9-1351">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="7fad9-1351">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="7fad9-1352">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1352">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="7fad9-1353">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1353">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1354">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1354">ACS</span></span>

* <span data-ttu-id="7fad9-1355">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7fad9-1355">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="7fad9-1356">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1356">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="7fad9-1357">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1357">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="7fad9-1358">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1358">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1359">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1359">Appservice</span></span>

* <span data-ttu-id="7fad9-1360">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1360">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="7fad9-1361">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="7fad9-1361">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7fad9-1362">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7fad9-1362">Cognitive Services</span></span>

* <span data-ttu-id="7fad9-1363">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7fad9-1363">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="7fad9-1364">Consumo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1364">Consumption</span></span>

* <span data-ttu-id="7fad9-1365">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="7fad9-1365">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="7fad9-1366">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="7fad9-1366">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1367">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1367">Container</span></span>

* <span data-ttu-id="7fad9-1368">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1368">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1369">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1369">Network</span></span>

* <span data-ttu-id="7fad9-1370">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1370">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1371">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1371">Resource</span></span>

* <span data-ttu-id="7fad9-1372">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="7fad9-1372">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-1373">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-1373">Role</span></span>

* <span data-ttu-id="7fad9-1374">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="7fad9-1374">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1375">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1375">SQL</span></span>

* <span data-ttu-id="7fad9-1376">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="7fad9-1376">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1377">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1377">Storage</span></span>

* <span data-ttu-id="7fad9-1378">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1378">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1379">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1379">VM</span></span>

* <span data-ttu-id="7fad9-1380">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1380">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="7fad9-1381">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1381">February 13, 2018</span></span>

<span data-ttu-id="7fad9-1382">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="7fad9-1382">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1383">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1383">Core</span></span>

* <span data-ttu-id="7fad9-1384">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="7fad9-1384">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1385">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1385">ACS</span></span>

* <span data-ttu-id="7fad9-1386">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1386">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="7fad9-1387">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1387">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="7fad9-1388">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7fad9-1388">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="7fad9-1389">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1389">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="7fad9-1390">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="7fad9-1390">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="7fad9-1391">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1391">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="7fad9-1392">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7fad9-1392">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="7fad9-1393">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1393">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1394">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1394">Appservice</span></span>

* <span data-ttu-id="7fad9-1395">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="7fad9-1395">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="7fad9-1396">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1396">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="7fad9-1397">CDN</span><span class="sxs-lookup"><span data-stu-id="7fad9-1397">CDN</span></span>

* <span data-ttu-id="7fad9-1398">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1398">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1399">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1399">Container</span></span>

* <span data-ttu-id="7fad9-1400">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="7fad9-1400">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="7fad9-1401">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-1401">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-1402">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-1402">CosmosDB</span></span>

* <span data-ttu-id="7fad9-1403">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="7fad9-1403">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1404">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1404">Extension</span></span>

* <span data-ttu-id="7fad9-1405">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1405">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="7fad9-1406">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1406">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="7fad9-1407">Comentarios</span><span class="sxs-lookup"><span data-stu-id="7fad9-1407">Feedback</span></span>

* <span data-ttu-id="7fad9-1408">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="7fad9-1408">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1409">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1409">Interactive</span></span>

* <span data-ttu-id="7fad9-1410">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7fad9-1410">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="7fad9-1411">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="7fad9-1411">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-1412">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-1412">IoT</span></span>

* <span data-ttu-id="7fad9-1413">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1413">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7fad9-1414">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1414">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7fad9-1415">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1415">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="7fad9-1416">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="7fad9-1416">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1417">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1417">Monitor</span></span>

* <span data-ttu-id="7fad9-1418">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1418">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1419">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1419">Network</span></span>

* <span data-ttu-id="7fad9-1420">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1420">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="7fad9-1421">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1421">Profile</span></span>

* <span data-ttu-id="7fad9-1422">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1422">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1423">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1423">Resource</span></span>

* <span data-ttu-id="7fad9-1424">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1424">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-1425">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-1425">Role</span></span>

* <span data-ttu-id="7fad9-1426">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1426">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1427">SQL</span></span>

* <span data-ttu-id="7fad9-1428">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1428">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="7fad9-1429">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1429">Added `sql db rename`</span></span>
* <span data-ttu-id="7fad9-1430">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="7fad9-1430">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1431">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1431">Storage</span></span>

* <span data-ttu-id="7fad9-1432">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="7fad9-1432">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1433">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1433">VM</span></span>

* <span data-ttu-id="7fad9-1434">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="7fad9-1434">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="7fad9-1435">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1435">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="7fad9-1436">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="7fad9-1436">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="7fad9-1437">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1437">January 31, 2018</span></span>

<span data-ttu-id="7fad9-1438">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="7fad9-1438">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1439">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1439">Core</span></span>

* <span data-ttu-id="7fad9-1440">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1440">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="7fad9-1441">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="7fad9-1441">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="7fad9-1442">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1442">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="7fad9-1443">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1443">Use `--verbose` to see</span></span>
* <span data-ttu-id="7fad9-1444">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="7fad9-1444">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1445">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1445">ACS</span></span>

* <span data-ttu-id="7fad9-1446">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1446">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="7fad9-1447">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1447">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1448">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1448">Appservice</span></span>

* <span data-ttu-id="7fad9-1449">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="7fad9-1449">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="7fad9-1450">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="7fad9-1450">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="7fad9-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="7fad9-1451">CDN</span></span>

* <span data-ttu-id="7fad9-1452">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1452">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-1453">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-1453">CosmosDB</span></span>

* <span data-ttu-id="7fad9-1454">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="7fad9-1454">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1455">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1455">Interactive</span></span>

* <span data-ttu-id="7fad9-1456">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="7fad9-1456">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1457">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1457">Network</span></span>

* <span data-ttu-id="7fad9-1458">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1458">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="7fad9-1459">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="7fad9-1459">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="7fad9-1460">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1460">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="7fad9-1461">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1461">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="7fad9-1462">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1462">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="7fad9-1463">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1463">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="7fad9-1464">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1464">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="7fad9-1465">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="7fad9-1465">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="7fad9-1466">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1466">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="7fad9-1467">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1467">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-1468">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1468">Profile</span></span>

* <span data-ttu-id="7fad9-1469">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="7fad9-1469">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1470">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1470">Resource</span></span>

* <span data-ttu-id="7fad9-1471">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1471">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1472">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1472">Storage</span></span>

* <span data-ttu-id="7fad9-1473">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="7fad9-1473">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="7fad9-1474">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="7fad9-1474">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="7fad9-1475">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1475">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="7fad9-1476">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1476">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="7fad9-1477">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="7fad9-1477">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1478">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1478">VM</span></span>

* <span data-ttu-id="7fad9-1479">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="7fad9-1479">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="7fad9-1480">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1480">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="7fad9-1481">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="7fad9-1481">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="7fad9-1482">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1482">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="7fad9-1483">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="7fad9-1483">January 17, 2018</span></span>

<span data-ttu-id="7fad9-1484">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="7fad9-1484">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-1485">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-1485">ACR</span></span>

* <span data-ttu-id="7fad9-1486">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="7fad9-1486">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="7fad9-1487">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="7fad9-1487">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1488">ACS</span></span>

* <span data-ttu-id="7fad9-1489">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1489">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="7fad9-1490">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="7fad9-1490">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1491">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1491">Appservice</span></span>

* <span data-ttu-id="7fad9-1492">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1492">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="7fad9-1493">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1493">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="7fad9-1494">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1494">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="7fad9-1495">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7fad9-1495">Backup</span></span>

* <span data-ttu-id="7fad9-1496">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="7fad9-1496">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="7fad9-1497">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1497">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="7fad9-1498">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1498">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="7fad9-1499">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="7fad9-1499">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="7fad9-1500">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="7fad9-1500">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-1501">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1501">Batch</span></span>

* <span data-ttu-id="7fad9-1502">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="7fad9-1502">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="7fad9-1503">Nube</span><span class="sxs-lookup"><span data-stu-id="7fad9-1503">Cloud</span></span>

* <span data-ttu-id="7fad9-1504">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="7fad9-1504">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="7fad9-1505">Consumo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1505">Consumption</span></span>

* <span data-ttu-id="7fad9-1506">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1506">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="7fad9-1507">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7fad9-1507">Event Grid</span></span>

* <span data-ttu-id="7fad9-1508">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1508">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7fad9-1509">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1509">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7fad9-1510">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1510">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="7fad9-1511">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1511">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="7fad9-1512">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1512">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="7fad9-1513">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1513">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="7fad9-1514">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1514">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="7fad9-1515">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="7fad9-1515">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1516">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1516">Interactive</span></span>

* <span data-ttu-id="7fad9-1517">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="7fad9-1517">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="7fad9-1518">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="7fad9-1518">Fixed errors on startup</span></span>
* <span data-ttu-id="7fad9-1519">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1519">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-1520">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-1520">IoT</span></span>

* <span data-ttu-id="7fad9-1521">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1521">Added support for device provisioning service</span></span>
* <span data-ttu-id="7fad9-1522">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1522">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="7fad9-1523">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-1523">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1524">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1524">Monitor</span></span>

* <span data-ttu-id="7fad9-1525">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1525">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="7fad9-1526">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1526">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="7fad9-1527">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1527">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1528">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1528">Network</span></span>

* <span data-ttu-id="7fad9-1529">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1529">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="7fad9-1530">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1530">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-1531">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1531">Profile</span></span>

* <span data-ttu-id="7fad9-1532">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="7fad9-1532">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-1533">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-1533">Role</span></span>

* <span data-ttu-id="7fad9-1534">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="7fad9-1534">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7fad9-1535">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7fad9-1535">Service Fabric</span></span>

* <span data-ttu-id="7fad9-1536">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="7fad9-1536">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="7fad9-1537">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1537">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1538">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1538">VM</span></span>

* <span data-ttu-id="7fad9-1539">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1539">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="7fad9-1540">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="7fad9-1540">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="7fad9-1541">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1541">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="7fad9-1542">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1542">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="7fad9-1543">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="7fad9-1543">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="7fad9-1544">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1544">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7fad9-1545">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1545">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="7fad9-1546">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1546">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="7fad9-1547">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1547">December 19, 2017</span></span>

<span data-ttu-id="7fad9-1548">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="7fad9-1548">Version 2.0.23</span></span>

* <span data-ttu-id="7fad9-1549">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="7fad9-1549">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1550">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1550">Container</span></span>

* <span data-ttu-id="7fad9-1551">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1551">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1552">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1552">Network</span></span>

* <span data-ttu-id="7fad9-1553">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1553">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="7fad9-1554">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1554">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1555">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1555">Storage</span></span>

* <span data-ttu-id="7fad9-1556">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="7fad9-1556">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1557">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1557">VM</span></span>

* <span data-ttu-id="7fad9-1558">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="7fad9-1558">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="7fad9-1559">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1559">December 5, 2017</span></span>

<span data-ttu-id="7fad9-1560">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="7fad9-1560">Version 2.0.22</span></span>

* <span data-ttu-id="7fad9-1561">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1561">Removed `az component` commands.</span></span> <span data-ttu-id="7fad9-1562">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1562">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1563">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1563">Core</span></span>
* <span data-ttu-id="7fad9-1564">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="7fad9-1564">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="7fad9-1565">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="7fad9-1565">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1566">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1566">ACS</span></span>

* <span data-ttu-id="7fad9-1567">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1567">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="7fad9-1568">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1568">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="7fad9-1569">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="7fad9-1569">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="7fad9-1570">Advisor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1570">Advisor</span></span>

* <span data-ttu-id="7fad9-1571">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1571">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1572">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1572">Appservice</span></span>

* <span data-ttu-id="7fad9-1573">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1573">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="7fad9-1574">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1574">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="7fad9-1575">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1575">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="7fad9-1576">Consumo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1576">Consumption</span></span>

* <span data-ttu-id="7fad9-1577">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="7fad9-1577">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1578">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1578">Container</span></span>

* <span data-ttu-id="7fad9-1579">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="7fad9-1579">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1580">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1580">Monitor</span></span>

* <span data-ttu-id="7fad9-1581">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="7fad9-1581">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1582">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1582">Resource</span></span>

* <span data-ttu-id="7fad9-1583">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1583">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-1584">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-1584">Role</span></span>

* <span data-ttu-id="7fad9-1585">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1585">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="7fad9-1586">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="7fad9-1586">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="7fad9-1587">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1587">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1588">SQL</span></span>

* <span data-ttu-id="7fad9-1589">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1589">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="7fad9-1590">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1590">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1591">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1591">VM</span></span>

* <span data-ttu-id="7fad9-1592">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1592">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="7fad9-1593">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1593">November 14, 2017</span></span>

<span data-ttu-id="7fad9-1594">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="7fad9-1594">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-1595">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-1595">ACR</span></span>

* <span data-ttu-id="7fad9-1596">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="7fad9-1596">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="7fad9-1597">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1597">ACS</span></span>

* <span data-ttu-id="7fad9-1598">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1598">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="7fad9-1599">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1599">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="7fad9-1600">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1600">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="7fad9-1601">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="7fad9-1601">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="7fad9-1602">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="7fad9-1602">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1603">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1603">Appservice</span></span>

* <span data-ttu-id="7fad9-1604">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="7fad9-1604">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="7fad9-1605">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1605">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="7fad9-1606">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1606">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="7fad9-1607">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1607">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="7fad9-1608">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="7fad9-1608">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="7fad9-1609">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="7fad9-1609">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-1610">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1610">Batch</span></span>

* <span data-ttu-id="7fad9-1611">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1611">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="7fad9-1612">Batchai</span><span class="sxs-lookup"><span data-stu-id="7fad9-1612">Batchai</span></span>

* <span data-ttu-id="7fad9-1613">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1613">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="7fad9-1614">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1614">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="7fad9-1615">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1615">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="7fad9-1616">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1616">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="7fad9-1617">Nube</span><span class="sxs-lookup"><span data-stu-id="7fad9-1617">Cloud</span></span>

* <span data-ttu-id="7fad9-1618">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="7fad9-1618">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1619">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1619">Container</span></span>

* <span data-ttu-id="7fad9-1620">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1620">Added support to open multiple ports</span></span>
* <span data-ttu-id="7fad9-1621">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="7fad9-1621">Added container group restart policy</span></span>
* <span data-ttu-id="7fad9-1622">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="7fad9-1622">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="7fad9-1623">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="7fad9-1623">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7fad9-1624">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7fad9-1624">Data Lake Analytics</span></span>

* <span data-ttu-id="7fad9-1625">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="7fad9-1625">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7fad9-1626">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7fad9-1626">Data Lake Store</span></span>

* <span data-ttu-id="7fad9-1627">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="7fad9-1627">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1628">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1628">Extension</span></span>

* <span data-ttu-id="7fad9-1629">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="7fad9-1629">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="7fad9-1630">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="7fad9-1630">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-1631">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-1631">IoT</span></span>

* <span data-ttu-id="7fad9-1632">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="7fad9-1632">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1633">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1633">Monitor</span></span>

* <span data-ttu-id="7fad9-1634">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1634">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1635">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1635">Network</span></span>

* <span data-ttu-id="7fad9-1636">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="7fad9-1636">Added support for CAA DNS records</span></span>
* <span data-ttu-id="7fad9-1637">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1637">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="7fad9-1638">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1638">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="7fad9-1639">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1639">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="7fad9-1640">Reservations</span><span class="sxs-lookup"><span data-stu-id="7fad9-1640">Reservations</span></span>

* <span data-ttu-id="7fad9-1641">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="7fad9-1641">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1642">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1642">Resource</span></span>

* <span data-ttu-id="7fad9-1643">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1643">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1644">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1644">SQL</span></span>

* <span data-ttu-id="7fad9-1645">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1645">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1646">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1646">Storage</span></span>

* <span data-ttu-id="7fad9-1647">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="7fad9-1647">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="7fad9-1648">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="7fad9-1648">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="7fad9-1649">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1649">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="7fad9-1650">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1650">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="7fad9-1651">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1651">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="7fad9-1652">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1652">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="7fad9-1653">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1653">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1654">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1654">VM</span></span>

* <span data-ttu-id="7fad9-1655">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1655">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="7fad9-1656">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="7fad9-1656">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="7fad9-1657">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="7fad9-1657">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="7fad9-1658">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1658">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="7fad9-1659">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1659">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="7fad9-1660">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1660">October 24, 2017</span></span>

<span data-ttu-id="7fad9-1661">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="7fad9-1661">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1662">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1662">Core</span></span>

* <span data-ttu-id="7fad9-1663">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1663">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-1664">ACR</span></span>

* <span data-ttu-id="7fad9-1665">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="7fad9-1665">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="7fad9-1666">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="7fad9-1666">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="7fad9-1667">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="7fad9-1667">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1668">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1668">ACS</span></span>

* <span data-ttu-id="7fad9-1669">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1669">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="7fad9-1670">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7fad9-1670">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1671">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1671">Appservice</span></span>

* <span data-ttu-id="7fad9-1672">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1672">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="7fad9-1673">Componente</span><span class="sxs-lookup"><span data-stu-id="7fad9-1673">Component</span></span>

* <span data-ttu-id="7fad9-1674">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="7fad9-1674">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1675">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1675">Monitor</span></span>

* <span data-ttu-id="7fad9-1676">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1676">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1677">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1677">Resource</span></span>

* <span data-ttu-id="7fad9-1678">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1678">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="7fad9-1679">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1679">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1680">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1680">VM</span></span>

* <span data-ttu-id="7fad9-1681">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1681">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="7fad9-1682">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1682">October 9, 2017</span></span>

<span data-ttu-id="7fad9-1683">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="7fad9-1683">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1684">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1684">Core</span></span>

* <span data-ttu-id="7fad9-1685">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7fad9-1685">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1686">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1686">Appservice</span></span>

* <span data-ttu-id="7fad9-1687">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1687">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-1688">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1688">Batch</span></span>

* <span data-ttu-id="7fad9-1689">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="7fad9-1689">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="7fad9-1690">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="7fad9-1690">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="7fad9-1691">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1691">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="7fad9-1692">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="7fad9-1692">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="7fad9-1693">Batchai</span><span class="sxs-lookup"><span data-stu-id="7fad9-1693">Batchai</span></span>

* <span data-ttu-id="7fad9-1694">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1694">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-1695">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7fad9-1695">Keyvault</span></span>

* <span data-ttu-id="7fad9-1696">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1696">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="7fad9-1697">(#4448)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1697">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="7fad9-1698">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1698">Network</span></span>

* <span data-ttu-id="7fad9-1699">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1699">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="7fad9-1700">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="7fad9-1700">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1701">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1701">Resource</span></span>

* <span data-ttu-id="7fad9-1702">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1702">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="7fad9-1703">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="7fad9-1703">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="7fad9-1704">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1704">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="7fad9-1705">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1705">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1706">Sql</span><span class="sxs-lookup"><span data-stu-id="7fad9-1706">Sql</span></span>

* <span data-ttu-id="7fad9-1707">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="7fad9-1707">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="7fad9-1708">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1708">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="7fad9-1709">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1709">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1710">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1710">Storage</span></span>

* <span data-ttu-id="7fad9-1711">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="7fad9-1711">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1712">Vm</span><span class="sxs-lookup"><span data-stu-id="7fad9-1712">Vm</span></span>

* <span data-ttu-id="7fad9-1713">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="7fad9-1713">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="7fad9-1714">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1714">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="7fad9-1715">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1715">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="7fad9-1716">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1716">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="7fad9-1717">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1717">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="7fad9-1718">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1718">September 22, 2017</span></span>

<span data-ttu-id="7fad9-1719">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="7fad9-1719">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1720">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1720">Resource</span></span>

* <span data-ttu-id="7fad9-1721">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="7fad9-1721">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="7fad9-1722">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="7fad9-1722">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="7fad9-1723">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1723">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="7fad9-1724">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1724">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1725">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1725">Network</span></span>

* <span data-ttu-id="7fad9-1726">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1726">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="7fad9-1727">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1727">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="7fad9-1728">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1728">Added `asg` application security group commands</span></span>
* <span data-ttu-id="7fad9-1729">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1729">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="7fad9-1730">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1730">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7fad9-1731">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1731">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="7fad9-1732">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1732">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1733">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1733">Storage</span></span>

* <span data-ttu-id="7fad9-1734">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="7fad9-1734">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7fad9-1735">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="7fad9-1735">Eventgrid</span></span>

* <span data-ttu-id="7fad9-1736">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="7fad9-1736">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1737">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1737">SQL</span></span>

* <span data-ttu-id="7fad9-1738">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1738">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="7fad9-1739">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="7fad9-1739">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="7fad9-1740">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1740">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-1741">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7fad9-1741">Keyvault</span></span>

* <span data-ttu-id="7fad9-1742">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="7fad9-1742">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1743">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1743">VM</span></span>

* <span data-ttu-id="7fad9-1744">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1744">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="7fad9-1745">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="7fad9-1745">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="7fad9-1746">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1746">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="7fad9-1747">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1747">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="7fad9-1748">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1748">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="7fad9-1749">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1749">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1750">ACS</span></span>

* <span data-ttu-id="7fad9-1751">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1751">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1752">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1752">Appservice</span></span>

* <span data-ttu-id="7fad9-1753">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1753">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7fad9-1754">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="7fad9-1754">Backup</span></span>

* <span data-ttu-id="7fad9-1755">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1755">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="7fad9-1756">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1756">September 11, 2017</span></span>

<span data-ttu-id="7fad9-1757">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="7fad9-1757">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="7fad9-1758">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1758">Core</span></span>

* <span data-ttu-id="7fad9-1759">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1759">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="7fad9-1760">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1760">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1761">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1761">Acs</span></span>

* <span data-ttu-id="7fad9-1762">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1762">Added `acs list-locations` command</span></span>
* <span data-ttu-id="7fad9-1763">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1763">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1764">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1764">Appservice</span></span>

* <span data-ttu-id="7fad9-1765">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1765">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="7fad9-1766">CDN</span><span class="sxs-lookup"><span data-stu-id="7fad9-1766">CDN</span></span>

* <span data-ttu-id="7fad9-1767">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1767">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="7fad9-1768">Extensión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1768">Extension</span></span>

* <span data-ttu-id="7fad9-1769">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="7fad9-1769">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-1770">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7fad9-1770">Keyvault</span></span>

* <span data-ttu-id="7fad9-1771">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1771">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1772">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1772">Network</span></span>

* <span data-ttu-id="7fad9-1773">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1773">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7fad9-1774">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1774">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="7fad9-1775">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1775">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="7fad9-1776">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1776">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7fad9-1777">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1777">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-1778">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-1778">Resource</span></span>

* <span data-ttu-id="7fad9-1779">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1779">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="7fad9-1780">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1780">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="7fad9-1781">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1781">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="7fad9-1782">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="7fad9-1782">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-1783">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-1783">SQL</span></span>

* <span data-ttu-id="7fad9-1784">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1784">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1785">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1785">VM</span></span>

* <span data-ttu-id="7fad9-1786">Problema corregido: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1786">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="7fad9-1787">Problema corregido: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1787">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="7fad9-1788">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1788">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="7fad9-1789">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1789">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="7fad9-1790">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1790">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="7fad9-1791">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1791">August 31, 2017</span></span>

<span data-ttu-id="7fad9-1792">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="7fad9-1792">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-1793">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7fad9-1793">Keyvault</span></span>

* <span data-ttu-id="7fad9-1794">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1794">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="7fad9-1795">Sf</span><span class="sxs-lookup"><span data-stu-id="7fad9-1795">Sf</span></span>

* <span data-ttu-id="7fad9-1796">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1796">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1797">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1797">Storage</span></span>

* <span data-ttu-id="7fad9-1798">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1798">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="7fad9-1799">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1799">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="7fad9-1800">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1800">August 28, 2017</span></span>

<span data-ttu-id="7fad9-1801">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="7fad9-1801">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="7fad9-1802">CLI</span><span class="sxs-lookup"><span data-stu-id="7fad9-1802">CLI</span></span>

* <span data-ttu-id="7fad9-1803">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1803">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1804">ACS</span></span>

* <span data-ttu-id="7fad9-1805">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1805">Corrected preview regions</span></span>
* <span data-ttu-id="7fad9-1806">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1806">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="7fad9-1807">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="7fad9-1807">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1808">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1808">Appservice</span></span>

* <span data-ttu-id="7fad9-1809">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1809">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="7fad9-1810">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1810">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="7fad9-1811">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1811">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="7fad9-1812">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1812">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="7fad9-1813">Problema corregido: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1813">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-1814">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-1814">IoT</span></span>

* <span data-ttu-id="7fad9-1815">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1815">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1816">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1816">Network</span></span>

* <span data-ttu-id="7fad9-1817">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1817">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7fad9-1818">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1818">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="7fad9-1819">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1819">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7fad9-1820">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1820">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7fad9-1821">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1821">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-1822">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1822">Profile</span></span>

* <span data-ttu-id="7fad9-1823">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1823">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7fad9-1824">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7fad9-1824">Service Fabric</span></span>

* <span data-ttu-id="7fad9-1825">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1825">Preview release</span></span>
* <span data-ttu-id="7fad9-1826">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1826">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="7fad9-1827">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1827">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="7fad9-1828">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1828">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1829">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1829">Storage</span></span>

* <span data-ttu-id="7fad9-1830">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1830">Enabled setting blob tier</span></span>
* <span data-ttu-id="7fad9-1831">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1831">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="7fad9-1832">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1832">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="7fad9-1833">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1833">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="7fad9-1834">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1834">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="7fad9-1835">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="7fad9-1835">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1836">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1836">VM</span></span>

* <span data-ttu-id="7fad9-1837">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1837">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="7fad9-1838">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1838">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="7fad9-1839">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1839">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="7fad9-1840">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1840">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="7fad9-1841">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1841">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="7fad9-1842">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1842">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="7fad9-1843">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1843">August 15, 2017</span></span>

<span data-ttu-id="7fad9-1844">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="7fad9-1844">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1845">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1845">ACS</span></span>

* <span data-ttu-id="7fad9-1846">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7fad9-1846">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1847">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1847">Appservice</span></span>

* <span data-ttu-id="7fad9-1848">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1848">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="7fad9-1849">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7fad9-1849">Event Grid</span></span>

* <span data-ttu-id="7fad9-1850">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1850">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="7fad9-1851">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1851">August 11, 2017</span></span>

<span data-ttu-id="7fad9-1852">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="7fad9-1852">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1853">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1853">ACS</span></span>

* <span data-ttu-id="7fad9-1854">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-1854">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-1855">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1855">Batch</span></span>

* <span data-ttu-id="7fad9-1856">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1856">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="7fad9-1857">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1857">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="7fad9-1858">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1858">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="7fad9-1859">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1859">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="7fad9-1860">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1860">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="7fad9-1861">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1861">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="7fad9-1862">Componente</span><span class="sxs-lookup"><span data-stu-id="7fad9-1862">Component</span></span>

* <span data-ttu-id="7fad9-1863">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1863">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="7fad9-1864">Contenedor</span><span class="sxs-lookup"><span data-stu-id="7fad9-1864">Container</span></span>

* <span data-ttu-id="7fad9-1865">`create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1865">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="7fad9-1866">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7fad9-1866">Data Lake Store</span></span>

* <span data-ttu-id="7fad9-1867">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1867">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="7fad9-1868">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7fad9-1868">Event Grid</span></span>

* <span data-ttu-id="7fad9-1869">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1869">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1870">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1870">Network</span></span>

* <span data-ttu-id="7fad9-1871">`lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1871">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="7fad9-1872">`application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1872">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="7fad9-1873">`application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1873">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="7fad9-1874">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1874">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-1875">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-1875">Profile</span></span>

* <span data-ttu-id="7fad9-1876">`account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1876">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-1877">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-1877">Storage</span></span>

* <span data-ttu-id="7fad9-1878">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1878">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-1879">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-1879">VM</span></span>

* <span data-ttu-id="7fad9-1880">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1880">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="7fad9-1881">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1881">Exposed `list-skus` command</span></span>
* <span data-ttu-id="7fad9-1882">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1882">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="7fad9-1883">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1883">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="7fad9-1884">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1884">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="7fad9-1885">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-1885">July 28, 2017</span></span>

<span data-ttu-id="7fad9-1886">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="7fad9-1886">Version 2.0.12</span></span>

* <span data-ttu-id="7fad9-1887">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1887">Added container commands</span></span>
* <span data-ttu-id="7fad9-1888">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1888">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="7fad9-1889">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-1889">Core</span></span>

* <span data-ttu-id="7fad9-1890">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1890">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="7fad9-1891">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1891">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="7fad9-1892">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1892">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="7fad9-1893">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1893">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="7fad9-1894">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1894">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="7fad9-1895">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1895">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="7fad9-1896">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1896">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7fad9-1897">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1897">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="7fad9-1898">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1898">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="7fad9-1899">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1899">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="7fad9-1900">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1900">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="7fad9-1901">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1901">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="7fad9-1902">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1902">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="7fad9-1903">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1903">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="7fad9-1904">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1904">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="7fad9-1905">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1905">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="7fad9-1906">ACR</span><span class="sxs-lookup"><span data-stu-id="7fad9-1906">ACR</span></span>

* <span data-ttu-id="7fad9-1907">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1907">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="7fad9-1908">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1908">Support SKU update for managed registries</span></span>
* <span data-ttu-id="7fad9-1909">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1909">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="7fad9-1910">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1910">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="7fad9-1911">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1911">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="7fad9-1912">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1912">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-1913">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-1913">ACS</span></span>

* <span data-ttu-id="7fad9-1914">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1914">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-1915">Appservice</span><span class="sxs-lookup"><span data-stu-id="7fad9-1915">Appservice</span></span>

* <span data-ttu-id="7fad9-1916">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1916">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="7fad9-1917">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1917">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="7fad9-1918">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1918">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="7fad9-1919">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1919">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="7fad9-1920">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1920">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="7fad9-1921">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1921">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="7fad9-1922">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1922">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="7fad9-1923">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1923">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="7fad9-1924">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1924">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="7fad9-1925">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1925">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="7fad9-1926">Batch</span><span class="sxs-lookup"><span data-stu-id="7fad9-1926">Batch</span></span>

* <span data-ttu-id="7fad9-1927">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1927">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="7fad9-1928">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1928">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="7fad9-1929">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1929">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="7fad9-1930">CDN</span><span class="sxs-lookup"><span data-stu-id="7fad9-1930">CDN</span></span>

* <span data-ttu-id="7fad9-1931">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="7fad9-1931">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="7fad9-1932">Nube</span><span class="sxs-lookup"><span data-stu-id="7fad9-1932">Cloud</span></span>

* <span data-ttu-id="7fad9-1933">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1933">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="7fad9-1934">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1934">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="7fad9-1935">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1935">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="7fad9-1936">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1936">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="7fad9-1937">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1937">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-1938">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-1938">CosmosDB</span></span>

* <span data-ttu-id="7fad9-1939">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1939">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="7fad9-1940">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="7fad9-1940">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7fad9-1941">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7fad9-1941">Data Lake Analytics</span></span>

* <span data-ttu-id="7fad9-1942">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1942">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="7fad9-1943">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1943">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="7fad9-1944">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1944">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7fad9-1945">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7fad9-1945">Data Lake Store</span></span>

* <span data-ttu-id="7fad9-1946">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1946">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="7fad9-1947">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1947">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="7fad9-1948">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1948">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="7fad9-1949">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1949">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="7fad9-1950">Interactive</span><span class="sxs-lookup"><span data-stu-id="7fad9-1950">Interactive</span></span>

* <span data-ttu-id="7fad9-1951">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1951">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="7fad9-1952">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1952">Increased test coverage</span></span>
* <span data-ttu-id="7fad9-1953">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1953">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="7fad9-1954">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1954">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="7fad9-1955">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1955">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="7fad9-1956">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1956">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="7fad9-1957">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1957">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7fad9-1958">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1958">Added `--progress` flag</span></span>
* <span data-ttu-id="7fad9-1959">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1959">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="7fad9-1960">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1960">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="7fad9-1961">IoT</span><span class="sxs-lookup"><span data-stu-id="7fad9-1961">IoT</span></span>

* <span data-ttu-id="7fad9-1962">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1962">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="7fad9-1963">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="7fad9-1963">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="7fad9-1964">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="7fad9-1964">Key vault</span></span>

* <span data-ttu-id="7fad9-1965">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1965">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="7fad9-1966">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1966">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="7fad9-1967">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1967">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7fad9-1968">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1968">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7fad9-1969">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7fad9-1969">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="7fad9-1970">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1970">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="7fad9-1971">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="7fad9-1971">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="7fad9-1972">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1972">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="7fad9-1973">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-1973">Lab</span></span>

* <span data-ttu-id="7fad9-1974">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1974">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="7fad9-1975">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1975">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-1976">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-1976">Monitor</span></span>

* <span data-ttu-id="7fad9-1977">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="7fad9-1977">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="7fad9-1978">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1978">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="7fad9-1979">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1979">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="7fad9-1980">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1980">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="7fad9-1981">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1981">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="7fad9-1982">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="7fad9-1982">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="7fad9-1983">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1983">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="7fad9-1984">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1984">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="7fad9-1985">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1985">`location` no longer required</span></span>
  * <span data-ttu-id="7fad9-1986">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1986">Add name and ID support for target</span></span>
  * <span data-ttu-id="7fad9-1987">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1987">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="7fad9-1988">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1988">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="7fad9-1989">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1989">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="7fad9-1990">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1990">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="7fad9-1991">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1991">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="7fad9-1992">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1992">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-1993">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-1993">Network</span></span>

* <span data-ttu-id="7fad9-1994">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1994">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="7fad9-1995">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1995">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="7fad9-1996">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1996">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="7fad9-1997">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1997">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="7fad9-1998">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1998">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="7fad9-1999">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-1999">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="7fad9-2000">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2000">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="7fad9-2001">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2001">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="7fad9-2002">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2002">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="7fad9-2003">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2003">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="7fad9-2004">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2004">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="7fad9-2005">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2005">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="7fad9-2006">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2006">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="7fad9-2007">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2007">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="7fad9-2008">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2008">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="7fad9-2009">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2009">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="7fad9-2010">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2010">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="7fad9-2011">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2011">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="7fad9-2012">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2012">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="7fad9-2013">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2013">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="7fad9-2014">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2014">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="7fad9-2015">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2015">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="7fad9-2016">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2016">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="7fad9-2017">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2017">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="7fad9-2018">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2018">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="7fad9-2019">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2019">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="7fad9-2020">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2020">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-2021">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-2021">Profile</span></span>

* <span data-ttu-id="7fad9-2022">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2022">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="7fad9-2023">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2023">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="7fad9-2024">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="7fad9-2024">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="7fad9-2025">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2025">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="7fad9-2026">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2026">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="7fad9-2027">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7fad9-2027">RDBMS</span></span>

* <span data-ttu-id="7fad9-2028">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2028">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="7fad9-2029">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2029">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="7fad9-2030">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2030">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="7fad9-2031">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2031">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-2032">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-2032">Resource</span></span>

* <span data-ttu-id="7fad9-2033">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2033">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="7fad9-2034">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2034">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="7fad9-2035">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2035">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="7fad9-2036">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2036">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="7fad9-2037">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2037">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="7fad9-2038">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2038">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="7fad9-2039">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2039">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="7fad9-2040">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2040">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-2041">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-2041">Role</span></span>

* <span data-ttu-id="7fad9-2042">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2042">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="7fad9-2043">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2043">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="7fad9-2044">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2044">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="7fad9-2045">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2045">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="7fad9-2046">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2046">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7fad9-2047">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7fad9-2047">Service Fabric</span></span>
* <span data-ttu-id="7fad9-2048">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2048">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="7fad9-2049">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2049">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="7fad9-2050">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2050">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-2051">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-2051">SQL</span></span>

* <span data-ttu-id="7fad9-2052">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2052">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="7fad9-2053">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2053">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="7fad9-2054">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2054">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-2055">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-2055">Storage</span></span>

* <span data-ttu-id="7fad9-2056">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2056">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="7fad9-2057">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2057">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="7fad9-2058">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2058">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="7fad9-2059">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2059">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="7fad9-2060">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2060">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="7fad9-2061">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2061">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-2062">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-2062">VM</span></span>

* <span data-ttu-id="7fad9-2063">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="7fad9-2063">Support configuring nsg</span></span>
* <span data-ttu-id="7fad9-2064">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2064">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="7fad9-2065">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2065">Support managed service identities</span></span>
* <span data-ttu-id="7fad9-2066">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2066">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="7fad9-2067">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="7fad9-2067">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="7fad9-2068">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-2068">May 10, 2017</span></span>

<span data-ttu-id="7fad9-2069">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="7fad9-2069">Version 2.0.6</span></span>

* <span data-ttu-id="7fad9-2070">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2070">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="7fad9-2071">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2071">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="7fad9-2072">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7fad9-2072">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="7fad9-2073">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7fad9-2073">Include Cognitive Services module</span></span>
* <span data-ttu-id="7fad9-2074">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7fad9-2074">Include Service Fabric module</span></span>
* <span data-ttu-id="7fad9-2075">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="7fad9-2075">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="7fad9-2076">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="7fad9-2076">Add support for CDN commands</span></span>
* <span data-ttu-id="7fad9-2077">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="7fad9-2077">Remove Container module</span></span>
* <span data-ttu-id="7fad9-2078">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2078">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="7fad9-2079">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2079">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="7fad9-2080">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-2080">Core</span></span>

* <span data-ttu-id="7fad9-2081">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="7fad9-2081">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="7fad9-2082">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2082">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="7fad9-2083">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2083">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="7fad9-2084">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2084">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="7fad9-2085">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2085">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="7fad9-2086">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2086">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="7fad9-2087">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2087">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="7fad9-2088">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2088">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="7fad9-2089">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2089">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="7fad9-2090">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2090">core: Improved performance</span></span>
* <span data-ttu-id="7fad9-2091">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="7fad9-2091">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="7fad9-2092">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="7fad9-2092">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-2093">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-2093">ACS</span></span>

* <span data-ttu-id="7fad9-2094">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="7fad9-2094">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="7fad9-2095">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="7fad9-2095">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="7fad9-2096">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="7fad9-2096">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="7fad9-2097">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2097">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-2098">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-2098">AppService</span></span>

* <span data-ttu-id="7fad9-2099">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2099">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="7fad9-2100">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="7fad9-2100">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="7fad9-2101">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="7fad9-2101">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="7fad9-2102">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="7fad9-2102">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="7fad9-2103">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="7fad9-2103">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="7fad9-2104">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2104">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="7fad9-2105">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="7fad9-2105">support slot swap with preview</span></span>
* <span data-ttu-id="7fad9-2106">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2106">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="7fad9-2107">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2107">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7fad9-2108">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-2108">CosmosDB</span></span>

* <span data-ttu-id="7fad9-2109">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-2109">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="7fad9-2110">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="7fad9-2110">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="7fad9-2111">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="7fad9-2111">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="7fad9-2112">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="7fad9-2112">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7fad9-2113">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7fad9-2113">Data Lake Analytics</span></span>

* <span data-ttu-id="7fad9-2114">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="7fad9-2114">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="7fad9-2115">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="7fad9-2115">Add support for new catalog item type: package.</span></span> <span data-ttu-id="7fad9-2116">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2116">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="7fad9-2117">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="7fad9-2117">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="7fad9-2118">Tabla</span><span class="sxs-lookup"><span data-stu-id="7fad9-2118">Table</span></span>
  * <span data-ttu-id="7fad9-2119">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="7fad9-2119">Table valued function</span></span>
  * <span data-ttu-id="7fad9-2120">Ver</span><span class="sxs-lookup"><span data-stu-id="7fad9-2120">View</span></span>
  * <span data-ttu-id="7fad9-2121">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2121">Table Statistics.</span></span> <span data-ttu-id="7fad9-2122">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="7fad9-2122">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7fad9-2123">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7fad9-2123">Data Lake Store</span></span>

* <span data-ttu-id="7fad9-2124">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="7fad9-2124">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="7fad9-2125">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2125">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="7fad9-2126">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2126">missed help for access show.</span></span> <span data-ttu-id="7fad9-2127">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2127">adding it.</span></span> <span data-ttu-id="7fad9-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="7fad9-2129">Buscar</span><span class="sxs-lookup"><span data-stu-id="7fad9-2129">Find</span></span>

* <span data-ttu-id="7fad9-2130">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="7fad9-2130">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="7fad9-2131">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7fad9-2131">KeyVault</span></span>

* <span data-ttu-id="7fad9-2132">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="7fad9-2132">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="7fad9-2133">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="7fad9-2133">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="7fad9-2134">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="7fad9-2134">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="7fad9-2135">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="7fad9-2135">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="7fad9-2136">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2136">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="7fad9-2137">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-2137">Lab</span></span>

* <span data-ttu-id="7fad9-2138">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-2138">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="7fad9-2139">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-2139">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="7fad9-2140">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-2140">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="7fad9-2141">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-2141">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="7fad9-2142">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="7fad9-2142">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="7fad9-2143">Supervisión</span><span class="sxs-lookup"><span data-stu-id="7fad9-2143">Monitor</span></span>

* <span data-ttu-id="7fad9-2144">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2144">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="7fad9-2145">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2145">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="7fad9-2146">Red</span><span class="sxs-lookup"><span data-stu-id="7fad9-2146">Network</span></span>

* <span data-ttu-id="7fad9-2147">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2147">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="7fad9-2148">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2148">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="7fad9-2149">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="7fad9-2149">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="7fad9-2150">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="7fad9-2150">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="7fad9-2151">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="7fad9-2151">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="7fad9-2152">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7fad9-2152">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="7fad9-2153">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="7fad9-2153">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="7fad9-2154">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="7fad9-2154">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="7fad9-2155">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2155">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="7fad9-2156">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="7fad9-2156">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="7fad9-2157">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2157">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="7fad9-2158">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2158">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="7fad9-2159">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="7fad9-2159">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="7fad9-2160">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="7fad9-2160">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="7fad9-2161">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="7fad9-2161">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="7fad9-2162">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="7fad9-2162">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="7fad9-2163">Perfil</span><span class="sxs-lookup"><span data-stu-id="7fad9-2163">Profile</span></span>

* <span data-ttu-id="7fad9-2164">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2164">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="7fad9-2165">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2165">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="7fad9-2166">Redis</span><span class="sxs-lookup"><span data-stu-id="7fad9-2166">Redis</span></span>

* <span data-ttu-id="7fad9-2167">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="7fad9-2167">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="7fad9-2168">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="7fad9-2168">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="7fad9-2169">Recurso</span><span class="sxs-lookup"><span data-stu-id="7fad9-2169">Resource</span></span>

* <span data-ttu-id="7fad9-2170">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2170">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="7fad9-2171">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2171">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="7fad9-2172">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2172">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="7fad9-2173">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="7fad9-2173">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="7fad9-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="7fad9-2175">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="7fad9-2175">Add docs for az lock update.</span></span> <span data-ttu-id="7fad9-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="7fad9-2177">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="7fad9-2177">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="7fad9-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="7fad9-2179">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="7fad9-2179">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="7fad9-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="7fad9-2181">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2181">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="7fad9-2182">Rol</span><span class="sxs-lookup"><span data-stu-id="7fad9-2182">Role</span></span>

* <span data-ttu-id="7fad9-2183">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2183">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="7fad9-2184">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2184">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="7fad9-2185">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2185">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="7fad9-2186">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="7fad9-2186">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="7fad9-2187">SQL</span><span class="sxs-lookup"><span data-stu-id="7fad9-2187">SQL</span></span>

* <span data-ttu-id="7fad9-2188">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="7fad9-2188">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="7fad9-2189">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2189">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="7fad9-2190">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-2190">Storage</span></span>

* <span data-ttu-id="7fad9-2191">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2191">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="7fad9-2192">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="7fad9-2192">Add support for incremental blob copy</span></span>
* <span data-ttu-id="7fad9-2193">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="7fad9-2193">Add support for large block blob upload</span></span>
* <span data-ttu-id="7fad9-2194">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="7fad9-2194">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-2195">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-2195">VM</span></span>

* <span data-ttu-id="7fad9-2196">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="7fad9-2196">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="7fad9-2197">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="7fad9-2197">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="7fad9-2198">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="7fad9-2198">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="7fad9-2199">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="7fad9-2199">az vm/vmss disk</span></span>
  3. <span data-ttu-id="7fad9-2200">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="7fad9-2200">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="7fad9-2201">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="7fad9-2201">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="7fad9-2202">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2202">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="7fad9-2203">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-2203">April 3, 2017</span></span>

<span data-ttu-id="7fad9-2204">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="7fad9-2204">Version 2.0.2</span></span>

<span data-ttu-id="7fad9-2205">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="7fad9-2205">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="7fad9-2206">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7fad9-2206">Core</span></span>

* <span data-ttu-id="7fad9-2207">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="7fad9-2207">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="7fad9-2208">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2208">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="7fad9-2209">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2209">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="7fad9-2210">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2210">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7fad9-2211">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2211">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="7fad9-2212">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2212">Add prompting for missing template parameters.</span></span> <span data-ttu-id="7fad9-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="7fad9-2214">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="7fad9-2214">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="7fad9-2215">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="7fad9-2215">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="7fad9-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="7fad9-2216">ACS</span></span>

* <span data-ttu-id="7fad9-2217">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2217">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="7fad9-2218">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2218">Add support for ssh key password prompting.</span></span> <span data-ttu-id="7fad9-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="7fad9-2220">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2220">Add support for windows clusters.</span></span> <span data-ttu-id="7fad9-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="7fad9-2222">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="7fad9-2222">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="7fad9-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="7fad9-2224">AppService</span><span class="sxs-lookup"><span data-stu-id="7fad9-2224">AppService</span></span>

* <span data-ttu-id="7fad9-2225">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2225">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="7fad9-2226">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2226">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="7fad9-2227">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2227">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="7fad9-2228">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2228">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="7fad9-2229">DataLake</span><span class="sxs-lookup"><span data-stu-id="7fad9-2229">DataLake</span></span>

* <span data-ttu-id="7fad9-2230">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7fad9-2230">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="7fad9-2231">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7fad9-2231">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="7fad9-2232">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="7fad9-2232">DocuemntDB</span></span>

* <span data-ttu-id="7fad9-2233">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2233">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="7fad9-2234">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7fad9-2234">VM</span></span>

* <span data-ttu-id="7fad9-2235">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2235">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="7fad9-2236">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2236">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="7fad9-2237">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2237">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="7fad9-2238">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2238">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7fad9-2239">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2239">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="7fad9-2240">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2240">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="7fad9-2241">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="7fad9-2241">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="7fad9-2242">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="7fad9-2242">February 27, 2017</span></span>

<span data-ttu-id="7fad9-2243">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7fad9-2243">Version 2.0.0</span></span>

<span data-ttu-id="7fad9-2244">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="7fad9-2244">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="7fad9-2245">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="7fad9-2245">Container Service (acs)</span></span>
- <span data-ttu-id="7fad9-2246">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="7fad9-2246">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="7fad9-2247">Redes</span><span class="sxs-lookup"><span data-stu-id="7fad9-2247">Networking</span></span>
- <span data-ttu-id="7fad9-2248">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="7fad9-2248">Storage</span></span>

<span data-ttu-id="7fad9-2249">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2249">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="7fad9-2250">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="7fad9-2250">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="7fad9-2251">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="7fad9-2251">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="7fad9-2252">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="7fad9-2252">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="7fad9-2253">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="7fad9-2253">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="7fad9-2254">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="7fad9-2254">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="7fad9-2255">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="7fad9-2255">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="7fad9-2256">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="7fad9-2256">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="7fad9-2257">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7fad9-2257">Provide feedback from the command line with the `az feedback` command</span></span>

