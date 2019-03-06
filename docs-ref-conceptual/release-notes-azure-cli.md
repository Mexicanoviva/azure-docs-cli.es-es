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
ms.openlocfilehash: 9f35084eeecab491e5be63eb856b0bb64a6157d0
ms.sourcegitcommit: 9fb008f2802ca6a58f33e01263bf55a80d01f031
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/27/2019
ms.locfileid: "56891218"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="0c3bf-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="0c3bf-103">Azure CLI release notes</span></span>
## <a name="february-26-2019"></a><span data-ttu-id="0c3bf-104">26 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="0c3bf-104">February 26, 2019</span></span>

<span data-ttu-id="0c3bf-105">Versión 2.0.59</span><span class="sxs-lookup"><span data-stu-id="0c3bf-105">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-106">Core</span></span>

* <span data-ttu-id="0c3bf-107">Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-107">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-108">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-108">ACR</span></span>

* <span data-ttu-id="0c3bf-109">Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-109">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="0c3bf-110">Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-110">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-111">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-111">ACS</span></span>

* <span data-ttu-id="0c3bf-112">Se agregó la opción `--listen-address` a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-112">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-113">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-113">AppService</span></span>

* <span data-ttu-id="0c3bf-114">Se agregó el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-114">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-115">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-115">Batch</span></span>
* <span data-ttu-id="0c3bf-116">[CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-116">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="0c3bf-117">[CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-117">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="0c3bf-118">Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-118">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="0c3bf-119">[CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-119">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="0c3bf-120">Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-120">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="0c3bf-121">Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-121">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-122">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-122">CosmosDB</span></span>

* <span data-ttu-id="0c3bf-123">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-123">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="0c3bf-124">Kusto</span><span class="sxs-lookup"><span data-stu-id="0c3bf-124">Kusto</span></span>

* <span data-ttu-id="0c3bf-125">[CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-125">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-126">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-126">Network</span></span>

* <span data-ttu-id="0c3bf-127">Se agregó el argumento `--express-route-gateway-bypass` a `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-127">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="0c3bf-128">Se han agregado grupos de comandos desde extensiones `express-route`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-128">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="0c3bf-129">Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-129">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="0c3bf-130">Se agregó el argumento `--legacy-mode` a `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-130">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="0c3bf-131">Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-131">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="0c3bf-132">Se agregó el argumento `--gateway-default-site` a `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-132">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="0c3bf-133">Se han agregado comandos `ipsec-policy` a `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-133">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-134">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-134">Resource</span></span>

* <span data-ttu-id="0c3bf-135">Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-135">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="0c3bf-136">Se ha agregado compatibilidad para el archivo de parámetros basado en URI a `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-136">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="0c3bf-137">Se ha agregado compatibilidad para definiciones y parámetros basados en URI para `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-137">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="0c3bf-138">Se ha corregido el control de parámetros y reglas para `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-138">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="0c3bf-139">Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-139">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-140">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-140">Role</span></span>

* <span data-ttu-id="0c3bf-141">Se ha agregado compatibilidad con roles de aplicación a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-141">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-142">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-142">VM</span></span>

* <span data-ttu-id="0c3bf-143">Se ha corregido un problema con `vm create where `--acelerated-networking\` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-143">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="0c3bf-144">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="0c3bf-144">February 12, 2019</span></span>

<span data-ttu-id="0c3bf-145">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="0c3bf-145">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-146">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-146">Core</span></span>

* <span data-ttu-id="0c3bf-147">`az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-147">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="0c3bf-148">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-148">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-149">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-149">ACR</span></span>
* <span data-ttu-id="0c3bf-150">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-150">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="0c3bf-151">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-151">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-152">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-152">ACS</span></span>
* <span data-ttu-id="0c3bf-153">Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-153">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="0c3bf-154">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-154">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="0c3bf-155">Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-155">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="0c3bf-156">AMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-156">AMS</span></span>
* <span data-ttu-id="0c3bf-157">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-157">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="0c3bf-158">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-158">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-159">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-159">Appservice</span></span>
* <span data-ttu-id="0c3bf-160">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-160">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="0c3bf-161">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-161">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="0c3bf-162">Se ha mejorado la ayuda de `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-162">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="0c3bf-163">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-163">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="0c3bf-164">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-164">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="0c3bf-165">Botservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-165">Botservice</span></span>
* <span data-ttu-id="0c3bf-166">Se ha mejorado la experiencia de usuario de `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-166">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="0c3bf-167">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-167">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="0c3bf-168">Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-168">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="0c3bf-169">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-169">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="0c3bf-170">[EN DESUSO] Se ha dejado de usar el argumento `--proj-name` en favor de `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-170">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="0c3bf-171">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-171">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="0c3bf-172">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-172">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="0c3bf-173">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-173">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="0c3bf-174">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-174">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="0c3bf-175">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-175">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="0c3bf-176">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-176">Key Vault</span></span>
* <span data-ttu-id="0c3bf-177">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-177">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-178">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-178">Monitor</span></span>
* <span data-ttu-id="0c3bf-179">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-179">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-180">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-180">Network</span></span>
* <span data-ttu-id="0c3bf-181">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-181">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="0c3bf-182">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-182">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="0c3bf-183">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-183">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="0c3bf-184">Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-184">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0c3bf-185">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="0c3bf-185">Policy Insights</span></span>
* <span data-ttu-id="0c3bf-186">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-186">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-187">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-187">RDBMS</span></span>
* <span data-ttu-id="0c3bf-188">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-188">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="0c3bf-189">Redis</span><span class="sxs-lookup"><span data-stu-id="0c3bf-189">Redis</span></span>
* <span data-ttu-id="0c3bf-190">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-190">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="0c3bf-191">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-191">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="0c3bf-192">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-192">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="0c3bf-193">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="0c3bf-193">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="0c3bf-194">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-194">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="0c3bf-195">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="0c3bf-195">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="0c3bf-196">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-196">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-197">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-197">Role</span></span>
* <span data-ttu-id="0c3bf-198">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-198">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="0c3bf-199">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-199">SQL VM</span></span>
* <span data-ttu-id="0c3bf-200">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-200">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-201">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-201">VM</span></span>
* <span data-ttu-id="0c3bf-202">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-202">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="0c3bf-203">Se agregó `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-203">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="0c3bf-204">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-204">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="0c3bf-205">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-205">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="0c3bf-206">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="0c3bf-206">January 31, 2019</span></span>

<span data-ttu-id="0c3bf-207">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="0c3bf-207">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-208">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-208">Core</span></span>

* <span data-ttu-id="0c3bf-209">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-209">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="0c3bf-210">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="0c3bf-210">January 28, 2019</span></span>

<span data-ttu-id="0c3bf-211">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="0c3bf-211">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-212">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-212">ACR</span></span>
* <span data-ttu-id="0c3bf-213">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-213">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-214">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-214">ACS</span></span>
* <span data-ttu-id="0c3bf-215">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-215">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0c3bf-216">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-216">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="0c3bf-217">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-217">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="0c3bf-218">AMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-218">AMS</span></span>
* <span data-ttu-id="0c3bf-219">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-219">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="0c3bf-220">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-220">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-221">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-221">Appservice</span></span>
* <span data-ttu-id="0c3bf-222">Se ha agregado compatibilidad para App Insights en `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-222">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="0c3bf-223">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-223">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="0c3bf-224">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-224">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-225">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-225">Container</span></span>
* <span data-ttu-id="0c3bf-226">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-226">Added `container start` command</span></span>
* <span data-ttu-id="0c3bf-227">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-227">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0c3bf-228">EventGrid</span><span class="sxs-lookup"><span data-stu-id="0c3bf-228">EventGrid</span></span>
* <span data-ttu-id="0c3bf-229">Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-229">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="0c3bf-230">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="0c3bf-230">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="0c3bf-231">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-231">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="0c3bf-232">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-232">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="0c3bf-233">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-233">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0c3bf-234">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0c3bf-234">HDInsight</span></span>
* <span data-ttu-id="0c3bf-235">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-235">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="0c3bf-236">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-236">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="0c3bf-237">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-237">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="0c3bf-238">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-238">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="0c3bf-239">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-239">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="0c3bf-240">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-240">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-241">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-241">IoT</span></span>
* <span data-ttu-id="0c3bf-242">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-242">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="0c3bf-243">Kusto</span><span class="sxs-lookup"><span data-stu-id="0c3bf-243">Kusto</span></span>
* <span data-ttu-id="0c3bf-244">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-244">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-245">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-245">Monitor</span></span>
* <span data-ttu-id="0c3bf-246">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-246">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-247">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-247">Profile</span></span>
* <span data-ttu-id="0c3bf-248">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-248">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-249">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-249">Network</span></span>
* <span data-ttu-id="0c3bf-250">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-250">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="0c3bf-251">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-251">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-252">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-252">Resource</span></span>
* <span data-ttu-id="0c3bf-253">Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-253">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="0c3bf-254">Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-254">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="0c3bf-255">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-255">SQL Virtual Machine</span></span>
* <span data-ttu-id="0c3bf-256">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-256">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-257">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-257">Storage</span></span>
* <span data-ttu-id="0c3bf-258">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-258">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="0c3bf-259">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-259">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-260">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-260">VM</span></span>
* <span data-ttu-id="0c3bf-261">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-261">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="0c3bf-262">Se ha agregado la marca `--force` a `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-262">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="0c3bf-263">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="0c3bf-263">January 15, 2019</span></span>

<span data-ttu-id="0c3bf-264">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="0c3bf-264">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-265">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-265">ACR</span></span>
* <span data-ttu-id="0c3bf-266">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-266">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="0c3bf-267">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-267">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="0c3bf-268">[EN DESUSO] El parámetro `--resource-group` está en desuso en los comandos:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-268">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="0c3bf-269">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-269">ACS</span></span>
* <span data-ttu-id="0c3bf-270">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-270">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-271">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-271">Appservice</span></span>
* <span data-ttu-id="0c3bf-272">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-272">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="0c3bf-273">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-273">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="0c3bf-274">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-274">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="0c3bf-275">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-275">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="0c3bf-276">Botservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-276">Botservice</span></span>
* <span data-ttu-id="0c3bf-277">Se han agregado actualizaciones al estado de implementación a `bot create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-277">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="0c3bf-278">Configuración</span><span class="sxs-lookup"><span data-stu-id="0c3bf-278">Configure</span></span>
* <span data-ttu-id="0c3bf-279">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-279">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-280">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-280">CosmosDB</span></span>
* <span data-ttu-id="0c3bf-281">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-281">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0c3bf-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0c3bf-282">HDInsight</span></span>
* <span data-ttu-id="0c3bf-283">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-283">Added commands for managing applications</span></span>
* <span data-ttu-id="0c3bf-284">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-284">Added commands for managing script actions</span></span>
* <span data-ttu-id="0c3bf-285">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-285">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="0c3bf-286">Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-286">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="0c3bf-287">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-287">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-288">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-288">Network</span></span>
* <span data-ttu-id="0c3bf-289">Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-289">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="0c3bf-290">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-290">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="0c3bf-291">Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-291">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="0c3bf-292">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-292">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-293">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-293">Role</span></span>
* <span data-ttu-id="0c3bf-294">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-294">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="0c3bf-295">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-295">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="0c3bf-296">Seguridad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-296">Security</span></span>
* <span data-ttu-id="0c3bf-297">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="0c3bf-297">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-298">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-298">Storage</span></span>
* <span data-ttu-id="0c3bf-299">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-299">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="0c3bf-300">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-300">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="0c3bf-301">Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-301">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="0c3bf-302">Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-302">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="0c3bf-303">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-303">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-304">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-304">VM</span></span>
* <span data-ttu-id="0c3bf-305">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-305">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="0c3bf-306">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-306">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0c3bf-307">Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-307">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="0c3bf-308">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-308">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="0c3bf-309">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-309">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="0c3bf-310">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-310">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="0c3bf-311">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-311">December 20, 2018</span></span>

<span data-ttu-id="0c3bf-312">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="0c3bf-312">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="0c3bf-313">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-313">Appservice</span></span>
* <span data-ttu-id="0c3bf-314">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-314">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="0c3bf-315">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-315">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="0c3bf-316">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-316">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0c3bf-317">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="0c3bf-317">IoTCentral</span></span>
* <span data-ttu-id="0c3bf-318">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="0c3bf-318">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-319">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-319">Role</span></span>
* <span data-ttu-id="0c3bf-320">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-320">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-321">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-321">SQL</span></span>
* <span data-ttu-id="0c3bf-322">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-322">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-323">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-323">VM</span></span>
* <span data-ttu-id="0c3bf-324">Se ha agregado el parámetro `---os-type` a `disk create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-324">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="0c3bf-325">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-325">December 18, 2018</span></span>

<span data-ttu-id="0c3bf-326">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="0c3bf-326">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="0c3bf-327">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-327">ACR</span></span>
* <span data-ttu-id="0c3bf-328">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-328">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="0c3bf-329">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-329">Condensed the table layout for task list</span></span>
* <span data-ttu-id="0c3bf-330">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-330">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-331">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-331">ACS</span></span>
* <span data-ttu-id="0c3bf-332">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-332">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0c3bf-333">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-333">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="0c3bf-334">[EN DESUSO] Se han dejado de utilizar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-334">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="0c3bf-335">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-335">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="0c3bf-336">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-336">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="0c3bf-337">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-337">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-338">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-338">Appservice</span></span>
* <span data-ttu-id="0c3bf-339">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-339">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="0c3bf-340">Botservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-340">Botservice</span></span>
* <span data-ttu-id="0c3bf-341">Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-341">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="0c3bf-342">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-342">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="0c3bf-343">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-343">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="0c3bf-344">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-344">Reduced Kudu network calls</span></span>
* <span data-ttu-id="0c3bf-345">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-345">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="0c3bf-346">Consumo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-346">Consumption</span></span>
* <span data-ttu-id="0c3bf-347">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-347">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-348">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-348">CosmosDB</span></span>
* <span data-ttu-id="0c3bf-349">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-349">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="0c3bf-350">Mapas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-350">Maps</span></span>
* <span data-ttu-id="0c3bf-351">Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-351">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-352">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-352">Network</span></span>
* <span data-ttu-id="0c3bf-353">Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-353">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="0c3bf-354">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-354">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-355">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-355">Resource</span></span>
* <span data-ttu-id="0c3bf-356">Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-356">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="0c3bf-357">Se ha agregado un nuevo comando `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-357">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-358">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-358">Storage</span></span>
*  <span data-ttu-id="0c3bf-359">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-359">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-360">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-360">VM</span></span>
* <span data-ttu-id="0c3bf-361">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-361">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="0c3bf-362">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-362">December 4, 2018</span></span>

<span data-ttu-id="0c3bf-363">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="0c3bf-363">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="0c3bf-364">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-364">Core</span></span>
* <span data-ttu-id="0c3bf-365">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="0c3bf-365">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="0c3bf-366">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-366">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-367">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-367">Appservice</span></span>
* <span data-ttu-id="0c3bf-368">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-368">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="0c3bf-369">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="0c3bf-369">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-370">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-370">Network</span></span>
* <span data-ttu-id="0c3bf-371">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="0c3bf-371">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-372">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-372">Role</span></span>
* <span data-ttu-id="0c3bf-373">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="0c3bf-373">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="0c3bf-374">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-374">VM</span></span>
* <span data-ttu-id="0c3bf-375">[EN DESUSO] El parámetro `vm extension [show|wait] --expand` está en desuso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-375">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="0c3bf-376">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="0c3bf-376">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="0c3bf-377">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="0c3bf-377">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="0c3bf-378">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="0c3bf-378">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="0c3bf-379">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-379">November 20, 2018</span></span>

<span data-ttu-id="0c3bf-380">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="0c3bf-380">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="0c3bf-381">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-381">Core</span></span>
* <span data-ttu-id="0c3bf-382">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-382">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-383">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-383">ACR</span></span>
* <span data-ttu-id="0c3bf-384">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-384">Added context token to task step</span></span>
* <span data-ttu-id="0c3bf-385">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-385">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="0c3bf-386">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-386">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-387">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-387">Appservice</span></span>
* <span data-ttu-id="0c3bf-388">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-388">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="0c3bf-389">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-389">Updated the default `node_version`.</span></span> <span data-ttu-id="0c3bf-390">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-390">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="0c3bf-391">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-391">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="0c3bf-392">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-392">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0c3bf-393">IotCentral</span><span class="sxs-lookup"><span data-stu-id="0c3bf-393">IotCentral</span></span>
* <span data-ttu-id="0c3bf-394">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="0c3bf-394">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-395">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-395">KeyVault</span></span>
* <span data-ttu-id="0c3bf-396">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-396">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-397">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-397">Network</span></span>
* <span data-ttu-id="0c3bf-398">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-398">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="0c3bf-399">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-399">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="0c3bf-400">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-400">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="0c3bf-401">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-401">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-402">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0c3bf-402">Rdbms</span></span>
* <span data-ttu-id="0c3bf-403">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-403">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="0c3bf-404">Rbac</span><span class="sxs-lookup"><span data-stu-id="0c3bf-404">Rbac</span></span>
* <span data-ttu-id="0c3bf-405">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-405">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="0c3bf-406">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-406">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="0c3bf-407">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-407">Storage</span></span>
* <span data-ttu-id="0c3bf-408">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-408">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="0c3bf-409">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-409">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="0c3bf-410">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-410">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="0c3bf-411">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-411">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-412">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-412">VM</span></span>
* <span data-ttu-id="0c3bf-413">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-413">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="0c3bf-414">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-414">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="0c3bf-415">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-415">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="0c3bf-416">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-416">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="0c3bf-417">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-417">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="0c3bf-418">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-418">Added `snapshot wait` command</span></span>
* <span data-ttu-id="0c3bf-419">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-419">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="0c3bf-420">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-420">November 6, 2018</span></span>

<span data-ttu-id="0c3bf-421">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="0c3bf-421">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-422">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-422">Core</span></span>
* <span data-ttu-id="0c3bf-423">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-423">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-424">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-424">ACR</span></span>
* <span data-ttu-id="0c3bf-425">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="0c3bf-425">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="0c3bf-426">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="0c3bf-426">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-427">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-427">ACS</span></span>
* <span data-ttu-id="0c3bf-428">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-428">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="0c3bf-429">Advisor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-429">Advisor</span></span>
* <span data-ttu-id="0c3bf-430">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="0c3bf-430">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="0c3bf-431">AMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-431">AMS</span></span>
* <span data-ttu-id="0c3bf-432">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-432">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="0c3bf-433">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-433">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="0c3bf-434">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-434">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="0c3bf-435">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-435">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="0c3bf-436">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-436">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="0c3bf-437">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-437">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="0c3bf-438">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-438">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="0c3bf-439">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-439">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="0c3bf-440">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-440">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="0c3bf-441">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-441">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="0c3bf-442">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-442">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="0c3bf-443">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-443">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="0c3bf-444">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-444">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="0c3bf-445">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-445">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="0c3bf-446">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-446">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="0c3bf-447">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="0c3bf-447">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="0c3bf-448">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="0c3bf-448">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-449">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-449">AppService</span></span>
* <span data-ttu-id="0c3bf-450">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="0c3bf-450">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="0c3bf-451">Configuración</span><span class="sxs-lookup"><span data-stu-id="0c3bf-451">Configure</span></span>
* <span data-ttu-id="0c3bf-452">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="0c3bf-452">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-453">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-453">Container</span></span>
* <span data-ttu-id="0c3bf-454">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="0c3bf-454">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="0c3bf-455">EventHub</span><span class="sxs-lookup"><span data-stu-id="0c3bf-455">EventHub</span></span>
* <span data-ttu-id="0c3bf-456">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-456">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-457">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-457">Interactive</span></span>
* <span data-ttu-id="0c3bf-458">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="0c3bf-458">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-459">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-459">Monitor</span></span>
* <span data-ttu-id="0c3bf-460">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-460">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-461">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-461">Network</span></span>
* <span data-ttu-id="0c3bf-462">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-462">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="0c3bf-463">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="0c3bf-463">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="0c3bf-464">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-464">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="0c3bf-465">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-465">Profile</span></span>
* <span data-ttu-id="0c3bf-466">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-466">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-467">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-467">RDBMS</span></span>
* <span data-ttu-id="0c3bf-468">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="0c3bf-468">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-469">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-469">Resource</span></span>
* <span data-ttu-id="0c3bf-470">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-470">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-471">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-471">Role</span></span>
* <span data-ttu-id="0c3bf-472">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-472">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="0c3bf-473">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-473">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="0c3bf-474">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="0c3bf-474">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-475">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-475">Storage</span></span>
* <span data-ttu-id="0c3bf-476">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-476">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-477">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-477">VM</span></span>
* <span data-ttu-id="0c3bf-478">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="0c3bf-478">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="0c3bf-479">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="0c3bf-479">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="0c3bf-480">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-480">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="0c3bf-481">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-481">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="0c3bf-482">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-482">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="0c3bf-483">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-483">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="0c3bf-484">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-484">October 23, 2018</span></span>

<span data-ttu-id="0c3bf-485">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="0c3bf-485">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-486">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-486">Core</span></span>
* <span data-ttu-id="0c3bf-487">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-487">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="0c3bf-488">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-488">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-489">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-489">ACR</span></span>
* <span data-ttu-id="0c3bf-490">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="0c3bf-490">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="0c3bf-491">CDN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-491">CDN</span></span>
* <span data-ttu-id="0c3bf-492">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="0c3bf-492">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="0c3bf-493">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-493">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-494">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-494">Container</span></span>
* <span data-ttu-id="0c3bf-495">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-495">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="0c3bf-496">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-496">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="0c3bf-497">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-497">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="0c3bf-498">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-498">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="0c3bf-499">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="0c3bf-499">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="0c3bf-500">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-500">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="0c3bf-501">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-501">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-502">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-502">CosmosDB</span></span>
* <span data-ttu-id="0c3bf-503">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-503">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-504">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-504">Interactive</span></span>
* <span data-ttu-id="0c3bf-505">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="0c3bf-505">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="0c3bf-506">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0c3bf-506">IoT Central</span></span>
* <span data-ttu-id="0c3bf-507">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="0c3bf-507">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="0c3bf-508">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="0c3bf-508">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-509">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-509">Monitor</span></span>
* <span data-ttu-id="0c3bf-510">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-510">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="0c3bf-511">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="0c3bf-511">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="0c3bf-512">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-512">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0c3bf-513">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-513">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="0c3bf-514">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-514">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="0c3bf-515">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-515">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="0c3bf-516">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-516">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="0c3bf-517">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-517">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0c3bf-518">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-518">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="0c3bf-519">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-519">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-520">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-520">Network</span></span>
* <span data-ttu-id="0c3bf-521">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="0c3bf-521">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="0c3bf-522">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="0c3bf-522">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="0c3bf-523">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0c3bf-523">ServiceBus</span></span>
* <span data-ttu-id="0c3bf-524">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="0c3bf-524">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-525">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-525">SQL</span></span>
* <span data-ttu-id="0c3bf-526">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-526">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-527">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-527">Storage</span></span>
* <span data-ttu-id="0c3bf-528">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="0c3bf-528">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="0c3bf-529">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-529">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-530">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-530">VM</span></span>
* <span data-ttu-id="0c3bf-531">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-531">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="0c3bf-532">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-532">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="0c3bf-533">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-533">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="0c3bf-534">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-534">October 16, 2018</span></span>

<span data-ttu-id="0c3bf-535">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="0c3bf-535">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-536">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-536">VM</span></span>
* <span data-ttu-id="0c3bf-537">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="0c3bf-537">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="0c3bf-538">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-538">October 9, 2018</span></span>

<span data-ttu-id="0c3bf-539">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="0c3bf-539">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-540">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-540">Core</span></span>
* <span data-ttu-id="0c3bf-541">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-541">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-542">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-542">ACR</span></span>
* <span data-ttu-id="0c3bf-543">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="0c3bf-543">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-544">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-544">ACS</span></span>
* <span data-ttu-id="0c3bf-545">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="0c3bf-545">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="0c3bf-546">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="0c3bf-546">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="0c3bf-547">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="0c3bf-547">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="0c3bf-548">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-548">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-549">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-549">Container</span></span>
* <span data-ttu-id="0c3bf-550">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="0c3bf-550">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="0c3bf-551">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="0c3bf-551">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="0c3bf-552">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-552">Event Hub</span></span>
* <span data-ttu-id="0c3bf-553">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-553">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="0c3bf-554">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="0c3bf-554">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="0c3bf-555">Extensiones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-555">Extensions</span></span>
* <span data-ttu-id="0c3bf-556">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-556">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0c3bf-557">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0c3bf-557">HDInsight</span></span>
* <span data-ttu-id="0c3bf-558">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-558">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-559">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-559">IoT</span></span>
* <span data-ttu-id="0c3bf-560">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="0c3bf-560">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-561">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-561">KeyVault</span></span>
* <span data-ttu-id="0c3bf-562">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-562">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-563">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-563">Network</span></span>
* <span data-ttu-id="0c3bf-564">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-564">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="0c3bf-565">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="0c3bf-565">See #6052</span></span>
* <span data-ttu-id="0c3bf-566">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-566">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="0c3bf-567">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="0c3bf-567">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="0c3bf-568">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-568">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="0c3bf-569">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-569">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="0c3bf-570">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-570">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="0c3bf-571">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-571">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-572">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-572">Role</span></span>
* <span data-ttu-id="0c3bf-573">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-573">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="0c3bf-574">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-574">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="0c3bf-575">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-575">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="0c3bf-576">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-576">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="0c3bf-577">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="0c3bf-577">Service Bus</span></span>
* <span data-ttu-id="0c3bf-578">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="0c3bf-578">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-579">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-579">VM</span></span>
* <span data-ttu-id="0c3bf-580">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-580">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="0c3bf-581">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-581">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="0c3bf-582">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-582">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="0c3bf-583">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-583">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="0c3bf-584">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-584">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="0c3bf-585">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="0c3bf-585">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="0c3bf-586">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-586">September 21, 2018</span></span>

<span data-ttu-id="0c3bf-587">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="0c3bf-587">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-588">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-588">ACR</span></span>
* <span data-ttu-id="0c3bf-589">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-589">Added ACR Task commands</span></span>
* <span data-ttu-id="0c3bf-590">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="0c3bf-590">Added quick run command</span></span>
* <span data-ttu-id="0c3bf-591">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-591">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="0c3bf-592">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-592">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="0c3bf-593">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-593">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="0c3bf-594">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-594">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-595">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-595">ACS</span></span>
* <span data-ttu-id="0c3bf-596">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-596">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="0c3bf-597">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="0c3bf-597">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-598">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-598">AppService</span></span>

* <span data-ttu-id="0c3bf-599">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-599">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="0c3bf-600">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="0c3bf-600">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="0c3bf-601">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="0c3bf-601">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="0c3bf-602">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-602">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-603">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-603">Batch</span></span>
* <span data-ttu-id="0c3bf-604">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="0c3bf-604">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="0c3bf-605">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-605">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="0c3bf-606">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-606">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="0c3bf-607">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="0c3bf-607">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0c3bf-608">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-608">Batch AI</span></span> 
* <span data-ttu-id="0c3bf-609">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-609">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0c3bf-610">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0c3bf-610">Cognitive Services</span></span>
* <span data-ttu-id="0c3bf-611">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-611">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="0c3bf-612">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-612">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="0c3bf-613">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-613">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="0c3bf-614">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-614">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="0c3bf-615">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-615">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="0c3bf-616">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-616">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-617">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-617">Container</span></span>
* <span data-ttu-id="0c3bf-618">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="0c3bf-618">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="0c3bf-619">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-619">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="0c3bf-620">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-620">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="0c3bf-621">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-621">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="0c3bf-622">DataLake</span><span class="sxs-lookup"><span data-stu-id="0c3bf-622">Datalake</span></span>
* <span data-ttu-id="0c3bf-623">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-623">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="0c3bf-624">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-624">Interactive Shell</span></span>
* <span data-ttu-id="0c3bf-625">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-625">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="0c3bf-626">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-626">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-627">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-627">IoT</span></span>
* <span data-ttu-id="0c3bf-628">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-628">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="0c3bf-629">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-629">Key Vault</span></span>
* <span data-ttu-id="0c3bf-630">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="0c3bf-630">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-631">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-631">Network</span></span>
* <span data-ttu-id="0c3bf-632">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-632">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="0c3bf-633">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-633">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="0c3bf-634">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="0c3bf-634">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="0c3bf-635">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-635">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="0c3bf-636">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-636">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="0c3bf-637">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-637">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="0c3bf-638">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-638">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="0c3bf-639">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-639">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="0c3bf-640">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-640">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="0c3bf-641">`network express-route create/update`: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-641">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="0c3bf-642">`network vnet subnet create/update`: Se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-642">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="0c3bf-643">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-643">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="0c3bf-644">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-644">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="0c3bf-645">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-645">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="0c3bf-646">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-646">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="0c3bf-647">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="0c3bf-647">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="0c3bf-648">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-648">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="0c3bf-649">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="0c3bf-649">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-650">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-650">RDBMS</span></span>
* <span data-ttu-id="0c3bf-651">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-651">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="0c3bf-652">Reserva</span><span class="sxs-lookup"><span data-stu-id="0c3bf-652">Reservation</span></span>
* <span data-ttu-id="0c3bf-653">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-653">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="0c3bf-654">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-654">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="0c3bf-655">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-655">Manage App</span></span>
* <span data-ttu-id="0c3bf-656">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-656">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="0c3bf-657">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-657">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-658">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-658">Role</span></span>
* <span data-ttu-id="0c3bf-659">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="0c3bf-659">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="0c3bf-660">SignalR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-660">SignalR</span></span>
* <span data-ttu-id="0c3bf-661">Primera versión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-661">First release</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-662">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-662">Storage</span></span>
* <span data-ttu-id="0c3bf-663">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-663">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="0c3bf-664">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="0c3bf-664">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-665">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-665">VM</span></span>
* <span data-ttu-id="0c3bf-666">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-666">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="0c3bf-667">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-667">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="0c3bf-668">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-668">August 28, 2018</span></span>

<span data-ttu-id="0c3bf-669">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="0c3bf-669">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-670">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-670">Core</span></span>

* <span data-ttu-id="0c3bf-671">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="0c3bf-671">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="0c3bf-672">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="0c3bf-672">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-673">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-673">ACR</span></span>

* <span data-ttu-id="0c3bf-674">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="0c3bf-674">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="0c3bf-675">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-675">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-676">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-676">ACS</span></span>

* <span data-ttu-id="0c3bf-677">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-677">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="0c3bf-678">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="0c3bf-678">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-679">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-679">AppService</span></span>

* <span data-ttu-id="0c3bf-680">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="0c3bf-680">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="0c3bf-681">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-681">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="0c3bf-682">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-682">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="0c3bf-683">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-683">Backup</span></span>

* <span data-ttu-id="0c3bf-684">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-684">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="0c3bf-685">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="0c3bf-685">Bot Service</span></span>

* <span data-ttu-id="0c3bf-686">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="0c3bf-686">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0c3bf-687">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0c3bf-687">Cognitive Services</span></span>

* <span data-ttu-id="0c3bf-688">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="0c3bf-688">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-689">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-689">IoT</span></span>

* <span data-ttu-id="0c3bf-690">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-690">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-691">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-691">Monitor</span></span>

* <span data-ttu-id="0c3bf-692">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="0c3bf-692">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="0c3bf-693">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-693">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-694">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-694">Network</span></span>

* <span data-ttu-id="0c3bf-695">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-695">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-696">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-696">Resource</span></span>

* <span data-ttu-id="0c3bf-697">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-697">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-698">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-698">Storage</span></span>

* <span data-ttu-id="0c3bf-699">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-699">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-700">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-700">VM</span></span>

* <span data-ttu-id="0c3bf-701">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-701">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="0c3bf-702">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-702">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="0c3bf-703">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-703">Auguest 14, 2018</span></span>

<span data-ttu-id="0c3bf-704">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="0c3bf-704">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-705">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-705">Core</span></span>

* <span data-ttu-id="0c3bf-706">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-706">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="0c3bf-707">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="0c3bf-707">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="0c3bf-708">Telemetría</span><span class="sxs-lookup"><span data-stu-id="0c3bf-708">Telemetry</span></span>

* <span data-ttu-id="0c3bf-709">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="0c3bf-709">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-710">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-710">ACR</span></span>

* <span data-ttu-id="0c3bf-711">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-711">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="0c3bf-712">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-712">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-713">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-713">ACS</span></span>

* <span data-ttu-id="0c3bf-714">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="0c3bf-714">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="0c3bf-715">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-715">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="0c3bf-716">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="0c3bf-716">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="0c3bf-717">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="0c3bf-717">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="0c3bf-718">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="0c3bf-718">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="0c3bf-719">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-719">AppService</span></span>

* <span data-ttu-id="0c3bf-720">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-720">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="0c3bf-721">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="0c3bf-721">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="0c3bf-722">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-722">BatchAI</span></span>

* <span data-ttu-id="0c3bf-723">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="0c3bf-723">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="0c3bf-724">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-724">Container</span></span>

* <span data-ttu-id="0c3bf-725">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-725">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="0c3bf-726">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-726">IoT</span></span>

* <span data-ttu-id="0c3bf-727">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="0c3bf-727">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="0c3bf-728">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-728">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="0c3bf-729">Iot Central</span><span class="sxs-lookup"><span data-stu-id="0c3bf-729">Iot Central</span></span>

* <span data-ttu-id="0c3bf-730">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="0c3bf-730">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-731">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-731">KeyVault</span></span>


* <span data-ttu-id="0c3bf-732">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-732">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="0c3bf-733">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-733">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="0c3bf-734">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="0c3bf-734">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="0c3bf-735">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="0c3bf-735">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="0c3bf-736">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="0c3bf-736">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="0c3bf-737">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-737">Relay</span></span>

* <span data-ttu-id="0c3bf-738">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-738">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-739">Sql</span><span class="sxs-lookup"><span data-stu-id="0c3bf-739">Sql</span></span>

* <span data-ttu-id="0c3bf-740">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-740">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-741">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-741">Storage</span></span>

* <span data-ttu-id="0c3bf-742">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="0c3bf-742">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="0c3bf-743">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-743">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="0c3bf-744">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-744">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="0c3bf-745">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-745">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="0c3bf-746">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-746">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-747">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-747">VM</span></span>

* <span data-ttu-id="0c3bf-748">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-748">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="0c3bf-749">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-749">July 31, 2018</span></span>

<span data-ttu-id="0c3bf-750">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="0c3bf-750">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-751">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-751">ACR</span></span>

* <span data-ttu-id="0c3bf-752">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-752">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="0c3bf-753">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-753">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-754">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-754">ACS</span></span>

* <span data-ttu-id="0c3bf-755">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="0c3bf-755">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-756">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-756">Batch</span></span>

* <span data-ttu-id="0c3bf-757">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-757">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-758">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-758">Container</span></span>

* <span data-ttu-id="0c3bf-759">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-759">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-760">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-760">Network</span></span>

* <span data-ttu-id="0c3bf-761">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-761">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="0c3bf-762">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-762">Resource</span></span>

* <span data-ttu-id="0c3bf-763">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-763">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="0c3bf-764">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-764">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-765">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-765">Role</span></span>

* <span data-ttu-id="0c3bf-766">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-766">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="0c3bf-767">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-767">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="0c3bf-768">Search</span><span class="sxs-lookup"><span data-stu-id="0c3bf-768">Search</span></span>

* <span data-ttu-id="0c3bf-769">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-769">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="0c3bf-770">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="0c3bf-770">Service Bus</span></span>

* <span data-ttu-id="0c3bf-771">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-771">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="0c3bf-772">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-772">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="0c3bf-773">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-773">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="0c3bf-774">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-774">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-775">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-775">Storage</span></span>

* <span data-ttu-id="0c3bf-776">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-776">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="0c3bf-777">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-777">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-778">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-778">VM</span></span>

* <span data-ttu-id="0c3bf-779">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-779">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="0c3bf-780">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-780">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="0c3bf-781">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-781">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="0c3bf-782">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-782">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="0c3bf-783">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-783">July 18, 2018</span></span>

<span data-ttu-id="0c3bf-784">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="0c3bf-784">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-785">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-785">Core</span></span>

* <span data-ttu-id="0c3bf-786">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-786">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="0c3bf-787">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-787">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="0c3bf-788">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-788">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-789">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-789">ACR</span></span>

* <span data-ttu-id="0c3bf-790">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-790">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="0c3bf-791">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-791">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="0c3bf-792">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-792">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="0c3bf-793">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="0c3bf-793">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-794">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-794">ACS</span></span>

* <span data-ttu-id="0c3bf-795">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="0c3bf-795">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-796">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-796">AppService</span></span>

* <span data-ttu-id="0c3bf-797">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="0c3bf-797">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-798">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-798">Batch</span></span>

* <span data-ttu-id="0c3bf-799">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="0c3bf-799">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="0c3bf-800">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-800">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0c3bf-801">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-801">Batch AI</span></span>

* <span data-ttu-id="0c3bf-802">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-802">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-803">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-803">Container</span></span>

* <span data-ttu-id="0c3bf-804">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="0c3bf-804">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="0c3bf-805">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="0c3bf-805">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-806">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-806">Network</span></span>

* <span data-ttu-id="0c3bf-807">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-807">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="0c3bf-808">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-808">Added `network nic wait`</span></span>
* <span data-ttu-id="0c3bf-809">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-809">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="0c3bf-810">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-810">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="0c3bf-811">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-811">Resource</span></span>

* <span data-ttu-id="0c3bf-812">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-812">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="0c3bf-813">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-813">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="0c3bf-814">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-814">Added `deployment wait` command</span></span>
* <span data-ttu-id="0c3bf-815">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="0c3bf-815">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-816">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-816">SQL</span></span>

* <span data-ttu-id="0c3bf-817">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-817">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="0c3bf-818">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-818">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="0c3bf-819">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-819">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-820">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-820">Storage</span></span>

* <span data-ttu-id="0c3bf-821">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-821">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-822">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-822">VM</span></span>

* <span data-ttu-id="0c3bf-823">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-823">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="0c3bf-824">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-824">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="0c3bf-825">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-825">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0c3bf-826">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-826">July 3, 2018</span></span>

<span data-ttu-id="0c3bf-827">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="0c3bf-827">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="0c3bf-828">AKS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-828">AKS</span></span>

* <span data-ttu-id="0c3bf-829">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="0c3bf-829">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0c3bf-830">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-830">July 3, 2018</span></span>

<span data-ttu-id="0c3bf-831">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="0c3bf-831">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-832">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-832">Core</span></span>

* <span data-ttu-id="0c3bf-833">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-833">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-834">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-834">ACR</span></span>

* <span data-ttu-id="0c3bf-835">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-835">Added polling build status</span></span>
* <span data-ttu-id="0c3bf-836">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-836">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="0c3bf-837">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-837">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-838">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-838">ACS</span></span>

* <span data-ttu-id="0c3bf-839">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-839">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="0c3bf-840">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-840">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="0c3bf-841">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-841">Updated options for `aks browse` command.</span></span> <span data-ttu-id="0c3bf-842">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-842">Added `--listen-port` support</span></span>
* <span data-ttu-id="0c3bf-843">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-843">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="0c3bf-844">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="0c3bf-844">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="0c3bf-845">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-845">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-846">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-846">AppService</span></span>

* <span data-ttu-id="0c3bf-847">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-847">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="0c3bf-848">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-848">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="0c3bf-849">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-849">Backup</span></span>

* <span data-ttu-id="0c3bf-850">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-850">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="0c3bf-851">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-851">BatchAI</span></span>

* <span data-ttu-id="0c3bf-852">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-852">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="0c3bf-853">Nube</span><span class="sxs-lookup"><span data-stu-id="0c3bf-853">Cloud</span></span>

* <span data-ttu-id="0c3bf-854">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="0c3bf-854">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-855">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-855">Container</span></span>

* <span data-ttu-id="0c3bf-856">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="0c3bf-856">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="0c3bf-857">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-857">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="0c3bf-858">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-858">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-859">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-859">Extension</span></span>

* <span data-ttu-id="0c3bf-860">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-860">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-861">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-861">Network</span></span>

* <span data-ttu-id="0c3bf-862">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-862">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-863">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0c3bf-863">Rdbms</span></span>

* <span data-ttu-id="0c3bf-864">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-864">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-865">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-865">Resource</span></span>

* <span data-ttu-id="0c3bf-866">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-866">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-867">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-867">VM</span></span>

* <span data-ttu-id="0c3bf-868">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="0c3bf-868">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="0c3bf-869">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-869">June 25, 2018</span></span>

<span data-ttu-id="0c3bf-870">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="0c3bf-870">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="0c3bf-871">CLI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-871">CLI</span></span>

* <span data-ttu-id="0c3bf-872">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-872">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="0c3bf-873">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-873">June 19, 2018</span></span>

<span data-ttu-id="0c3bf-874">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="0c3bf-874">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-875">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-875">Core</span></span>

* <span data-ttu-id="0c3bf-876">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-876">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-877">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-877">ACR</span></span>

* <span data-ttu-id="0c3bf-878">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="0c3bf-878">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="0c3bf-879">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-879">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-880">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-880">ACS</span></span>

* <span data-ttu-id="0c3bf-881">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-881">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="0c3bf-882">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-882">Added `--update` support</span></span>
* <span data-ttu-id="0c3bf-883">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-883">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="0c3bf-884">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-884">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="0c3bf-885">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-885">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="0c3bf-886">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-886">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="0c3bf-887">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-887">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="0c3bf-888">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-888">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-889">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-889">AppService</span></span>

* <span data-ttu-id="0c3bf-890">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="0c3bf-890">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="0c3bf-891">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-891">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-892">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-892">Batch</span></span>

* <span data-ttu-id="0c3bf-893">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-893">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0c3bf-894">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-894">Batch AI</span></span>

* <span data-ttu-id="0c3bf-895">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-895">Added support for workspaces.</span></span> <span data-ttu-id="0c3bf-896">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-896">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="0c3bf-897">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-897">Added support for experiments.</span></span> <span data-ttu-id="0c3bf-898">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-898">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="0c3bf-899">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="0c3bf-899">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="0c3bf-900">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-900">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="0c3bf-901">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-901">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="0c3bf-902">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-902">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="0c3bf-903">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-903">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="0c3bf-904">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-904">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="0c3bf-905">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-905">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="0c3bf-906">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-906">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="0c3bf-907">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-907">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="0c3bf-908">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-908">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="0c3bf-909">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-909">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="0c3bf-910">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-910">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="0c3bf-911">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-911">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="0c3bf-912">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-912">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="0c3bf-913">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="0c3bf-913">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="0c3bf-914">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="0c3bf-914">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0c3bf-915">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="0c3bf-915">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0c3bf-916">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="0c3bf-916">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="0c3bf-917">Mapas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-917">Maps</span></span>

* <span data-ttu-id="0c3bf-918">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-918">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-919">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-919">Network</span></span>

* <span data-ttu-id="0c3bf-920">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-920">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="0c3bf-921">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-921">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="0c3bf-922">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="0c3bf-922">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="0c3bf-923">Reservations</span><span class="sxs-lookup"><span data-stu-id="0c3bf-923">Reservations</span></span>

* <span data-ttu-id="0c3bf-924">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-924">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="0c3bf-925">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-925">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="0c3bf-926">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-926">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="0c3bf-927">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-927">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="0c3bf-928">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-928">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="0c3bf-929">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-929">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-930">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-930">Role</span></span>

* <span data-ttu-id="0c3bf-931">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-931">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-932">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-932">SQL</span></span>

* <span data-ttu-id="0c3bf-933">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="0c3bf-933">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-934">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-934">Storage</span></span>

* <span data-ttu-id="0c3bf-935">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="0c3bf-935">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-936">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-936">VM</span></span>

* <span data-ttu-id="0c3bf-937">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-937">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="0c3bf-938">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-938">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="0c3bf-939">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-939">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0c3bf-940">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-940">June 13, 2018</span></span>

<span data-ttu-id="0c3bf-941">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="0c3bf-941">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-942">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-942">Core</span></span>

* <span data-ttu-id="0c3bf-943">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="0c3bf-943">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0c3bf-944">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-944">June 13, 2018</span></span>

<span data-ttu-id="0c3bf-945">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="0c3bf-945">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="0c3bf-946">AKS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-946">AKS</span></span>

* <span data-ttu-id="0c3bf-947">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-947">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="0c3bf-948">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="0c3bf-948">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="0c3bf-949">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-949">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="0c3bf-950">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-950">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="0c3bf-951">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-951">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-952">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-952">AppService</span></span>

* <span data-ttu-id="0c3bf-953">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="0c3bf-953">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0c3bf-954">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-954">June 5, 2018</span></span>

<span data-ttu-id="0c3bf-955">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="0c3bf-955">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-956">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-956">Interactive</span></span>

* <span data-ttu-id="0c3bf-957">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-957">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0c3bf-958">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-958">June 5, 2018</span></span>

<span data-ttu-id="0c3bf-959">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="0c3bf-959">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-960">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-960">Core</span></span>

* <span data-ttu-id="0c3bf-961">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-961">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="0c3bf-962">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="0c3bf-962">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-963">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-963">ACR</span></span>

* <span data-ttu-id="0c3bf-964">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="0c3bf-964">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="0c3bf-965">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-965">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="0c3bf-966">AKS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-966">AKS</span></span>

* <span data-ttu-id="0c3bf-967">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-967">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-968">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-968">Batch</span></span>

* <span data-ttu-id="0c3bf-969">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="0c3bf-969">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-970">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-970">IOT</span></span>

* <span data-ttu-id="0c3bf-971">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="0c3bf-971">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-972">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-972">Network</span></span>

* <span data-ttu-id="0c3bf-973">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-973">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0c3bf-974">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="0c3bf-974">Policy Insights</span></span>

* <span data-ttu-id="0c3bf-975">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="0c3bf-975">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="0c3bf-976">ARM</span><span class="sxs-lookup"><span data-stu-id="0c3bf-976">ARM</span></span>

* <span data-ttu-id="0c3bf-977">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-977">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-978">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-978">SQL</span></span>

* <span data-ttu-id="0c3bf-979">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-979">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="0c3bf-980">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-980">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="0c3bf-981">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-981">Storage</span></span>

* <span data-ttu-id="0c3bf-982">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-982">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-983">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-983">VM</span></span>

* <span data-ttu-id="0c3bf-984">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-984">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="0c3bf-985">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-985">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="0c3bf-986">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-986">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="0c3bf-987">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-987">May 22, 2018</span></span>

<span data-ttu-id="0c3bf-988">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="0c3bf-988">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-989">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-989">Core</span></span>

* <span data-ttu-id="0c3bf-990">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-990">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-991">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-991">ACS</span></span>

* <span data-ttu-id="0c3bf-992">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-992">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="0c3bf-993">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="0c3bf-993">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-994">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-994">AppService</span></span>

* <span data-ttu-id="0c3bf-995">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-995">Improved generic update commands</span></span>
* <span data-ttu-id="0c3bf-996">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-996">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-997">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-997">Container</span></span>

* <span data-ttu-id="0c3bf-998">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="0c3bf-998">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="0c3bf-999">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-999">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1000">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1000">Extension</span></span>

* <span data-ttu-id="0c3bf-1001">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1001">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1002">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1002">Interactive</span></span>

* <span data-ttu-id="0c3bf-1003">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1003">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="0c3bf-1004">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1004">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-1005">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1005">KeyVault</span></span>

* <span data-ttu-id="0c3bf-1006">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1006">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1007">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1007">Network</span></span>

* <span data-ttu-id="0c3bf-1008">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1008">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="0c3bf-1009">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1009">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1010">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1010">SQL</span></span>

* <span data-ttu-id="0c3bf-1011">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1011">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="0c3bf-1012">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1012">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="0c3bf-1013">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1013">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="0c3bf-1014">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1014">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="0c3bf-1015">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1015">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="0c3bf-1016">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1016">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="0c3bf-1017">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1017">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="0c3bf-1018">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1018">`edition`.</span></span> <span data-ttu-id="0c3bf-1019">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1019">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="0c3bf-1020">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1020">`elasticPoolName`.</span></span> <span data-ttu-id="0c3bf-1021">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1021">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="0c3bf-1022">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1022">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="0c3bf-1023">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1023">`edition`.</span></span> <span data-ttu-id="0c3bf-1024">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1024">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="0c3bf-1025">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1025">`dtu`.</span></span> <span data-ttu-id="0c3bf-1026">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1026">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="0c3bf-1027">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1027">`databaseDtuMin`.</span></span> <span data-ttu-id="0c3bf-1028">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1028">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="0c3bf-1029">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1029">`databaseDtuMax`.</span></span> <span data-ttu-id="0c3bf-1030">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1030">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="0c3bf-1031">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1031">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="0c3bf-1032">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1032">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1033">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1033">Storage</span></span>

* <span data-ttu-id="0c3bf-1034">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1034">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="0c3bf-1035">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1035">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1036">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1036">VM</span></span>

* <span data-ttu-id="0c3bf-1037">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1037">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="0c3bf-1038">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1038">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="0c3bf-1039">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1039">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="0c3bf-1040">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1040">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="0c3bf-1041">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1041">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="0c3bf-1042">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1042">May 7, 2018</span></span>

<span data-ttu-id="0c3bf-1043">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1043">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1044">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1044">Core</span></span>

* <span data-ttu-id="0c3bf-1045">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1045">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="0c3bf-1046">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1046">Added limited support for positional arguments</span></span>
* <span data-ttu-id="0c3bf-1047">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1047">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="0c3bf-1048">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1048">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="0c3bf-1049">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1049">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="0c3bf-1050">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1050">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="0c3bf-1051">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1051">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="0c3bf-1052">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1052">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="0c3bf-1053">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1053">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-1054">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1054">ACR</span></span>

* <span data-ttu-id="0c3bf-1055">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1055">Added ACR Build commands</span></span>
* <span data-ttu-id="0c3bf-1056">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1056">Improved resource not found error messages</span></span>
* <span data-ttu-id="0c3bf-1057">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1057">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="0c3bf-1058">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1058">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="0c3bf-1059">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1059">Improved repository commands error messages</span></span>
* <span data-ttu-id="0c3bf-1060">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1060">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1061">ACS</span></span>

* <span data-ttu-id="0c3bf-1062">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1062">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="0c3bf-1063">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1063">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="0c3bf-1064">AMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1064">AMS</span></span>

* <span data-ttu-id="0c3bf-1065">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1065">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1066">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1066">Appservice</span></span>

* <span data-ttu-id="0c3bf-1067">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1067">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="0c3bf-1068">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1068">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="0c3bf-1069">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1069">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="0c3bf-1070">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1070">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0c3bf-1071">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1071">Batch AI</span></span>

* <span data-ttu-id="0c3bf-1072">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1072">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0c3bf-1073">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1073">Cognitive Services</span></span>

* <span data-ttu-id="0c3bf-1074">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1074">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="0c3bf-1075">Consumo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1075">Consumption</span></span>

* <span data-ttu-id="0c3bf-1076">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1076">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1077">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1077">Container</span></span>

* <span data-ttu-id="0c3bf-1078">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1078">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0c3bf-1079">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1079">Cosmos DB</span></span>

* <span data-ttu-id="0c3bf-1080">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1080">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="0c3bf-1081">DMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1081">DMS</span></span>

* <span data-ttu-id="0c3bf-1082">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1082">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1083">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1083">Extension</span></span>

* <span data-ttu-id="0c3bf-1084">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1084">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1085">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1085">Interactive</span></span>

* <span data-ttu-id="0c3bf-1086">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1086">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="0c3bf-1087">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1087">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="0c3bf-1088">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1088">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="0c3bf-1089">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1089">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="0c3bf-1090">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1090">Lab</span></span>

* <span data-ttu-id="0c3bf-1091">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1091">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1092">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1092">Network</span></span>

* <span data-ttu-id="0c3bf-1093">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1093">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="0c3bf-1094">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1094">Profile</span></span>

* <span data-ttu-id="0c3bf-1095">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1095">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="0c3bf-1096">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1096">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="0c3bf-1097">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1097">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="0c3bf-1098">Redis</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1098">Redis</span></span>

* <span data-ttu-id="0c3bf-1099">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1099">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="0c3bf-1100">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1100">Deprecated `redis list-all`.</span></span> <span data-ttu-id="0c3bf-1101">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1101">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="0c3bf-1102">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1102">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="0c3bf-1103">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1103">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-1104">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1104">Role</span></span>

* <span data-ttu-id="0c3bf-1105">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1105">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1106">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1106">Storage</span></span>

* <span data-ttu-id="0c3bf-1107">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1107">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="0c3bf-1108">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1108">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="0c3bf-1109">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1109">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="0c3bf-1110">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1110">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="0c3bf-1111">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1111">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1112">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1112">VM</span></span>

* <span data-ttu-id="0c3bf-1113">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1113">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="0c3bf-1114">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1114">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="0c3bf-1115">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1115">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="0c3bf-1116">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1116">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="0c3bf-1117">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1117">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="0c3bf-1118">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1118">Added write accelerator support</span></span>
* <span data-ttu-id="0c3bf-1119">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1119">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="0c3bf-1120">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1120">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="0c3bf-1121">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1121">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="0c3bf-1122">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1122">April 10, 2018</span></span>

<span data-ttu-id="0c3bf-1123">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1123">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-1124">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1124">ACR</span></span>

* <span data-ttu-id="0c3bf-1125">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1125">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1126">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1126">ACS</span></span>

* <span data-ttu-id="0c3bf-1127">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1127">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1128">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1128">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="0c3bf-1130">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1130">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="0c3bf-1131">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1131">BatchAI</span></span>

* <span data-ttu-id="0c3bf-1132">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1132">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="0c3bf-1133">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1133">Job level mounting</span></span>
  - <span data-ttu-id="0c3bf-1134">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1134">Environment variables with secret values</span></span>
  - <span data-ttu-id="0c3bf-1135">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1135">Performance counters settings</span></span>
  - <span data-ttu-id="0c3bf-1136">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1136">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="0c3bf-1137">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1137">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="0c3bf-1138">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1138">Usage and limits reporting</span></span>
  - <span data-ttu-id="0c3bf-1139">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1139">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="0c3bf-1140">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1140">Support for custom images</span></span>
  - <span data-ttu-id="0c3bf-1141">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1141">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="0c3bf-1142">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1142">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="0c3bf-1143">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1143">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="0c3bf-1144">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1144">National clouds are supported</span></span>
* <span data-ttu-id="0c3bf-1145">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1145">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="0c3bf-1146">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1146">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="0c3bf-1147">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1147">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="0c3bf-1148">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1148">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="0c3bf-1149">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1149">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="0c3bf-1150">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1150">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="0c3bf-1151">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1151">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="0c3bf-1152">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1152">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="0c3bf-1153">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1153">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="0c3bf-1154">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1154">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="0c3bf-1155">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1155">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="0c3bf-1156">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1156">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="0c3bf-1157">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1157">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="0c3bf-1158">Facturación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1158">Billing</span></span>

* <span data-ttu-id="0c3bf-1159">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1159">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="0c3bf-1160">Consumo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1160">Consumption</span></span>

* <span data-ttu-id="0c3bf-1161">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1161">Added `marketplace` commands</span></span>
* <span data-ttu-id="0c3bf-1162">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1162">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="0c3bf-1163">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1163">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="0c3bf-1164">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1164">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="0c3bf-1165">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1165">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="0c3bf-1166">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1166">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1167">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1167">Container</span></span>

* <span data-ttu-id="0c3bf-1168">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1168">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="0c3bf-1169">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1169">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1170">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1170">Extension</span></span>

* <span data-ttu-id="0c3bf-1171">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1171">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1172">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1172">Interactive</span></span>

* <span data-ttu-id="0c3bf-1173">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1173">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="0c3bf-1174">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1174">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="0c3bf-1175">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1175">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1176">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1176">Network</span></span>

* <span data-ttu-id="0c3bf-1177">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1177">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="0c3bf-1178">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1178">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="0c3bf-1179">4910</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1179">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="0c3bf-1180">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1180">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="0c3bf-1181">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1181">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="0c3bf-1182">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1182">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1183">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1183">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1184">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1184">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1185">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1185">Profile</span></span>

* <span data-ttu-id="0c3bf-1186">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1186">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="0c3bf-1187">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1187">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-1188">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1188">RDBMS</span></span>

* <span data-ttu-id="0c3bf-1189">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1189">Added `georestore` command</span></span>
* <span data-ttu-id="0c3bf-1190">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1190">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1191">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1191">Resource</span></span>

* <span data-ttu-id="0c3bf-1192">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1192">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="0c3bf-1193">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1193">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1194">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1194">SQL</span></span>

* <span data-ttu-id="0c3bf-1195">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1195">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1196">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1196">Storage</span></span>

* <span data-ttu-id="0c3bf-1197">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1197">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1198">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1198">VM</span></span>

* <span data-ttu-id="0c3bf-1199">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1199">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="0c3bf-1200">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1200">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="0c3bf-1202">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1202">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="0c3bf-1203">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1203">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="0c3bf-1204">5718</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1204">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="0c3bf-1205">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1205">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="0c3bf-1206">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1206">March 27, 2018</span></span>

<span data-ttu-id="0c3bf-1207">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1207">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1208">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1208">Core</span></span>

* <span data-ttu-id="0c3bf-1209">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1209">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1210">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1210">ACS</span></span>

* <span data-ttu-id="0c3bf-1211">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1211">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1212">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1212">Appservice</span></span>

* <span data-ttu-id="0c3bf-1213">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1213">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="0c3bf-1214">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1214">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0c3bf-1215">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1215">Backup</span></span>

* <span data-ttu-id="0c3bf-1216">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1216">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="0c3bf-1217">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1217">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="0c3bf-1218">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1218">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="0c3bf-1219">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1219">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1220">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1220">Container</span></span>

* <span data-ttu-id="0c3bf-1221">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1221">Added `container exec` command.</span></span> <span data-ttu-id="0c3bf-1222">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1222">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="0c3bf-1223">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1223">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1224">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1224">Extension</span></span>

* <span data-ttu-id="0c3bf-1225">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1225">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="0c3bf-1226">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1226">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="0c3bf-1227">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1227">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1228">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1228">Interactive</span></span>

* <span data-ttu-id="0c3bf-1229">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1229">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="0c3bf-1230">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1230">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="0c3bf-1231">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1231">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="0c3bf-1232">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1232">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="0c3bf-1233">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1233">Lab</span></span>

* <span data-ttu-id="0c3bf-1234">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1234">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1235">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1235">Monitor</span></span>

* <span data-ttu-id="0c3bf-1236">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1236">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="0c3bf-1237">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1237">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="0c3bf-1238">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1238">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1239">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1239">Network</span></span>

* <span data-ttu-id="0c3bf-1240">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1240">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1241">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1241">Profile</span></span>

* <span data-ttu-id="0c3bf-1242">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1242">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-1243">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1243">RDBMS</span></span>

* <span data-ttu-id="0c3bf-1244">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1244">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1245">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1245">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="0c3bf-1247">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1247">Role</span></span>

* <span data-ttu-id="0c3bf-1248">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1248">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="0c3bf-1249">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1249">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="0c3bf-1250">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1250">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="0c3bf-1251">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1251">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="0c3bf-1252">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1252">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1253">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1253">Storage</span></span>

* <span data-ttu-id="0c3bf-1254">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1254">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="0c3bf-1255">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1255">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1256">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1256">VM</span></span>

* <span data-ttu-id="0c3bf-1257">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1257">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="0c3bf-1258">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1258">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="0c3bf-1259">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1259">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="0c3bf-1260">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1260">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="0c3bf-1261">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1261">March 13, 2018</span></span>

<span data-ttu-id="0c3bf-1262">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1262">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-1263">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1263">ACR</span></span>

* <span data-ttu-id="0c3bf-1264">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1264">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="0c3bf-1265">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1265">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="0c3bf-1266">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1266">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1267">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1267">ACS</span></span>

* <span data-ttu-id="0c3bf-1268">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1268">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="0c3bf-1269">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1269">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="0c3bf-1270">Advisor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1270">Advisor</span></span>

* <span data-ttu-id="0c3bf-1271">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1271">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="0c3bf-1272">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1272">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="0c3bf-1273">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1273">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="0c3bf-1274">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1274">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="0c3bf-1275">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1275">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1276">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1276">Appservice</span></span>

* <span data-ttu-id="0c3bf-1277">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1277">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="0c3bf-1278">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1278">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0c3bf-1279">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1279">Eventhubs</span></span>

* <span data-ttu-id="0c3bf-1280">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1280">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1281">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1281">Extension</span></span>

* <span data-ttu-id="0c3bf-1282">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1282">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1283">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1283">Interactive</span></span>

* <span data-ttu-id="0c3bf-1284">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1284">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="0c3bf-1285">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1285">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="0c3bf-1286">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1286">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="0c3bf-1287">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1287">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1288">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1288">Monitor</span></span>

* <span data-ttu-id="0c3bf-1289">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1289">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="0c3bf-1290">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1290">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="0c3bf-1291">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1291">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="0c3bf-1292">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1292">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1293">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1293">Network</span></span>

* <span data-ttu-id="0c3bf-1294">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1294">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="0c3bf-1295">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1295">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="0c3bf-1296">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1296">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="0c3bf-1297">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1297">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1298">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1298">Profile</span></span>

* <span data-ttu-id="0c3bf-1299">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1299">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="0c3bf-1300">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1300">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-1301">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1301">RDBMS</span></span>

* <span data-ttu-id="0c3bf-1302">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1302">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="0c3bf-1303">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1303">Service Bus</span></span>

* <span data-ttu-id="0c3bf-1304">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1304">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1305">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1305">Storage</span></span>

* <span data-ttu-id="0c3bf-1306">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1306">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="0c3bf-1307">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1307">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1308">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1308">VM</span></span>

* <span data-ttu-id="0c3bf-1309">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1309">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="0c3bf-1310">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1310">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="0c3bf-1311">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1311">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="0c3bf-1312">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1312">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="0c3bf-1313">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1313">February 27, 2018</span></span>

<span data-ttu-id="0c3bf-1314">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1314">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1315">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1315">Core</span></span>

* <span data-ttu-id="0c3bf-1316">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1316">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="0c3bf-1317">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1317">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="0c3bf-1318">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1318">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1319">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1319">ACS</span></span>

* <span data-ttu-id="0c3bf-1320">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1320">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="0c3bf-1321">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1321">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="0c3bf-1322">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1322">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="0c3bf-1323">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1323">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1324">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1324">Appservice</span></span>

* <span data-ttu-id="0c3bf-1325">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1325">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="0c3bf-1326">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1326">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0c3bf-1327">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1327">Cognitive Services</span></span>

* <span data-ttu-id="0c3bf-1328">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1328">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="0c3bf-1329">Consumo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1329">Consumption</span></span>

* <span data-ttu-id="0c3bf-1330">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1330">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="0c3bf-1331">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1331">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1332">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1332">Container</span></span>

* <span data-ttu-id="0c3bf-1333">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1333">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1334">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1334">Network</span></span>

* <span data-ttu-id="0c3bf-1335">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1335">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1336">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1336">Resource</span></span>

* <span data-ttu-id="0c3bf-1337">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1337">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-1338">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1338">Role</span></span>

* <span data-ttu-id="0c3bf-1339">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1339">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1340">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1340">SQL</span></span>

* <span data-ttu-id="0c3bf-1341">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1341">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1342">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1342">Storage</span></span>

* <span data-ttu-id="0c3bf-1343">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1343">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1344">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1344">VM</span></span>

* <span data-ttu-id="0c3bf-1345">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1345">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="0c3bf-1346">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1346">February 13, 2018</span></span>

<span data-ttu-id="0c3bf-1347">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1347">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1348">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1348">Core</span></span>

* <span data-ttu-id="0c3bf-1349">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1349">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1350">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1350">ACS</span></span>

* <span data-ttu-id="0c3bf-1351">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1351">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="0c3bf-1352">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1352">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="0c3bf-1353">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1353">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="0c3bf-1354">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1354">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="0c3bf-1355">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1355">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="0c3bf-1356">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1356">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="0c3bf-1357">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1357">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="0c3bf-1358">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1358">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1359">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1359">Appservice</span></span>

* <span data-ttu-id="0c3bf-1360">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1360">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="0c3bf-1361">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1361">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="0c3bf-1362">CDN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1362">CDN</span></span>

* <span data-ttu-id="0c3bf-1363">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1363">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1364">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1364">Container</span></span>

* <span data-ttu-id="0c3bf-1365">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1365">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="0c3bf-1366">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1366">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-1367">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1367">CosmosDB</span></span>

* <span data-ttu-id="0c3bf-1368">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1368">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1369">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1369">Extension</span></span>

* <span data-ttu-id="0c3bf-1370">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1370">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="0c3bf-1371">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1371">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="0c3bf-1372">Comentarios</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1372">Feedback</span></span>

* <span data-ttu-id="0c3bf-1373">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1373">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1374">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1374">Interactive</span></span>

* <span data-ttu-id="0c3bf-1375">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1375">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="0c3bf-1376">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1376">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-1377">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1377">IoT</span></span>

* <span data-ttu-id="0c3bf-1378">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1378">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0c3bf-1379">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1379">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0c3bf-1380">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1380">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1381">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1381">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1382">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1382">Monitor</span></span>

* <span data-ttu-id="0c3bf-1383">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1383">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1384">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1384">Network</span></span>

* <span data-ttu-id="0c3bf-1385">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1385">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="0c3bf-1386">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1386">Profile</span></span>

* <span data-ttu-id="0c3bf-1387">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1387">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1388">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1388">Resource</span></span>

* <span data-ttu-id="0c3bf-1389">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1389">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-1390">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1390">Role</span></span>

* <span data-ttu-id="0c3bf-1391">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1391">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1392">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1392">SQL</span></span>

* <span data-ttu-id="0c3bf-1393">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1393">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="0c3bf-1394">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1394">Added `sql db rename`</span></span>
* <span data-ttu-id="0c3bf-1395">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1395">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1396">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1396">Storage</span></span>

* <span data-ttu-id="0c3bf-1397">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1397">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1398">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1398">VM</span></span>

* <span data-ttu-id="0c3bf-1399">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1399">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="0c3bf-1400">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1400">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="0c3bf-1401">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1401">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="0c3bf-1402">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1402">January 31, 2018</span></span>

<span data-ttu-id="0c3bf-1403">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1403">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1404">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1404">Core</span></span>

* <span data-ttu-id="0c3bf-1405">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1405">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="0c3bf-1406">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1406">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="0c3bf-1407">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1407">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="0c3bf-1408">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1408">Use `--verbose` to see</span></span>
* <span data-ttu-id="0c3bf-1409">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1409">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1410">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1410">ACS</span></span>

* <span data-ttu-id="0c3bf-1411">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1411">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="0c3bf-1412">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1412">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1413">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1413">Appservice</span></span>

* <span data-ttu-id="0c3bf-1414">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1414">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="0c3bf-1415">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1415">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="0c3bf-1416">CDN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1416">CDN</span></span>

* <span data-ttu-id="0c3bf-1417">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1417">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-1418">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1418">CosmosDB</span></span>

* <span data-ttu-id="0c3bf-1419">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1419">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1420">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1420">Interactive</span></span>

* <span data-ttu-id="0c3bf-1421">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1421">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1422">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1422">Network</span></span>

* <span data-ttu-id="0c3bf-1423">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1423">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="0c3bf-1424">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1424">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="0c3bf-1425">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1425">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="0c3bf-1426">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1426">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="0c3bf-1427">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1427">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="0c3bf-1428">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1428">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="0c3bf-1429">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1429">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="0c3bf-1430">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1430">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="0c3bf-1431">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1431">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="0c3bf-1432">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1432">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1433">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1433">Profile</span></span>

* <span data-ttu-id="0c3bf-1434">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1434">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1435">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1435">Resource</span></span>

* <span data-ttu-id="0c3bf-1436">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1436">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1437">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1437">Storage</span></span>

* <span data-ttu-id="0c3bf-1438">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1438">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="0c3bf-1439">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1439">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="0c3bf-1440">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1440">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="0c3bf-1441">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1441">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="0c3bf-1442">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1442">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1443">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1443">VM</span></span>

* <span data-ttu-id="0c3bf-1444">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1444">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="0c3bf-1445">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1445">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="0c3bf-1446">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1446">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="0c3bf-1447">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1447">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="0c3bf-1448">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1448">January 17, 2018</span></span>

<span data-ttu-id="0c3bf-1449">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1449">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-1450">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1450">ACR</span></span>

* <span data-ttu-id="0c3bf-1451">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1451">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="0c3bf-1452">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1452">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1453">ACS</span></span>

* <span data-ttu-id="0c3bf-1454">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1454">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="0c3bf-1455">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1455">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1456">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1456">Appservice</span></span>

* <span data-ttu-id="0c3bf-1457">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1457">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="0c3bf-1458">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1458">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="0c3bf-1459">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1459">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="0c3bf-1460">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1460">Backup</span></span>

* <span data-ttu-id="0c3bf-1461">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1461">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="0c3bf-1462">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1462">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="0c3bf-1463">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1463">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="0c3bf-1464">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1464">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="0c3bf-1465">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1465">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-1466">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1466">Batch</span></span>

* <span data-ttu-id="0c3bf-1467">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1467">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="0c3bf-1468">Nube</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1468">Cloud</span></span>

* <span data-ttu-id="0c3bf-1469">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1469">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="0c3bf-1470">Consumo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1470">Consumption</span></span>

* <span data-ttu-id="0c3bf-1471">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1471">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="0c3bf-1472">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1472">Event Grid</span></span>

* <span data-ttu-id="0c3bf-1473">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1473">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0c3bf-1474">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1474">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0c3bf-1475">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1475">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="0c3bf-1476">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1476">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="0c3bf-1477">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1477">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="0c3bf-1478">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1478">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="0c3bf-1479">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1479">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="0c3bf-1480">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1480">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1481">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1481">Interactive</span></span>

* <span data-ttu-id="0c3bf-1482">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1482">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="0c3bf-1483">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1483">Fixed errors on startup</span></span>
* <span data-ttu-id="0c3bf-1484">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1484">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-1485">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1485">IoT</span></span>

* <span data-ttu-id="0c3bf-1486">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1486">Added support for device provisioning service</span></span>
* <span data-ttu-id="0c3bf-1487">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1487">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="0c3bf-1488">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1488">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1489">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1489">Monitor</span></span>

* <span data-ttu-id="0c3bf-1490">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1490">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="0c3bf-1491">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1491">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="0c3bf-1492">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1492">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1493">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1493">Network</span></span>

* <span data-ttu-id="0c3bf-1494">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1494">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="0c3bf-1495">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1495">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1496">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1496">Profile</span></span>

* <span data-ttu-id="0c3bf-1497">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1497">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-1498">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1498">Role</span></span>

* <span data-ttu-id="0c3bf-1499">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1499">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0c3bf-1500">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1500">Service Fabric</span></span>

* <span data-ttu-id="0c3bf-1501">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1501">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="0c3bf-1502">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1502">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1503">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1503">VM</span></span>

* <span data-ttu-id="0c3bf-1504">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1504">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="0c3bf-1505">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1505">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="0c3bf-1506">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1506">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="0c3bf-1507">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1507">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="0c3bf-1508">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1508">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="0c3bf-1509">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1509">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0c3bf-1510">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1510">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="0c3bf-1511">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1511">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="0c3bf-1512">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1512">December 19, 2017</span></span>

<span data-ttu-id="0c3bf-1513">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1513">Version 2.0.23</span></span>

* <span data-ttu-id="0c3bf-1514">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1514">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1515">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1515">Container</span></span>

* <span data-ttu-id="0c3bf-1516">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1516">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1517">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1517">Network</span></span>

* <span data-ttu-id="0c3bf-1518">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1518">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1519">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1519">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1520">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1520">Storage</span></span>

* <span data-ttu-id="0c3bf-1521">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1521">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1522">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1522">VM</span></span>

* <span data-ttu-id="0c3bf-1523">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1523">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="0c3bf-1524">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1524">December 5, 2017</span></span>

<span data-ttu-id="0c3bf-1525">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1525">Version 2.0.22</span></span>

* <span data-ttu-id="0c3bf-1526">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1526">Removed `az component` commands.</span></span> <span data-ttu-id="0c3bf-1527">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1527">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1528">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1528">Core</span></span>
* <span data-ttu-id="0c3bf-1529">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1529">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="0c3bf-1530">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1530">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1531">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1531">ACS</span></span>

* <span data-ttu-id="0c3bf-1532">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1532">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="0c3bf-1533">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1533">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="0c3bf-1534">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1534">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="0c3bf-1535">Advisor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1535">Advisor</span></span>

* <span data-ttu-id="0c3bf-1536">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1536">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1537">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1537">Appservice</span></span>

* <span data-ttu-id="0c3bf-1538">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1538">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="0c3bf-1539">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1539">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="0c3bf-1540">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1540">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="0c3bf-1541">Consumo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1541">Consumption</span></span>

* <span data-ttu-id="0c3bf-1542">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1542">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1543">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1543">Container</span></span>

* <span data-ttu-id="0c3bf-1544">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1544">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1545">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1545">Monitor</span></span>

* <span data-ttu-id="0c3bf-1546">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1546">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1547">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1547">Resource</span></span>

* <span data-ttu-id="0c3bf-1548">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1548">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-1549">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1549">Role</span></span>

* <span data-ttu-id="0c3bf-1550">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1550">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="0c3bf-1551">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1551">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="0c3bf-1552">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1552">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1553">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1553">SQL</span></span>

* <span data-ttu-id="0c3bf-1554">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1554">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="0c3bf-1555">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1555">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1556">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1556">VM</span></span>

* <span data-ttu-id="0c3bf-1557">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1557">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="0c3bf-1558">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1558">November 14, 2017</span></span>

<span data-ttu-id="0c3bf-1559">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1559">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-1560">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1560">ACR</span></span>

* <span data-ttu-id="0c3bf-1561">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1561">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="0c3bf-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1562">ACS</span></span>

* <span data-ttu-id="0c3bf-1563">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1563">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="0c3bf-1564">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1564">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="0c3bf-1565">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1565">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="0c3bf-1566">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1566">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="0c3bf-1567">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1567">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1568">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1568">Appservice</span></span>

* <span data-ttu-id="0c3bf-1569">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1569">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="0c3bf-1570">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1570">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="0c3bf-1571">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1571">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="0c3bf-1572">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1572">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="0c3bf-1573">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1573">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="0c3bf-1574">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1574">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-1575">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1575">Batch</span></span>

* <span data-ttu-id="0c3bf-1576">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1576">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="0c3bf-1577">Batchai</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1577">Batchai</span></span>

* <span data-ttu-id="0c3bf-1578">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1578">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="0c3bf-1579">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1579">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="0c3bf-1580">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1580">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="0c3bf-1581">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1581">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="0c3bf-1582">Nube</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1582">Cloud</span></span>

* <span data-ttu-id="0c3bf-1583">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1583">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1584">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1584">Container</span></span>

* <span data-ttu-id="0c3bf-1585">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1585">Added support to open multiple ports</span></span>
* <span data-ttu-id="0c3bf-1586">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1586">Added container group restart policy</span></span>
* <span data-ttu-id="0c3bf-1587">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1587">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="0c3bf-1588">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1588">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0c3bf-1589">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1589">Data Lake Analytics</span></span>

* <span data-ttu-id="0c3bf-1590">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1590">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0c3bf-1591">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1591">Data Lake Store</span></span>

* <span data-ttu-id="0c3bf-1592">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1592">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1593">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1593">Extension</span></span>

* <span data-ttu-id="0c3bf-1594">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1594">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="0c3bf-1595">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1595">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-1596">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1596">IoT</span></span>

* <span data-ttu-id="0c3bf-1597">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1597">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1598">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1598">Monitor</span></span>

* <span data-ttu-id="0c3bf-1599">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1599">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1600">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1600">Network</span></span>

* <span data-ttu-id="0c3bf-1601">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1601">Added support for CAA DNS records</span></span>
* <span data-ttu-id="0c3bf-1602">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1602">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="0c3bf-1603">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1603">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="0c3bf-1604">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1604">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="0c3bf-1605">Reservations</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1605">Reservations</span></span>

* <span data-ttu-id="0c3bf-1606">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1606">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1607">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1607">Resource</span></span>

* <span data-ttu-id="0c3bf-1608">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1608">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1609">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1609">SQL</span></span>

* <span data-ttu-id="0c3bf-1610">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1610">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1611">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1611">Storage</span></span>

* <span data-ttu-id="0c3bf-1612">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1612">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="0c3bf-1613">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1613">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="0c3bf-1614">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1614">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="0c3bf-1615">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1615">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="0c3bf-1616">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1616">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="0c3bf-1617">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1617">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="0c3bf-1618">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1618">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1619">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1619">VM</span></span>

* <span data-ttu-id="0c3bf-1620">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1620">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="0c3bf-1621">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1621">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="0c3bf-1622">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1622">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="0c3bf-1623">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1623">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="0c3bf-1624">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1624">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="0c3bf-1625">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1625">October 24, 2017</span></span>

<span data-ttu-id="0c3bf-1626">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1626">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1627">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1627">Core</span></span>

* <span data-ttu-id="0c3bf-1628">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1628">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-1629">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1629">ACR</span></span>

* <span data-ttu-id="0c3bf-1630">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1630">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="0c3bf-1631">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1631">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="0c3bf-1632">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1632">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1633">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1633">ACS</span></span>

* <span data-ttu-id="0c3bf-1634">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1634">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="0c3bf-1635">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1635">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1636">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1636">Appservice</span></span>

* <span data-ttu-id="0c3bf-1637">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1637">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="0c3bf-1638">Componente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1638">Component</span></span>

* <span data-ttu-id="0c3bf-1639">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1639">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1640">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1640">Monitor</span></span>

* <span data-ttu-id="0c3bf-1641">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1641">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1642">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1642">Resource</span></span>

* <span data-ttu-id="0c3bf-1643">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1643">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="0c3bf-1644">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1644">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1645">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1645">VM</span></span>

* <span data-ttu-id="0c3bf-1646">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1646">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="0c3bf-1647">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1647">October 9, 2017</span></span>

<span data-ttu-id="0c3bf-1648">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1648">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1649">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1649">Core</span></span>

* <span data-ttu-id="0c3bf-1650">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1650">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1651">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1651">Appservice</span></span>

* <span data-ttu-id="0c3bf-1652">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1652">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-1653">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1653">Batch</span></span>

* <span data-ttu-id="0c3bf-1654">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1654">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="0c3bf-1655">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1655">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="0c3bf-1656">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1656">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="0c3bf-1657">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1657">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="0c3bf-1658">Batchai</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1658">Batchai</span></span>

* <span data-ttu-id="0c3bf-1659">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1659">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-1660">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1660">Keyvault</span></span>

* <span data-ttu-id="0c3bf-1661">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1661">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="0c3bf-1662">(#4448)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1662">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="0c3bf-1663">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1663">Network</span></span>

* <span data-ttu-id="0c3bf-1664">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1664">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="0c3bf-1665">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1665">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1666">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1666">Resource</span></span>

* <span data-ttu-id="0c3bf-1667">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1667">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="0c3bf-1668">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1668">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="0c3bf-1669">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1669">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="0c3bf-1670">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1670">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1671">Sql</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1671">Sql</span></span>

* <span data-ttu-id="0c3bf-1672">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1672">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="0c3bf-1673">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1673">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="0c3bf-1674">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1674">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1675">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1675">Storage</span></span>

* <span data-ttu-id="0c3bf-1676">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1676">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1677">Vm</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1677">Vm</span></span>

* <span data-ttu-id="0c3bf-1678">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1678">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="0c3bf-1679">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1679">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="0c3bf-1680">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1680">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="0c3bf-1681">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1681">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="0c3bf-1682">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1682">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="0c3bf-1683">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1683">September 22, 2017</span></span>

<span data-ttu-id="0c3bf-1684">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1684">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1685">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1685">Resource</span></span>

* <span data-ttu-id="0c3bf-1686">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1686">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="0c3bf-1687">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1687">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="0c3bf-1688">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1688">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="0c3bf-1689">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1689">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1690">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1690">Network</span></span>

* <span data-ttu-id="0c3bf-1691">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1691">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="0c3bf-1692">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1692">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="0c3bf-1693">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1693">Added `asg` application security group commands</span></span>
* <span data-ttu-id="0c3bf-1694">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1694">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="0c3bf-1695">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1695">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1696">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1696">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1697">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1697">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1698">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1698">Storage</span></span>

* <span data-ttu-id="0c3bf-1699">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1699">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0c3bf-1700">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1700">Eventgrid</span></span>

* <span data-ttu-id="0c3bf-1701">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1701">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1702">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1702">SQL</span></span>

* <span data-ttu-id="0c3bf-1703">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1703">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="0c3bf-1704">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1704">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="0c3bf-1705">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1705">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-1706">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1706">Keyvault</span></span>

* <span data-ttu-id="0c3bf-1707">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1707">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1708">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1708">VM</span></span>

* <span data-ttu-id="0c3bf-1709">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1709">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="0c3bf-1710">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1710">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="0c3bf-1711">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1711">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="0c3bf-1712">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1712">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="0c3bf-1713">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1713">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="0c3bf-1714">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1714">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1715">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1715">ACS</span></span>

* <span data-ttu-id="0c3bf-1716">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1716">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1717">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1717">Appservice</span></span>

* <span data-ttu-id="0c3bf-1718">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1718">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0c3bf-1719">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1719">Backup</span></span>

* <span data-ttu-id="0c3bf-1720">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1720">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="0c3bf-1721">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1721">September 11, 2017</span></span>

<span data-ttu-id="0c3bf-1722">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1722">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="0c3bf-1723">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1723">Core</span></span>

* <span data-ttu-id="0c3bf-1724">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1724">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="0c3bf-1725">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1725">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1726">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1726">Acs</span></span>

* <span data-ttu-id="0c3bf-1727">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1727">Added `acs list-locations` command</span></span>
* <span data-ttu-id="0c3bf-1728">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1728">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1729">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1729">Appservice</span></span>

* <span data-ttu-id="0c3bf-1730">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1730">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="0c3bf-1731">CDN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1731">CDN</span></span>

* <span data-ttu-id="0c3bf-1732">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1732">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="0c3bf-1733">Extensión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1733">Extension</span></span>

* <span data-ttu-id="0c3bf-1734">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1734">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-1735">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1735">Keyvault</span></span>

* <span data-ttu-id="0c3bf-1736">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1736">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1737">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1737">Network</span></span>

* <span data-ttu-id="0c3bf-1738">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1738">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0c3bf-1739">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1739">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="0c3bf-1740">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1740">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="0c3bf-1741">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1741">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0c3bf-1742">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1742">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1743">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1743">Resource</span></span>

* <span data-ttu-id="0c3bf-1744">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1744">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="0c3bf-1745">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1745">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="0c3bf-1746">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1746">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="0c3bf-1747">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1747">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-1748">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1748">SQL</span></span>

* <span data-ttu-id="0c3bf-1749">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1749">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1750">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1750">VM</span></span>

* <span data-ttu-id="0c3bf-1751">Problema corregido: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1751">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="0c3bf-1752">Problema corregido: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1752">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="0c3bf-1753">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1753">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="0c3bf-1754">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1754">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="0c3bf-1755">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1755">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="0c3bf-1756">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1756">August 31, 2017</span></span>

<span data-ttu-id="0c3bf-1757">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1757">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-1758">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1758">Keyvault</span></span>

* <span data-ttu-id="0c3bf-1759">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1759">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="0c3bf-1760">Sf</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1760">Sf</span></span>

* <span data-ttu-id="0c3bf-1761">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1761">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1762">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1762">Storage</span></span>

* <span data-ttu-id="0c3bf-1763">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1763">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="0c3bf-1764">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1764">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="0c3bf-1765">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1765">August 28, 2017</span></span>

<span data-ttu-id="0c3bf-1766">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1766">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="0c3bf-1767">CLI</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1767">CLI</span></span>

* <span data-ttu-id="0c3bf-1768">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1768">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1769">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1769">ACS</span></span>

* <span data-ttu-id="0c3bf-1770">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1770">Corrected preview regions</span></span>
* <span data-ttu-id="0c3bf-1771">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1771">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="0c3bf-1772">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1772">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1773">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1773">Appservice</span></span>

* <span data-ttu-id="0c3bf-1774">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1774">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="0c3bf-1775">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1775">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="0c3bf-1776">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1776">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="0c3bf-1777">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1777">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="0c3bf-1778">Problema corregido: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1778">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-1779">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1779">IoT</span></span>

* <span data-ttu-id="0c3bf-1780">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1780">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1781">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1781">Network</span></span>

* <span data-ttu-id="0c3bf-1782">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1782">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0c3bf-1783">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1783">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1784">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1784">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0c3bf-1785">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1785">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0c3bf-1786">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1786">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1787">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1787">Profile</span></span>

* <span data-ttu-id="0c3bf-1788">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1788">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0c3bf-1789">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1789">Service Fabric</span></span>

* <span data-ttu-id="0c3bf-1790">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1790">Preview release</span></span>
* <span data-ttu-id="0c3bf-1791">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1791">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="0c3bf-1792">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1792">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="0c3bf-1793">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1793">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1794">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1794">Storage</span></span>

* <span data-ttu-id="0c3bf-1795">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1795">Enabled setting blob tier</span></span>
* <span data-ttu-id="0c3bf-1796">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1796">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="0c3bf-1797">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1797">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="0c3bf-1798">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1798">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="0c3bf-1799">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1799">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="0c3bf-1800">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1800">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1801">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1801">VM</span></span>

* <span data-ttu-id="0c3bf-1802">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1802">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="0c3bf-1803">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1803">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="0c3bf-1804">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1804">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="0c3bf-1805">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1805">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="0c3bf-1806">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1806">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="0c3bf-1807">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1807">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="0c3bf-1808">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1808">August 15, 2017</span></span>

<span data-ttu-id="0c3bf-1809">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1809">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1810">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1810">ACS</span></span>

* <span data-ttu-id="0c3bf-1811">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1811">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1812">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1812">Appservice</span></span>

* <span data-ttu-id="0c3bf-1813">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1813">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="0c3bf-1814">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1814">Event Grid</span></span>

* <span data-ttu-id="0c3bf-1815">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1815">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="0c3bf-1816">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1816">August 11, 2017</span></span>

<span data-ttu-id="0c3bf-1817">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1817">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1818">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1818">ACS</span></span>

* <span data-ttu-id="0c3bf-1819">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1819">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-1820">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1820">Batch</span></span>

* <span data-ttu-id="0c3bf-1821">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1821">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="0c3bf-1822">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1822">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="0c3bf-1823">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1823">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="0c3bf-1824">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1824">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="0c3bf-1825">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1825">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="0c3bf-1826">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1826">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="0c3bf-1827">Componente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1827">Component</span></span>

* <span data-ttu-id="0c3bf-1828">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1828">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="0c3bf-1829">Contenedor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1829">Container</span></span>

* <span data-ttu-id="0c3bf-1830">`create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1830">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="0c3bf-1831">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1831">Data Lake Store</span></span>

* <span data-ttu-id="0c3bf-1832">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1832">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="0c3bf-1833">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1833">Event Grid</span></span>

* <span data-ttu-id="0c3bf-1834">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1834">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1835">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1835">Network</span></span>

* <span data-ttu-id="0c3bf-1836">`lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1836">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="0c3bf-1837">`application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1837">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="0c3bf-1838">`application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1838">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="0c3bf-1839">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1839">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1840">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1840">Profile</span></span>

* <span data-ttu-id="0c3bf-1841">`account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1841">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-1842">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1842">Storage</span></span>

* <span data-ttu-id="0c3bf-1843">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1843">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-1844">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1844">VM</span></span>

* <span data-ttu-id="0c3bf-1845">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1845">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="0c3bf-1846">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1846">Exposed `list-skus` command</span></span>
* <span data-ttu-id="0c3bf-1847">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1847">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="0c3bf-1848">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1848">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="0c3bf-1849">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1849">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="0c3bf-1850">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1850">July 28, 2017</span></span>

<span data-ttu-id="0c3bf-1851">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1851">Version 2.0.12</span></span>

* <span data-ttu-id="0c3bf-1852">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1852">Added container commands</span></span>
* <span data-ttu-id="0c3bf-1853">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1853">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="0c3bf-1854">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1854">Core</span></span>

* <span data-ttu-id="0c3bf-1855">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1855">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="0c3bf-1856">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1856">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="0c3bf-1857">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1857">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="0c3bf-1858">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1858">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="0c3bf-1859">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1859">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="0c3bf-1860">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1860">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="0c3bf-1861">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1861">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0c3bf-1862">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1862">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="0c3bf-1863">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1863">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="0c3bf-1864">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1864">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="0c3bf-1865">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1865">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="0c3bf-1866">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1866">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="0c3bf-1867">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1867">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="0c3bf-1868">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1868">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="0c3bf-1869">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1869">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="0c3bf-1870">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1870">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="0c3bf-1871">ACR</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1871">ACR</span></span>

* <span data-ttu-id="0c3bf-1872">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1872">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="0c3bf-1873">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1873">Support SKU update for managed registries</span></span>
* <span data-ttu-id="0c3bf-1874">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1874">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="0c3bf-1875">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1875">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="0c3bf-1876">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1876">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="0c3bf-1877">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1877">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-1878">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1878">ACS</span></span>

* <span data-ttu-id="0c3bf-1879">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1879">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-1880">Appservice</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1880">Appservice</span></span>

* <span data-ttu-id="0c3bf-1881">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1881">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="0c3bf-1882">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1882">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="0c3bf-1883">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1883">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="0c3bf-1884">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1884">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="0c3bf-1885">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1885">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="0c3bf-1886">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1886">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="0c3bf-1887">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1887">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="0c3bf-1888">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1888">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="0c3bf-1889">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1889">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="0c3bf-1890">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1890">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="0c3bf-1891">Batch</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1891">Batch</span></span>

* <span data-ttu-id="0c3bf-1892">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1892">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="0c3bf-1893">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1893">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="0c3bf-1894">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1894">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="0c3bf-1895">CDN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1895">CDN</span></span>

* <span data-ttu-id="0c3bf-1896">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1896">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="0c3bf-1897">Nube</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1897">Cloud</span></span>

* <span data-ttu-id="0c3bf-1898">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1898">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="0c3bf-1899">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1899">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="0c3bf-1900">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1900">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="0c3bf-1901">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1901">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="0c3bf-1902">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1902">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-1903">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1903">CosmosDB</span></span>

* <span data-ttu-id="0c3bf-1904">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1904">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="0c3bf-1905">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1905">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0c3bf-1906">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1906">Data Lake Analytics</span></span>

* <span data-ttu-id="0c3bf-1907">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1907">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="0c3bf-1908">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1908">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="0c3bf-1909">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1909">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0c3bf-1910">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1910">Data Lake Store</span></span>

* <span data-ttu-id="0c3bf-1911">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1911">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="0c3bf-1912">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1912">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="0c3bf-1913">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1913">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="0c3bf-1914">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1914">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="0c3bf-1915">Interactive</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1915">Interactive</span></span>

* <span data-ttu-id="0c3bf-1916">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1916">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="0c3bf-1917">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1917">Increased test coverage</span></span>
* <span data-ttu-id="0c3bf-1918">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1918">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="0c3bf-1919">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1919">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="0c3bf-1920">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1920">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="0c3bf-1921">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1921">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="0c3bf-1922">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1922">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0c3bf-1923">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1923">Added `--progress` flag</span></span>
* <span data-ttu-id="0c3bf-1924">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1924">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="0c3bf-1925">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1925">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="0c3bf-1926">IoT</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1926">IoT</span></span>

* <span data-ttu-id="0c3bf-1927">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1927">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="0c3bf-1928">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1928">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="0c3bf-1929">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1929">Key vault</span></span>

* <span data-ttu-id="0c3bf-1930">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1930">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="0c3bf-1931">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1931">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="0c3bf-1932">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1932">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0c3bf-1933">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1933">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0c3bf-1934">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1934">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="0c3bf-1935">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1935">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="0c3bf-1936">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1936">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="0c3bf-1937">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1937">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="0c3bf-1938">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1938">Lab</span></span>

* <span data-ttu-id="0c3bf-1939">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1939">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="0c3bf-1940">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1940">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-1941">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1941">Monitor</span></span>

* <span data-ttu-id="0c3bf-1942">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1942">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="0c3bf-1943">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1943">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="0c3bf-1944">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1944">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="0c3bf-1945">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1945">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="0c3bf-1946">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1946">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="0c3bf-1947">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1947">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="0c3bf-1948">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1948">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="0c3bf-1949">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1949">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="0c3bf-1950">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1950">`location` no longer required</span></span>
  * <span data-ttu-id="0c3bf-1951">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1951">Add name and ID support for target</span></span>
  * <span data-ttu-id="0c3bf-1952">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1952">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="0c3bf-1953">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1953">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="0c3bf-1954">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1954">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="0c3bf-1955">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1955">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="0c3bf-1956">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1956">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="0c3bf-1957">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1957">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-1958">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1958">Network</span></span>

* <span data-ttu-id="0c3bf-1959">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1959">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="0c3bf-1960">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1960">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="0c3bf-1961">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1961">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="0c3bf-1962">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1962">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="0c3bf-1963">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1963">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="0c3bf-1964">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1964">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="0c3bf-1965">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1965">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="0c3bf-1966">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1966">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="0c3bf-1967">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1967">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="0c3bf-1968">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1968">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="0c3bf-1969">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1969">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="0c3bf-1970">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1970">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="0c3bf-1971">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1971">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="0c3bf-1972">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1972">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="0c3bf-1973">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1973">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="0c3bf-1974">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1974">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="0c3bf-1975">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1975">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="0c3bf-1976">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1976">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="0c3bf-1977">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1977">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="0c3bf-1978">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1978">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="0c3bf-1979">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1979">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="0c3bf-1980">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1980">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="0c3bf-1981">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1981">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="0c3bf-1982">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1982">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="0c3bf-1983">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1983">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="0c3bf-1984">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1984">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="0c3bf-1985">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1985">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-1986">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1986">Profile</span></span>

* <span data-ttu-id="0c3bf-1987">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1987">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="0c3bf-1988">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1988">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="0c3bf-1989">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1989">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="0c3bf-1990">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1990">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="0c3bf-1991">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1991">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="0c3bf-1992">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1992">RDBMS</span></span>

* <span data-ttu-id="0c3bf-1993">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1993">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="0c3bf-1994">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1994">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="0c3bf-1995">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1995">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="0c3bf-1996">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1996">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-1997">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1997">Resource</span></span>

* <span data-ttu-id="0c3bf-1998">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1998">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="0c3bf-1999">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-1999">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="0c3bf-2000">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2000">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="0c3bf-2001">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2001">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="0c3bf-2002">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2002">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="0c3bf-2003">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2003">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="0c3bf-2004">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2004">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="0c3bf-2005">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2005">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-2006">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2006">Role</span></span>

* <span data-ttu-id="0c3bf-2007">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2007">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="0c3bf-2008">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2008">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="0c3bf-2009">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2009">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="0c3bf-2010">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2010">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="0c3bf-2011">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2011">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0c3bf-2012">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2012">Service Fabric</span></span>
* <span data-ttu-id="0c3bf-2013">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2013">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="0c3bf-2014">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2014">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="0c3bf-2015">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2015">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2016">SQL</span></span>

* <span data-ttu-id="0c3bf-2017">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2017">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="0c3bf-2018">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2018">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="0c3bf-2019">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2019">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-2020">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2020">Storage</span></span>

* <span data-ttu-id="0c3bf-2021">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2021">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="0c3bf-2022">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2022">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="0c3bf-2023">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2023">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="0c3bf-2024">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2024">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="0c3bf-2025">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2025">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="0c3bf-2026">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2026">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-2027">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2027">VM</span></span>

* <span data-ttu-id="0c3bf-2028">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2028">Support configuring nsg</span></span>
* <span data-ttu-id="0c3bf-2029">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2029">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="0c3bf-2030">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2030">Support managed service identities</span></span>
* <span data-ttu-id="0c3bf-2031">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2031">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="0c3bf-2032">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2032">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="0c3bf-2033">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2033">May 10, 2017</span></span>

<span data-ttu-id="0c3bf-2034">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2034">Version 2.0.6</span></span>

* <span data-ttu-id="0c3bf-2035">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2035">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="0c3bf-2036">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2036">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="0c3bf-2037">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2037">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="0c3bf-2038">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2038">Include Cognitive Services module</span></span>
* <span data-ttu-id="0c3bf-2039">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2039">Include Service Fabric module</span></span>
* <span data-ttu-id="0c3bf-2040">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2040">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="0c3bf-2041">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2041">Add support for CDN commands</span></span>
* <span data-ttu-id="0c3bf-2042">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2042">Remove Container module</span></span>
* <span data-ttu-id="0c3bf-2043">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2043">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="0c3bf-2044">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2044">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="0c3bf-2045">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2045">Core</span></span>

* <span data-ttu-id="0c3bf-2046">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2046">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="0c3bf-2047">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2047">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="0c3bf-2048">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2048">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="0c3bf-2049">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2049">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="0c3bf-2050">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2050">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="0c3bf-2051">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2051">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="0c3bf-2052">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2052">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="0c3bf-2053">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2053">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="0c3bf-2054">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2054">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="0c3bf-2055">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2055">core: Improved performance</span></span>
* <span data-ttu-id="0c3bf-2056">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2056">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="0c3bf-2057">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2057">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-2058">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2058">ACS</span></span>

* <span data-ttu-id="0c3bf-2059">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2059">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="0c3bf-2060">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2060">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="0c3bf-2061">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2061">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="0c3bf-2062">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2062">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-2063">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2063">AppService</span></span>

* <span data-ttu-id="0c3bf-2064">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2064">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="0c3bf-2065">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2065">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="0c3bf-2066">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2066">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="0c3bf-2067">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2067">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="0c3bf-2068">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2068">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="0c3bf-2069">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2069">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="0c3bf-2070">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2070">support slot swap with preview</span></span>
* <span data-ttu-id="0c3bf-2071">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2071">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="0c3bf-2072">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2072">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0c3bf-2073">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2073">CosmosDB</span></span>

* <span data-ttu-id="0c3bf-2074">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2074">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="0c3bf-2075">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2075">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="0c3bf-2076">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2076">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="0c3bf-2077">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2077">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0c3bf-2078">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2078">Data Lake Analytics</span></span>

* <span data-ttu-id="0c3bf-2079">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2079">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="0c3bf-2080">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2080">Add support for new catalog item type: package.</span></span> <span data-ttu-id="0c3bf-2081">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2081">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="0c3bf-2082">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2082">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="0c3bf-2083">Tabla</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2083">Table</span></span>
  * <span data-ttu-id="0c3bf-2084">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2084">Table valued function</span></span>
  * <span data-ttu-id="0c3bf-2085">Ver</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2085">View</span></span>
  * <span data-ttu-id="0c3bf-2086">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2086">Table Statistics.</span></span> <span data-ttu-id="0c3bf-2087">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2087">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0c3bf-2088">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2088">Data Lake Store</span></span>

* <span data-ttu-id="0c3bf-2089">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2089">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="0c3bf-2090">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2090">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="0c3bf-2091">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2091">missed help for access show.</span></span> <span data-ttu-id="0c3bf-2092">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2092">adding it.</span></span> <span data-ttu-id="0c3bf-2093">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2093">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="0c3bf-2094">Buscar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2094">Find</span></span>

* <span data-ttu-id="0c3bf-2095">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2095">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="0c3bf-2096">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2096">KeyVault</span></span>

* <span data-ttu-id="0c3bf-2097">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2097">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="0c3bf-2098">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2098">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="0c3bf-2099">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2099">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="0c3bf-2100">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2100">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="0c3bf-2101">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2101">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="0c3bf-2102">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2102">Lab</span></span>

* <span data-ttu-id="0c3bf-2103">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2103">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="0c3bf-2104">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2104">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="0c3bf-2105">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2105">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="0c3bf-2106">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2106">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="0c3bf-2107">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2107">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="0c3bf-2108">Supervisión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2108">Monitor</span></span>

* <span data-ttu-id="0c3bf-2109">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2109">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="0c3bf-2110">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2110">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="0c3bf-2111">Red</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2111">Network</span></span>

* <span data-ttu-id="0c3bf-2112">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2112">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="0c3bf-2113">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2113">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="0c3bf-2114">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2114">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="0c3bf-2115">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2115">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="0c3bf-2116">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2116">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="0c3bf-2117">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2117">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="0c3bf-2118">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2118">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="0c3bf-2119">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2119">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="0c3bf-2120">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2120">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="0c3bf-2121">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2121">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="0c3bf-2122">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2122">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="0c3bf-2123">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2123">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="0c3bf-2124">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2124">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="0c3bf-2125">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2125">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="0c3bf-2126">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2126">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="0c3bf-2127">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2127">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="0c3bf-2128">Perfil</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2128">Profile</span></span>

* <span data-ttu-id="0c3bf-2129">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2129">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="0c3bf-2130">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2130">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="0c3bf-2131">Redis</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2131">Redis</span></span>

* <span data-ttu-id="0c3bf-2132">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2132">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="0c3bf-2133">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2133">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="0c3bf-2134">Recurso</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2134">Resource</span></span>

* <span data-ttu-id="0c3bf-2135">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2135">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="0c3bf-2136">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2136">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="0c3bf-2137">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2137">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="0c3bf-2138">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2138">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="0c3bf-2139">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2139">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="0c3bf-2140">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2140">Add docs for az lock update.</span></span> <span data-ttu-id="0c3bf-2141">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2141">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="0c3bf-2142">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2142">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="0c3bf-2143">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2143">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="0c3bf-2144">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2144">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="0c3bf-2145">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2145">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="0c3bf-2146">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2146">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="0c3bf-2147">Rol</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2147">Role</span></span>

* <span data-ttu-id="0c3bf-2148">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2148">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="0c3bf-2149">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2149">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="0c3bf-2150">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2150">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="0c3bf-2151">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2151">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="0c3bf-2152">SQL</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2152">SQL</span></span>

* <span data-ttu-id="0c3bf-2153">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2153">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="0c3bf-2154">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2154">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="0c3bf-2155">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2155">Storage</span></span>

* <span data-ttu-id="0c3bf-2156">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2156">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="0c3bf-2157">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2157">Add support for incremental blob copy</span></span>
* <span data-ttu-id="0c3bf-2158">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2158">Add support for large block blob upload</span></span>
* <span data-ttu-id="0c3bf-2159">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2159">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-2160">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2160">VM</span></span>

* <span data-ttu-id="0c3bf-2161">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2161">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="0c3bf-2162">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2162">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="0c3bf-2163">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2163">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="0c3bf-2164">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2164">az vm/vmss disk</span></span>
  3. <span data-ttu-id="0c3bf-2165">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2165">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="0c3bf-2166">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2166">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="0c3bf-2167">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2167">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="0c3bf-2168">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2168">April 3, 2017</span></span>

<span data-ttu-id="0c3bf-2169">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2169">Version 2.0.2</span></span>

<span data-ttu-id="0c3bf-2170">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2170">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="0c3bf-2171">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2171">Core</span></span>

* <span data-ttu-id="0c3bf-2172">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2172">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="0c3bf-2173">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2173">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="0c3bf-2174">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2174">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="0c3bf-2175">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2175">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0c3bf-2176">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2176">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="0c3bf-2177">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2177">Add prompting for missing template parameters.</span></span> <span data-ttu-id="0c3bf-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="0c3bf-2179">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2179">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="0c3bf-2180">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2180">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="0c3bf-2181">ACS</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2181">ACS</span></span>

* <span data-ttu-id="0c3bf-2182">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2182">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="0c3bf-2183">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2183">Add support for ssh key password prompting.</span></span> <span data-ttu-id="0c3bf-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="0c3bf-2185">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2185">Add support for windows clusters.</span></span> <span data-ttu-id="0c3bf-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="0c3bf-2187">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2187">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="0c3bf-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="0c3bf-2189">AppService</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2189">AppService</span></span>

* <span data-ttu-id="0c3bf-2190">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2190">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="0c3bf-2191">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2191">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="0c3bf-2192">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2192">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="0c3bf-2193">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2193">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="0c3bf-2194">DataLake</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2194">DataLake</span></span>

* <span data-ttu-id="0c3bf-2195">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2195">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="0c3bf-2196">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2196">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="0c3bf-2197">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2197">DocuemntDB</span></span>

* <span data-ttu-id="0c3bf-2198">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2198">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="0c3bf-2199">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2199">VM</span></span>

* <span data-ttu-id="0c3bf-2200">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2200">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="0c3bf-2201">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2201">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="0c3bf-2202">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2202">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="0c3bf-2203">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2203">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0c3bf-2204">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2204">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="0c3bf-2205">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2205">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="0c3bf-2206">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2206">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="0c3bf-2207">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2207">February 27, 2017</span></span>

<span data-ttu-id="0c3bf-2208">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2208">Version 2.0.0</span></span>

<span data-ttu-id="0c3bf-2209">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2209">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="0c3bf-2210">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2210">Container Service (acs)</span></span>
- <span data-ttu-id="0c3bf-2211">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2211">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="0c3bf-2212">Redes</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2212">Networking</span></span>
- <span data-ttu-id="0c3bf-2213">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2213">Storage</span></span>

<span data-ttu-id="0c3bf-2214">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2214">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="0c3bf-2215">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2215">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="0c3bf-2216">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2216">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="0c3bf-2217">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2217">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="0c3bf-2218">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2218">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="0c3bf-2219">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2219">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="0c3bf-2220">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2220">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="0c3bf-2221">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2221">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="0c3bf-2222">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="0c3bf-2222">Provide feedback from the command line with the `az feedback` command</span></span>

