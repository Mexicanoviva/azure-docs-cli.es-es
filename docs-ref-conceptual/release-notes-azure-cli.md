---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/09/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: df665565130322504c4794462098980b1064a6c7
ms.sourcegitcommit: c6dff58438d256647d4aa29a53eef4bf93a0cd24
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/11/2019
ms.locfileid: "59480004"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="012e3-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="012e3-103">Azure CLI release notes</span></span>
## <a name="april-9-2019"></a><span data-ttu-id="012e3-104">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-104">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="012e3-105">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-105">Core</span></span>
* <span data-ttu-id="012e3-106">Se ha corregido el problema por el que algunas extensiones mostraban una versión `Unknown` y no se podían actualizar.</span><span class="sxs-lookup"><span data-stu-id="012e3-106">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-107">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-107">ACR</span></span>
* <span data-ttu-id="012e3-108">Se ha agregado compatibilidad con la ejecución de una imagen sin contexto.</span><span class="sxs-lookup"><span data-stu-id="012e3-108">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="012e3-109">AMS</span><span class="sxs-lookup"><span data-stu-id="012e3-109">AMS</span></span>
* [<span data-ttu-id="012e3-110">EN DESUSO</span><span class="sxs-lookup"><span data-stu-id="012e3-110">DEPRECATED</span></span>]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [<span data-ttu-id="012e3-111">CAMBIO IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="012e3-111">BREAKING CHANGE</span></span>]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="012e3-112">Se ha agregado compatibilidad con los parámetros de cifrado en</span><span class="sxs-lookup"><span data-stu-id="012e3-112">Added new encryption parameters support in</span></span> `ams streaming-policy create`
* <span data-ttu-id="012e3-113">Se ha agregado un nuevo parámetro `--filters` a</span><span class="sxs-lookup"><span data-stu-id="012e3-113">Added new paramter `--filters` to</span></span> `ams streaming-locator create`

### <a name="appservice"></a><span data-ttu-id="012e3-114">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-114">AppService</span></span>
* <span data-ttu-id="012e3-115">Se ha agregado compatibilidad con `--logs` a</span><span class="sxs-lookup"><span data-stu-id="012e3-115">Added `--logs` support to</span></span> `webapp up`
* <span data-ttu-id="012e3-116">En el comando `functionapp devops-build create`, se han corregido los problemas de generación de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="012e3-116">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="012e3-117">Se ha mejorado el control de errores y los indicadores de `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="012e3-117">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="012e3-118">[CAMBIO IMPORTANTE] Se ha quitado la marca `--local-git` del comando `devops-build`; la detección y administración del repositorio git local son obligatorias para crear canalizaciones de Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="012e3-118">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="012e3-119">Se ha agregado compatibilidad para crear planes de funciones Linux</span><span class="sxs-lookup"><span data-stu-id="012e3-119">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="012e3-120">Se ha agregado la posibilidad de cambiar un plan subyacente a una aplicación de función mediante</span><span class="sxs-lookup"><span data-stu-id="012e3-120">Added ability to switch a plan underneath a function app using</span></span> `functionapp update --plan`
* <span data-ttu-id="012e3-121">Se ha agregado compatibilidad para las opciones de escalado horizontal del plan Premium de Azure Functions</span><span class="sxs-lookup"><span data-stu-id="012e3-121">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="012e3-122">CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-122">CDN</span></span>
* <span data-ttu-id="012e3-123">Se ha agregado compatibilidad para `Microsoft_Standard` y</span><span class="sxs-lookup"><span data-stu-id="012e3-123">Added support for `Microsoft_Standard` and</span></span> `Standard_ChinaCdn`

### <a name="feedback"></a><span data-ttu-id="012e3-124">Comentarios</span><span class="sxs-lookup"><span data-stu-id="012e3-124">Feedback</span></span>
* <span data-ttu-id="012e3-125">Se ha cambiado `feedback` para mostrar los metadatos de los comandos ejecutados recientemente</span><span class="sxs-lookup"><span data-stu-id="012e3-125">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="012e3-126">Se ha cambiado `feedback` para pedir al usuario que abra un explorador y use una plantilla de incidencia para ayudar en el proceso de creación de la incidencia</span><span class="sxs-lookup"><span data-stu-id="012e3-126">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="012e3-127">Se ha cambiado `feedback` para imprimir el cuerpo de la incidencia cuando se ejecuta con "--verbose"</span><span class="sxs-lookup"><span data-stu-id="012e3-127">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-128">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-128">Monitor</span></span>
* <span data-ttu-id="012e3-129">Se ha corregido un problema por el que "count" no era un valor permitido con</span><span class="sxs-lookup"><span data-stu-id="012e3-129">Fixed issue where "count" was not a permitted value with</span></span> `metrics alert [create|update]` 

### <a name="network"></a><span data-ttu-id="012e3-130">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-130">Network</span></span>
* <span data-ttu-id="012e3-131">Se ha corregido un problema por el que no se mostraba el formato de tabla con</span><span class="sxs-lookup"><span data-stu-id="012e3-131">Fixed table format not displaying with</span></span> `vnet-gateway list-bgp-peer-status`
* <span data-ttu-id="012e3-132">Se han agregado los comandos `list-request-headers` y `list-response-headers` a</span><span class="sxs-lookup"><span data-stu-id="012e3-132">Added `list-request-headers` and `list-response-headers` commands to</span></span> `application-gateway rewrite-rule`
* <span data-ttu-id="012e3-133">Se ha agregado el comando `list-server-variables` a</span><span class="sxs-lookup"><span data-stu-id="012e3-133">Added `list-server-variables` command to</span></span> `application-gateway rewrite-rule condition`
* <span data-ttu-id="012e3-134">Se ha corregido un problema por el que la actualización del estado de vínculo de un puerto de ExpressRoute generaba una excepción de atributo desconocido</span><span class="sxs-lookup"><span data-stu-id="012e3-134">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception</span></span> `express-route port update`

### <a name="privatedns"></a><span data-ttu-id="012e3-135">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="012e3-135">PrivateDNS</span></span>
* <span data-ttu-id="012e3-136">Se ha agregado `network private-dns` para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="012e3-136">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-137">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-137">Resource</span></span>
* <span data-ttu-id="012e3-138">Se ha corregido el problema con `deployment create` y `group deployment create` por el que no funcionaba un archivo de parámetros con un conjunto de parámetros vacío</span><span class="sxs-lookup"><span data-stu-id="012e3-138">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="012e3-139">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-139">Role</span></span>
* <span data-ttu-id="012e3-140">Se ha corregido `create-for-rbac` para que trate `--years` correctamente</span><span class="sxs-lookup"><span data-stu-id="012e3-140">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="012e3-141">[CAMBIO IMPORTANTE] Se ha cambiado `role assignment delete` para preguntar cuando se eliminan todas las asignaciones de la suscripción de forma incondicional</span><span class="sxs-lookup"><span data-stu-id="012e3-141">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-142">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-142">SQL</span></span>
* <span data-ttu-id="012e3-143">Se ha actualizado `sql mi [create|update]` con las propiedades proxyOverride y publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="012e3-143">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-144">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-144">Storage</span></span>
* <span data-ttu-id="012e3-145">[CAMBIO IMPORTANTE] Se ha eliminado el resultado de</span><span class="sxs-lookup"><span data-stu-id="012e3-145">[BREAKING CHANGE] Removed result of</span></span> `storage blob delete`
* <span data-ttu-id="012e3-146">Se ha agregado `--full-uri` a `storage blob generate-sas` para crear el URI completo para el blob con SAS</span><span class="sxs-lookup"><span data-stu-id="012e3-146">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="012e3-147">Se ha agregado `--file-snapshot` a `storage file copy start` para copiar el archivo desde la instantánea</span><span class="sxs-lookup"><span data-stu-id="012e3-147">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="012e3-148">Se ha cambiado `storage blob copy cancel` para mostrar solo el error en lugar de la excepción para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="012e3-148">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="012e3-149">26 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-149">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="012e3-150">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-150">Core</span></span>
* <span data-ttu-id="012e3-151">Se han corregido problemas con la incompatibilidad de la extensión de desarrollo.</span><span class="sxs-lookup"><span data-stu-id="012e3-151">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="012e3-152">El control de errores ahora dirige a los clientes a la página de problemas.</span><span class="sxs-lookup"><span data-stu-id="012e3-152">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="012e3-153">Nube</span><span class="sxs-lookup"><span data-stu-id="012e3-153">Cloud</span></span>
* <span data-ttu-id="012e3-154">Se ha corregido un error de "suscripción no encontrada" en</span><span class="sxs-lookup"><span data-stu-id="012e3-154">Fixed a 'subscription not found' error in</span></span> `cloud set`

### <a name="acr"></a><span data-ttu-id="012e3-155">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-155">ACR</span></span>
* <span data-ttu-id="012e3-156">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="012e3-156">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="012e3-157">Se ha agregado `--auth-mode` a los comandos `acr build`, `acr run`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="012e3-157">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="012e3-158">Se ha agregado el grupo de comandos "acr task credential" para administrar las credenciales de una tarea.</span><span class="sxs-lookup"><span data-stu-id="012e3-158">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="012e3-159">Se ha agregado "--no-wait" al comando `acr build`.</span><span class="sxs-lookup"><span data-stu-id="012e3-159">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-160">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-160">AppService</span></span>
* <span data-ttu-id="012e3-161">Se ha corregido el error por el que `webapp up` no controlaba correctamente los escenarios de ejecución desde un directorio o de código desconocido.</span><span class="sxs-lookup"><span data-stu-id="012e3-161">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="012e3-162">Se ha corregido el error por el que los espacios no funcionaban para</span><span class="sxs-lookup"><span data-stu-id="012e3-162">Fixed bug where slots didn't work for</span></span> `[webapp|functionapp] config ssl bind`

### <a name="bot-service"></a><span data-ttu-id="012e3-163">Servicio BOT</span><span class="sxs-lookup"><span data-stu-id="012e3-163">BOT Service</span></span>
* <span data-ttu-id="012e3-164">Se ha agregado `bot prepare-deploy` para preparar la implementación de bots mediante</span><span class="sxs-lookup"><span data-stu-id="012e3-164">Added `bot prepare-deploy` to prepare for deploying bots via</span></span> `webapp`
* <span data-ttu-id="012e3-165">Se ha cambiado `bot create --kind registration` para que muestre la contraseña si no se proporciona una.</span><span class="sxs-lookup"><span data-stu-id="012e3-165">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="012e3-166">[CAMBIO IMPORTANTE] Se ha cambiado `--endpoint` en `bot create --kind registration` a que sea una cadena vacía de forma predeterminada en lugar de que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="012e3-166">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="012e3-167">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="012e3-167">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="012e3-168">CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-168">CDN</span></span>
* <span data-ttu-id="012e3-169">Se ha agregado compatibilidad para `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="012e3-169">Added support for `--no-wait` to</span></span> `cdn endpoint [create|update|start|stop|delete|load|purge]`  
* <span data-ttu-id="012e3-170">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento de almacenamiento de cadenas de consulta en caché predeterminado de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-170">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="012e3-171">El valor predeterminado ya no es "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="012e3-171">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="012e3-172">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="012e3-172">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="012e3-173">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="012e3-173">Cosmosdb</span></span>
* <span data-ttu-id="012e3-174">Se ha agregado compatibilidad con `--enable-multiple-write-locations` al actualizar la cuenta.</span><span class="sxs-lookup"><span data-stu-id="012e3-174">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="012e3-175">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="012e3-175">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-176">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-176">Interactive</span></span>
* <span data-ttu-id="012e3-177">Se ha corregido la incompatibilidad con la extensión interactiva instalada mediante azdev.</span><span class="sxs-lookup"><span data-stu-id="012e3-177">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-178">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-178">Monitor</span></span>
* <span data-ttu-id="012e3-179">Se ha cambiado para permitir el valor de dimensión `*` para</span><span class="sxs-lookup"><span data-stu-id="012e3-179">Changed to allow dimension value `*` for</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="012e3-180">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-180">Network</span></span>
* <span data-ttu-id="012e3-181">Se ha agregado el grupo de comandos `rewrite-rule` a</span><span class="sxs-lookup"><span data-stu-id="012e3-181">Added `rewrite-rule` command group to</span></span> `application-gateway`

### <a name="profile"></a><span data-ttu-id="012e3-182">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-182">Profile</span></span>
* <span data-ttu-id="012e3-183">Se ha agregado compatibilidad de la cuenta en el nivel de inquilino para la identidad de servicio administrada a</span><span class="sxs-lookup"><span data-stu-id="012e3-183">Added tenant level account support for managed service identity to</span></span> `login`

### <a name="postgres"></a><span data-ttu-id="012e3-184">Postgres</span><span class="sxs-lookup"><span data-stu-id="012e3-184">Postgres</span></span> 
* <span data-ttu-id="012e3-185">Se han agregado los comandos postgresql `replica` y el comando `restart server`.</span><span class="sxs-lookup"><span data-stu-id="012e3-185">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="012e3-186">Se ha cambiado para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="012e3-186">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-187">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-187">Resource</span></span>
* <span data-ttu-id="012e3-188">Se ha mejorado la salida de tabla de</span><span class="sxs-lookup"><span data-stu-id="012e3-188">Improved table output for</span></span> `deployment [create|list|show]`
* <span data-ttu-id="012e3-189">Se ha corregido el problema con `deployment [create|validate]` por el que no reconocía el tipo secureObject.</span><span class="sxs-lookup"><span data-stu-id="012e3-189">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="012e3-190">Grafo</span><span class="sxs-lookup"><span data-stu-id="012e3-190">Graph</span></span>
* <span data-ttu-id="012e3-191">Se ha agregado compatibilidad para `--end-date` a</span><span class="sxs-lookup"><span data-stu-id="012e3-191">Added support for `--end-date` to</span></span> `ad [app|sp] credential reset`
* <span data-ttu-id="012e3-192">Se ha agregado compatibilidad para agregar permisos con</span><span class="sxs-lookup"><span data-stu-id="012e3-192">Added support to add permissions with</span></span> `ad app permission add`
* <span data-ttu-id="012e3-193">Se ha corregido un error con `ad app permission list` cuando no había ningún permiso.</span><span class="sxs-lookup"><span data-stu-id="012e3-193">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="012e3-194">Se ha cambiado `ad sp delete` para omitir la eliminación de la asignación de roles si la cuenta actual no tiene ninguna suscripción.</span><span class="sxs-lookup"><span data-stu-id="012e3-194">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="012e3-195">Se ha cambiado `ad app create` para que `--identifier-uris` sea una lista vacía de forma predeterminada si no se proporciona.</span><span class="sxs-lookup"><span data-stu-id="012e3-195">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-196">storage</span><span class="sxs-lookup"><span data-stu-id="012e3-196">storage</span></span>
* <span data-ttu-id="012e3-197">Se ha agregado `--snapshot` a `storage file download-batch` para descargar desde una instantánea de recurso compartido.</span><span class="sxs-lookup"><span data-stu-id="012e3-197">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="012e3-198">Se ha cambiado la barra de progreso `storage blob [download-batch|upload-batch]` para que sea menos detallada y que indique el blob actual.</span><span class="sxs-lookup"><span data-stu-id="012e3-198">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="012e3-199">Se ha corregido el problema con `storage account update` al actualizar los parámetros de cifrado.</span><span class="sxs-lookup"><span data-stu-id="012e3-199">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="012e3-200">Se ha corregido el problema por el que `storage blob show` producía un error al usar oauth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="012e3-200">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-201">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-201">VM</span></span>
* <span data-ttu-id="012e3-202">Se agregó el comando `image update`.</span><span class="sxs-lookup"><span data-stu-id="012e3-202">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="012e3-203">12 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-203">March 12, 2019</span></span>

<span data-ttu-id="012e3-204">Versión 2.0.60</span><span class="sxs-lookup"><span data-stu-id="012e3-204">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="012e3-205">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-205">Core</span></span>

* <span data-ttu-id="012e3-206">Se ha corregido un error incorrecto en `cloud set` sobre la suscripción no encontrada.</span><span class="sxs-lookup"><span data-stu-id="012e3-206">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-207">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-207">ACR</span></span>

* <span data-ttu-id="012e3-208">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="012e3-208">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-209">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-209">ACS</span></span>

* <span data-ttu-id="012e3-210">Ahora, se omite el parámetro `--listen-address` de `aks browse` si kubectl no lo admite</span><span class="sxs-lookup"><span data-stu-id="012e3-210">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="012e3-211">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-211">AppService</span></span>

* <span data-ttu-id="012e3-212">Se ha agregado `[webapp|functionapp] deployment list-publishing-credentials` para obtener la dirección URL y sus credenciales de publicación de Kudu.</span><span class="sxs-lookup"><span data-stu-id="012e3-212">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="012e3-213">Se ha quitado la instrucción de impresión errónea para</span><span class="sxs-lookup"><span data-stu-id="012e3-213">Removed erroneous print statement for</span></span> `webapp auth update`
* <span data-ttu-id="012e3-214">Se ha corregido `functionapp` para establecer la imagen correcta en el entorno de ejecución en los planes de App Service de Linux</span><span class="sxs-lookup"><span data-stu-id="012e3-214">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="012e3-215">Se ha quitado la etiqueta de versión preliminar para `webapp up` y se han agregado mejoras al comando.</span><span class="sxs-lookup"><span data-stu-id="012e3-215">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="012e3-216">Botservice</span><span class="sxs-lookup"><span data-stu-id="012e3-216">Botservice</span></span>

* <span data-ttu-id="012e3-217">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="012e3-217">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="012e3-218">Se han agregado `Microsoft-BotFramework-AppId` y `Microsoft-BotFramework-AppPassword` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web</span><span class="sxs-lookup"><span data-stu-id="012e3-218">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="012e3-219">Se han quitado las comillas simples de la salida del comando `bot publish` al final de</span><span class="sxs-lookup"><span data-stu-id="012e3-219">Removed single quotes from `bot publish` command output at end of</span></span> `bot create`
* <span data-ttu-id="012e3-220">Se ha cambiado `bot publish` para que sea asincrónico.</span><span class="sxs-lookup"><span data-stu-id="012e3-220">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="012e3-221">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-221">Container</span></span>

* <span data-ttu-id="012e3-222">Se ha agregado el argumento `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="012e3-222">Added `--no-wait` argument to</span></span> `container [start|restart]`

### <a name="eventhub"></a><span data-ttu-id="012e3-223">EventHub</span><span class="sxs-lookup"><span data-stu-id="012e3-223">EventHub</span></span>

* <span data-ttu-id="012e3-224">Se ha agregado la marca `--skip-empty-archives` a `eventhub create|update` para admitir archivos vacíos en la captura.</span><span class="sxs-lookup"><span data-stu-id="012e3-224">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="012e3-225">Buscar</span><span class="sxs-lookup"><span data-stu-id="012e3-225">Find</span></span>

* <span data-ttu-id="012e3-226">Actualización de la funcionalidad principal</span><span class="sxs-lookup"><span data-stu-id="012e3-226">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="012e3-227">HDInsight</span><span class="sxs-lookup"><span data-stu-id="012e3-227">HDInsight</span></span>

* <span data-ttu-id="012e3-228">Se ha agregado el parámetro `--storage-account-managed-identity` a `hdinsight create` para admitir MSI de ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="012e3-228">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="012e3-229">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-229">Network</span></span>

* <span data-ttu-id="012e3-230">Se ha corregido un problema con `vpn-connection update` por el que no se podía actualizar una conexión VPN entre pasarelas de diferentes suscripciones.</span><span class="sxs-lookup"><span data-stu-id="012e3-230">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="012e3-231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="012e3-231">Rdbms</span></span>

* <span data-ttu-id="012e3-232">Correcciones menores para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="012e3-232">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="012e3-233">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-233">Role</span></span>

* <span data-ttu-id="012e3-234">Se ha corregido `role definition update` para usar el identificador para resolver la definición correctamente.</span><span class="sxs-lookup"><span data-stu-id="012e3-234">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="012e3-235">Se ha cambiado `ad app credential reset` para eliminar la suposición de que la entidad de servicio de la aplicación siempre existe.</span><span class="sxs-lookup"><span data-stu-id="012e3-235">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="012e3-236">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="012e3-236">Service Fabric</span></span>

* <span data-ttu-id="012e3-237">Se ha corregido un problema con `sf cluster list` que no se podía iterar.</span><span class="sxs-lookup"><span data-stu-id="012e3-237">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="012e3-238">26 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-238">February 26, 2019</span></span>

<span data-ttu-id="012e3-239">Versión 2.0.59</span><span class="sxs-lookup"><span data-stu-id="012e3-239">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="012e3-240">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-240">Core</span></span>

* <span data-ttu-id="012e3-241">Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.</span><span class="sxs-lookup"><span data-stu-id="012e3-241">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-242">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-242">ACR</span></span>

* <span data-ttu-id="012e3-243">Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="012e3-243">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="012e3-244">Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.</span><span class="sxs-lookup"><span data-stu-id="012e3-244">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-245">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-245">ACS</span></span>

* <span data-ttu-id="012e3-246">Se ha agregado la opción `--listen-address` a</span><span class="sxs-lookup"><span data-stu-id="012e3-246">Added `--listen-address` option to</span></span> `aks port-forward`

### <a name="appservice"></a><span data-ttu-id="012e3-247">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-247">AppService</span></span>

* <span data-ttu-id="012e3-248">Se agregó el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="012e3-248">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-249">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-249">Batch</span></span>
* <span data-ttu-id="012e3-250">[CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="012e3-250">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="012e3-251">[CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.</span><span class="sxs-lookup"><span data-stu-id="012e3-251">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="012e3-252">Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="012e3-252">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="012e3-253">[CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`.</span><span class="sxs-lookup"><span data-stu-id="012e3-253">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="012e3-254">Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.</span><span class="sxs-lookup"><span data-stu-id="012e3-254">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="012e3-255">Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.</span><span class="sxs-lookup"><span data-stu-id="012e3-255">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="012e3-256">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-256">CosmosDB</span></span>

* <span data-ttu-id="012e3-257">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="012e3-257">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="012e3-258">Kusto</span><span class="sxs-lookup"><span data-stu-id="012e3-258">Kusto</span></span>

* <span data-ttu-id="012e3-259">[CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.</span><span class="sxs-lookup"><span data-stu-id="012e3-259">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="012e3-260">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-260">Network</span></span>

* <span data-ttu-id="012e3-261">Se ha agregado el argumento `--express-route-gateway-bypass`</span><span class="sxs-lookup"><span data-stu-id="012e3-261">Added `--express-route-gateway-bypass` argument to</span></span> `vpn-connection [create|update]`
* <span data-ttu-id="012e3-262">Se han agregado grupos de comandos desde extensiones `express-route`.</span><span class="sxs-lookup"><span data-stu-id="012e3-262">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="012e3-263">Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="012e3-263">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="012e3-264">Se ha agregado el argumento `--legacy-mode` a</span><span class="sxs-lookup"><span data-stu-id="012e3-264">Added argument `--legacy-mode` to</span></span> `express-route peering [create|update]` 
* <span data-ttu-id="012e3-265">Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a</span><span class="sxs-lookup"><span data-stu-id="012e3-265">Added arguments `--allow-classic-operations` and `--express-route-port` to</span></span> `express-route [create|update]`
* <span data-ttu-id="012e3-266">Se ha agregado el argumento `--gateway-default-site` a</span><span class="sxs-lookup"><span data-stu-id="012e3-266">Added `--gateway-default-site` argument to</span></span> `vnet-gateway [create|update]`
* <span data-ttu-id="012e3-267">Se han agregado comandos `ipsec-policy` a</span><span class="sxs-lookup"><span data-stu-id="012e3-267">Added `ipsec-policy` commands to</span></span> `vnet-gateway`

### <a name="resource"></a><span data-ttu-id="012e3-268">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-268">Resource</span></span>

* <span data-ttu-id="012e3-269">Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="012e3-269">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="012e3-270">Se ha agregado compatibilidad para el archivo de parámetros basado en URI a</span><span class="sxs-lookup"><span data-stu-id="012e3-270">Added support for URI-based parameters file to</span></span> `policy assignment create`
* <span data-ttu-id="012e3-271">Se ha agregado compatibilidad para definiciones y parámetros basados en URI para</span><span class="sxs-lookup"><span data-stu-id="012e3-271">Added support for URI-based parameters and definitions to</span></span> `policy set-definition update`
* <span data-ttu-id="012e3-272">Se ha corregido el control de parámetros y reglas para</span><span class="sxs-lookup"><span data-stu-id="012e3-272">Fixed handling of parameters and rules for</span></span> `policy definition update`
* <span data-ttu-id="012e3-273">Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.</span><span class="sxs-lookup"><span data-stu-id="012e3-273">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="012e3-274">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-274">Role</span></span>

* <span data-ttu-id="012e3-275">Se ha agregado compatibilidad con roles de aplicación a</span><span class="sxs-lookup"><span data-stu-id="012e3-275">Added support for app roles to</span></span> `ad app [create|update]`

### <a name="vm"></a><span data-ttu-id="012e3-276">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-276">VM</span></span>

* <span data-ttu-id="012e3-277">Se ha corregido un problema con `vm create where `--acelerated-networking\` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="012e3-277">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="012e3-278">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-278">February 12, 2019</span></span>

<span data-ttu-id="012e3-279">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="012e3-279">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="012e3-280">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-280">Core</span></span>

* `az --version` <span data-ttu-id="012e3-281">ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="012e3-281">now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="012e3-282">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="012e3-282">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-283">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-283">ACR</span></span>
* <span data-ttu-id="012e3-284">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="012e3-284">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="012e3-285">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de</span><span class="sxs-lookup"><span data-stu-id="012e3-285">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from</span></span> `acr repository delete`

### <a name="acs"></a><span data-ttu-id="012e3-286">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-286">ACS</span></span>
* <span data-ttu-id="012e3-287">Se ha agregado compatibilidad para que no distinga mayúsculas y minúsculas en los nombres a</span><span class="sxs-lookup"><span data-stu-id="012e3-287">Added support for case-insensitive names to</span></span> `aks [enable-addons|disable-addons]`
* <span data-ttu-id="012e3-288">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante</span><span class="sxs-lookup"><span data-stu-id="012e3-288">Added support for Azure Active Directory updating operation using</span></span> `aks update-credentials --reset-aad`
* <span data-ttu-id="012e3-289">Se ha incluido una aclaración de que `--output` se omite para</span><span class="sxs-lookup"><span data-stu-id="012e3-289">Added clarification that `--output` is ignored for</span></span> `aks get-credentials`

### <a name="ams"></a><span data-ttu-id="012e3-290">AMS</span><span class="sxs-lookup"><span data-stu-id="012e3-290">AMS</span></span>
* <span data-ttu-id="012e3-291">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="012e3-291">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="012e3-292">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="012e3-292">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-293">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-293">Appservice</span></span>
* <span data-ttu-id="012e3-294">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="012e3-294">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="012e3-295">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="012e3-295">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="012e3-296">Se ha mejorado la ayuda de</span><span class="sxs-lookup"><span data-stu-id="012e3-296">Improved help for</span></span> `appservice-plan-update`
* <span data-ttu-id="012e3-297">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="012e3-297">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="012e3-298">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="012e3-298">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="012e3-299">Botservice</span><span class="sxs-lookup"><span data-stu-id="012e3-299">Botservice</span></span>
* <span data-ttu-id="012e3-300">Se ha mejorado la experiencia de usuario de</span><span class="sxs-lookup"><span data-stu-id="012e3-300">Improved UX for</span></span> `bot publish`
* <span data-ttu-id="012e3-301">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante</span><span class="sxs-lookup"><span data-stu-id="012e3-301">Added warning for timeouts when running `npm install` during</span></span> `az bot publish`
* <span data-ttu-id="012e3-302">Se han quitado caracteres no válidos `.` de `--name` en</span><span class="sxs-lookup"><span data-stu-id="012e3-302">Removed invalid char `.` from `--name`  in</span></span> `az bot create`
* <span data-ttu-id="012e3-303">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="012e3-303">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="012e3-304">[EN DESUSO] Se ha dejado de usar el argumento `--proj-name` en favor de</span><span class="sxs-lookup"><span data-stu-id="012e3-304">[DEPRECATED] Deprecated `--proj-name` argument in favor of</span></span> `--proj-file-path`
* <span data-ttu-id="012e3-305">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="012e3-305">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="012e3-306">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="012e3-306">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="012e3-307">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="012e3-307">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="012e3-308">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="012e3-308">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="012e3-309">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="012e3-309">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="012e3-310">Key Vault</span><span class="sxs-lookup"><span data-stu-id="012e3-310">Key Vault</span></span>
* <span data-ttu-id="012e3-311">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban</span><span class="sxs-lookup"><span data-stu-id="012e3-311">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using</span></span> `--id`

### <a name="monitor"></a><span data-ttu-id="012e3-312">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-312">Monitor</span></span>
* <span data-ttu-id="012e3-313">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión</span><span class="sxs-lookup"><span data-stu-id="012e3-313">Changed `monitor metrics alert [create|update]` to allow dimension value</span></span> `*`

### <a name="network"></a><span data-ttu-id="012e3-314">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-314">Network</span></span>
* <span data-ttu-id="012e3-315">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="012e3-315">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="012e3-316">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="012e3-316">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="012e3-317">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="012e3-317">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="012e3-318">Se ha agregado `--idle-timeout` y `--floating-ip` a</span><span class="sxs-lookup"><span data-stu-id="012e3-318">Added `--idle-timeout` and `--floating-ip` to</span></span> `lb inbound-nat-pool [create|update]`

### <a name="policy-insights"></a><span data-ttu-id="012e3-319">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="012e3-319">Policy Insights</span></span>
* <span data-ttu-id="012e3-320">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="012e3-320">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="012e3-321">RDBMS</span><span class="sxs-lookup"><span data-stu-id="012e3-321">RDBMS</span></span>
* <span data-ttu-id="012e3-322">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="012e3-322">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="012e3-323">Redis</span><span class="sxs-lookup"><span data-stu-id="012e3-323">Redis</span></span>
* <span data-ttu-id="012e3-324">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="012e3-324">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="012e3-325">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="012e3-325">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="012e3-326">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="012e3-326">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="012e3-327">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="012e3-327">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="012e3-328">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="012e3-328">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="012e3-329">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="012e3-329">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="012e3-330">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="012e3-330">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="012e3-331">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-331">Role</span></span>
* <span data-ttu-id="012e3-332">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="012e3-332">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="012e3-333">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-333">SQL VM</span></span>
* <span data-ttu-id="012e3-334">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="012e3-334">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-335">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-335">VM</span></span>
* <span data-ttu-id="012e3-336">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de</span><span class="sxs-lookup"><span data-stu-id="012e3-336">Changed `vm list-skus` to allow use of `--all` in place of</span></span> `--all true`
* <span data-ttu-id="012e3-337">Se agregó</span><span class="sxs-lookup"><span data-stu-id="012e3-337">Added</span></span> `vmss run-command [invoke | list | show]`
* <span data-ttu-id="012e3-338">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="012e3-338">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="012e3-339">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="012e3-339">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="012e3-340">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-340">January 31, 2019</span></span>

<span data-ttu-id="012e3-341">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="012e3-341">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="012e3-342">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-342">Core</span></span>

* <span data-ttu-id="012e3-343">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="012e3-343">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="012e3-344">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-344">January 28, 2019</span></span>

<span data-ttu-id="012e3-345">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="012e3-345">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-346">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-346">ACR</span></span>
* <span data-ttu-id="012e3-347">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="012e3-347">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-348">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-348">ACS</span></span>
* <span data-ttu-id="012e3-349">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="012e3-349">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="012e3-350">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="012e3-350">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="012e3-351">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con</span><span class="sxs-lookup"><span data-stu-id="012e3-351">Added support for service principal updates operation with</span></span> `aks update-credentials -reset-service-principal`

### <a name="ams"></a><span data-ttu-id="012e3-352">AMS</span><span class="sxs-lookup"><span data-stu-id="012e3-352">AMS</span></span>
* <span data-ttu-id="012e3-353">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a</span><span class="sxs-lookup"><span data-stu-id="012e3-353">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to</span></span> `ams asset list-streaming-locators`
* <span data-ttu-id="012e3-354">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a</span><span class="sxs-lookup"><span data-stu-id="012e3-354">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to</span></span> `ams streaming-locator list-content-keys`

### <a name="appservice"></a><span data-ttu-id="012e3-355">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-355">Appservice</span></span>
* <span data-ttu-id="012e3-356">Se ha agregado compatibilidad para App Insights en</span><span class="sxs-lookup"><span data-stu-id="012e3-356">Added support for app insights on</span></span> `functionapp create`
* <span data-ttu-id="012e3-357">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="012e3-357">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="012e3-358">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="012e3-358">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="012e3-359">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-359">Container</span></span>
* <span data-ttu-id="012e3-360">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="012e3-360">Added `container start` command</span></span>
* <span data-ttu-id="012e3-361">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="012e3-361">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="012e3-362">EventGrid</span><span class="sxs-lookup"><span data-stu-id="012e3-362">EventGrid</span></span>
* <span data-ttu-id="012e3-363">Se ha agregado el parámetro `--deadletter-endpoint` a</span><span class="sxs-lookup"><span data-stu-id="012e3-363">Added `--deadletter-endpoint` parameter to</span></span> `event-subscription [create|update]`
* <span data-ttu-id="012e3-364">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="012e3-364">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="012e3-365">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="012e3-365">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="012e3-366">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="012e3-366">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="012e3-367">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="012e3-367">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="012e3-368">HDInsight</span><span class="sxs-lookup"><span data-stu-id="012e3-368">HDInsight</span></span>
* <span data-ttu-id="012e3-369">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en</span><span class="sxs-lookup"><span data-stu-id="012e3-369">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from</span></span> `hdinsight [application] create`
* <span data-ttu-id="012e3-370">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="012e3-370">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="012e3-371">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a</span><span class="sxs-lookup"><span data-stu-id="012e3-371">Added `--vnet-name` and `--subnet-name` parameters to</span></span> `hdinsight create`
* <span data-ttu-id="012e3-372">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a</span><span class="sxs-lookup"><span data-stu-id="012e3-372">Added support for Enterprise Security Package and disk encryption to</span></span> `hdinsight create` 
* <span data-ttu-id="012e3-373">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="012e3-373">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="012e3-374">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="012e3-374">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-375">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-375">IoT</span></span>
* <span data-ttu-id="012e3-376">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="012e3-376">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="012e3-377">Kusto</span><span class="sxs-lookup"><span data-stu-id="012e3-377">Kusto</span></span>
* <span data-ttu-id="012e3-378">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-378">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-379">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-379">Monitor</span></span>
* <span data-ttu-id="012e3-380">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="012e3-380">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="012e3-381">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-381">Profile</span></span>
* <span data-ttu-id="012e3-382">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de</span><span class="sxs-lookup"><span data-stu-id="012e3-382">Enable tenant level account for managed service identity for</span></span> `login`

### <a name="network"></a><span data-ttu-id="012e3-383">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-383">Network</span></span>
* <span data-ttu-id="012e3-384">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="012e3-384">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="012e3-385">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="012e3-385">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-386">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-386">Resource</span></span>
* <span data-ttu-id="012e3-387">Se ha agregado compatibilidad para el archivo de parámetros URI a</span><span class="sxs-lookup"><span data-stu-id="012e3-387">Added support for URI parameters file to</span></span> `group deployment create`
* <span data-ttu-id="012e3-388">Se ha agregado compatibilidad para identidades administradas a</span><span class="sxs-lookup"><span data-stu-id="012e3-388">Added support for managed identity to</span></span> `policy assignment [create|list|show]`

### <a name="sql-virtual-machine"></a><span data-ttu-id="012e3-389">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-389">SQL Virtual Machine</span></span>
* <span data-ttu-id="012e3-390">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-390">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-391">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-391">Storage</span></span>
* <span data-ttu-id="012e3-392">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="012e3-392">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="012e3-393">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="012e3-393">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-394">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-394">VM</span></span>
* <span data-ttu-id="012e3-395">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="012e3-395">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="012e3-396">Se ha agregado la marca `--force` a</span><span class="sxs-lookup"><span data-stu-id="012e3-396">Added `--force` flag to</span></span> `vm encryption enable`

## <a name="january-15-2019"></a><span data-ttu-id="012e3-397">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="012e3-397">January 15, 2019</span></span>

<span data-ttu-id="012e3-398">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="012e3-398">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-399">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-399">ACR</span></span>
* <span data-ttu-id="012e3-400">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="012e3-400">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="012e3-401">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="012e3-401">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="012e3-402">[EN DESUSO] Se ha dejado de usar el parámetro `--resource-group` en los comandos:</span><span class="sxs-lookup"><span data-stu-id="012e3-402">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="012e3-403">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-403">ACS</span></span>
* <span data-ttu-id="012e3-404">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="012e3-404">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-405">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-405">Appservice</span></span>
* <span data-ttu-id="012e3-406">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="012e3-406">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="012e3-407">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="012e3-407">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="012e3-408">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="012e3-408">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="012e3-409">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="012e3-409">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="012e3-410">Botservice</span><span class="sxs-lookup"><span data-stu-id="012e3-410">Botservice</span></span>
* <span data-ttu-id="012e3-411">Se han agregado actualizaciones al estado de implementación a</span><span class="sxs-lookup"><span data-stu-id="012e3-411">Added deployment status updates to</span></span> `bot create`

### <a name="configure"></a><span data-ttu-id="012e3-412">Configuración</span><span class="sxs-lookup"><span data-stu-id="012e3-412">Configure</span></span>
* <span data-ttu-id="012e3-413">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="012e3-413">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="012e3-414">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-414">CosmosDB</span></span>
* <span data-ttu-id="012e3-415">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="012e3-415">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="012e3-416">HDInsight</span><span class="sxs-lookup"><span data-stu-id="012e3-416">HDInsight</span></span>
* <span data-ttu-id="012e3-417">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="012e3-417">Added commands for managing applications</span></span>
* <span data-ttu-id="012e3-418">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="012e3-418">Added commands for managing script actions</span></span>
* <span data-ttu-id="012e3-419">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="012e3-419">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="012e3-420">Se ha agregado compatibilidad para enumerar el uso regional a</span><span class="sxs-lookup"><span data-stu-id="012e3-420">Added support to list regional usage to</span></span> `hdinsight list-usage`
* <span data-ttu-id="012e3-421">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de</span><span class="sxs-lookup"><span data-stu-id="012e3-421">[BREAKING CHANGE] Removed default cluster type from</span></span> `hdinsight create`

### <a name="network"></a><span data-ttu-id="012e3-422">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-422">Network</span></span>
* <span data-ttu-id="012e3-423">Se han agregado los argumentos `--custom-headers` y `--status-code-ranges` a</span><span class="sxs-lookup"><span data-stu-id="012e3-423">Added `--custom-headers` and `--status-code-ranges` arguments to</span></span> `traffic-manager profile [create|update]`
* <span data-ttu-id="012e3-424">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="012e3-424">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="012e3-425">Se agregaron los argumentos `--custom-headers` y `--subnets` a</span><span class="sxs-lookup"><span data-stu-id="012e3-425">Added `--custom-headers` and `--subnets` arguments to</span></span> `traffic-manager endpoint [create|update]`  
* <span data-ttu-id="012e3-426">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="012e3-426">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="012e3-427">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-427">Role</span></span>
* <span data-ttu-id="012e3-428">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="012e3-428">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="012e3-429">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="012e3-429">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="012e3-430">Seguridad</span><span class="sxs-lookup"><span data-stu-id="012e3-430">Security</span></span>
* <span data-ttu-id="012e3-431">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="012e3-431">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-432">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-432">Storage</span></span>
* <span data-ttu-id="012e3-433">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="012e3-433">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="012e3-434">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="012e3-434">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="012e3-435">Se ha agregado el parámetro `--marker` a</span><span class="sxs-lookup"><span data-stu-id="012e3-435">Added `--marker` parameter to</span></span> `storage [blob|file|container|share] list`
* <span data-ttu-id="012e3-436">Se ha agregado un marcador de registro para página siguiente en STDERR para</span><span class="sxs-lookup"><span data-stu-id="012e3-436">Added log marker for next page to STDERR for</span></span> `storage [blob|file|container|share] list` 
* <span data-ttu-id="012e3-437">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="012e3-437">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-438">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-438">VM</span></span>
* <span data-ttu-id="012e3-439">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="012e3-439">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="012e3-440">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a</span><span class="sxs-lookup"><span data-stu-id="012e3-440">Added support for cross tenant image referencing to</span></span> `[vm|vmss] create`
* <span data-ttu-id="012e3-441">Se ha corregido el error con la configuración predeterminada de</span><span class="sxs-lookup"><span data-stu-id="012e3-441">Fixed bug with default configuration in</span></span> `vm diagnostics get-default-config --windows-os`
* <span data-ttu-id="012e3-442">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="012e3-442">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="012e3-443">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="012e3-443">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="012e3-444">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="012e3-444">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="012e3-445">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-445">December 20, 2018</span></span>

<span data-ttu-id="012e3-446">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="012e3-446">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="012e3-447">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-447">Appservice</span></span>
* <span data-ttu-id="012e3-448">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="012e3-448">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="012e3-449">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="012e3-449">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="012e3-450">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="012e3-450">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="012e3-451">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="012e3-451">IoTCentral</span></span>
* <span data-ttu-id="012e3-452">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="012e3-452">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="012e3-453">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-453">Role</span></span>
* <span data-ttu-id="012e3-454">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="012e3-454">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-455">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-455">SQL</span></span>
* <span data-ttu-id="012e3-456">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="012e3-456">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-457">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-457">VM</span></span>
* <span data-ttu-id="012e3-458">Se ha agregado el parámetro `---os-type` a</span><span class="sxs-lookup"><span data-stu-id="012e3-458">Added `---os-type` parameter to</span></span> `disk create`

## <a name="december-18-2018"></a><span data-ttu-id="012e3-459">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-459">December 18, 2018</span></span>

<span data-ttu-id="012e3-460">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="012e3-460">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="012e3-461">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-461">ACR</span></span>
* <span data-ttu-id="012e3-462">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="012e3-462">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="012e3-463">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="012e3-463">Condensed the table layout for task list</span></span>
* <span data-ttu-id="012e3-464">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="012e3-464">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-465">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-465">ACS</span></span>
* <span data-ttu-id="012e3-466">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="012e3-466">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="012e3-467">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a</span><span class="sxs-lookup"><span data-stu-id="012e3-467">Removed "(PREVIEW)" from AAD arguments to</span></span> `aks create`
* <span data-ttu-id="012e3-468">[EN DESUSO] Se han dejado de usar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="012e3-468">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="012e3-469">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="012e3-469">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="012e3-470">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="012e3-470">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="012e3-471">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="012e3-471">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-472">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-472">Appservice</span></span>
* <span data-ttu-id="012e3-473">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="012e3-473">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="012e3-474">Botservice</span><span class="sxs-lookup"><span data-stu-id="012e3-474">Botservice</span></span>
* <span data-ttu-id="012e3-475">Se ha agregado compatibilidad con el análisis de archivos `.bot` al llamar a</span><span class="sxs-lookup"><span data-stu-id="012e3-475">Added support for `.bot` file parsing when calling</span></span> `bot show`
* <span data-ttu-id="012e3-476">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="012e3-476">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="012e3-477">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="012e3-477">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="012e3-478">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="012e3-478">Reduced Kudu network calls</span></span>
* <span data-ttu-id="012e3-479">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="012e3-479">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="012e3-480">Consumo</span><span class="sxs-lookup"><span data-stu-id="012e3-480">Consumption</span></span>
* <span data-ttu-id="012e3-481">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="012e3-481">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="012e3-482">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-482">CosmosDB</span></span>
* <span data-ttu-id="012e3-483">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="012e3-483">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="012e3-484">Mapas</span><span class="sxs-lookup"><span data-stu-id="012e3-484">Maps</span></span>
* <span data-ttu-id="012e3-485">Se ha agregado compatibilidad para la SKU S1 a</span><span class="sxs-lookup"><span data-stu-id="012e3-485">Added support for the S1 SKU to</span></span> `maps account [create|update]`

### <a name="network"></a><span data-ttu-id="012e3-486">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-486">Network</span></span>
* <span data-ttu-id="012e3-487">Se ha agregado compatibilidad para `--format` y `--log-version` a</span><span class="sxs-lookup"><span data-stu-id="012e3-487">Added support for `--format` and `--log-version` to</span></span> `watcher flow-log configure`
* <span data-ttu-id="012e3-488">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="012e3-488">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-489">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-489">Resource</span></span>
* <span data-ttu-id="012e3-490">Se ha corregido el control del parámetro de ámbito para los grupos de administración en</span><span class="sxs-lookup"><span data-stu-id="012e3-490">Fixed handling of scope parameter for management groups in</span></span> `policy assignment [create|list|delete|show|update]` 
* <span data-ttu-id="012e3-491">Se ha agregado un nuevo comando</span><span class="sxs-lookup"><span data-stu-id="012e3-491">Added new command</span></span> `resource wait`

### <a name="storage"></a><span data-ttu-id="012e3-492">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-492">Storage</span></span>
*  <span data-ttu-id="012e3-493">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en</span><span class="sxs-lookup"><span data-stu-id="012e3-493">Added ability to update log schema version for storage services in</span></span> `storage logging update`

### <a name="vm"></a><span data-ttu-id="012e3-494">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-494">VM</span></span>
* <span data-ttu-id="012e3-495">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="012e3-495">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="012e3-496">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-496">December 4, 2018</span></span>

<span data-ttu-id="012e3-497">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="012e3-497">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="012e3-498">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-498">Core</span></span>
* <span data-ttu-id="012e3-499">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="012e3-499">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="012e3-500">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="012e3-500">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-501">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-501">Appservice</span></span>
* <span data-ttu-id="012e3-502">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="012e3-502">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="012e3-503">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="012e3-503">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="012e3-504">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-504">Network</span></span>
* <span data-ttu-id="012e3-505">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="012e3-505">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="012e3-506">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-506">Role</span></span>
* <span data-ttu-id="012e3-507">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="012e3-507">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="012e3-508">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-508">VM</span></span>
* <span data-ttu-id="012e3-509">[EN DESUSO] Se ha dejado de usar el parámetro `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="012e3-509">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="012e3-510">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="012e3-510">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="012e3-511">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="012e3-511">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="012e3-512">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="012e3-512">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="012e3-513">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-513">November 20, 2018</span></span>

<span data-ttu-id="012e3-514">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="012e3-514">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="012e3-515">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-515">Core</span></span>
* <span data-ttu-id="012e3-516">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="012e3-516">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-517">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-517">ACR</span></span>
* <span data-ttu-id="012e3-518">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="012e3-518">Added context token to task step</span></span>
* <span data-ttu-id="012e3-519">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="012e3-519">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="012e3-520">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="012e3-520">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-521">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-521">Appservice</span></span>
* <span data-ttu-id="012e3-522">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="012e3-522">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="012e3-523">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="012e3-523">Updated the default `node_version`.</span></span> <span data-ttu-id="012e3-524">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="012e3-524">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="012e3-525">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="012e3-525">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="012e3-526">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="012e3-526">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="012e3-527">IotCentral</span><span class="sxs-lookup"><span data-stu-id="012e3-527">IotCentral</span></span>
* <span data-ttu-id="012e3-528">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="012e3-528">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-529">KeyVault</span><span class="sxs-lookup"><span data-stu-id="012e3-529">KeyVault</span></span>
* <span data-ttu-id="012e3-530">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="012e3-530">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="012e3-531">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-531">Network</span></span>
* <span data-ttu-id="012e3-532">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="012e3-532">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="012e3-533">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="012e3-533">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="012e3-534">Se ha agregado `--zones` para compatibilidad con la zona de disponibilidad a</span><span class="sxs-lookup"><span data-stu-id="012e3-534">Added `--zones` for availability zone support to</span></span> `application-gateway create` 
* <span data-ttu-id="012e3-535">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a</span><span class="sxs-lookup"><span data-stu-id="012e3-535">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to</span></span> `application-gateway waf-config set`

### <a name="rdbms"></a><span data-ttu-id="012e3-536">Rdbms</span><span class="sxs-lookup"><span data-stu-id="012e3-536">Rdbms</span></span>
* <span data-ttu-id="012e3-537">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="012e3-537">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="012e3-538">Rbac</span><span class="sxs-lookup"><span data-stu-id="012e3-538">Rbac</span></span>
* <span data-ttu-id="012e3-539">Se ha corregido un problema al intentar actualizar credenciales inmutables en</span><span class="sxs-lookup"><span data-stu-id="012e3-539">Fixed an issue with attempting to update immutable credentials in</span></span> `ad app update`
* <span data-ttu-id="012e3-540">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para</span><span class="sxs-lookup"><span data-stu-id="012e3-540">Added output warnings to communicate breaking changes in the near future for</span></span> `ad [app|sp] list` 

### <a name="storage"></a><span data-ttu-id="012e3-541">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-541">Storage</span></span>
* <span data-ttu-id="012e3-542">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="012e3-542">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="012e3-543">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="012e3-543">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="012e3-544">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="012e3-544">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="012e3-545">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="012e3-545">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-546">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-546">VM</span></span>
* <span data-ttu-id="012e3-547">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="012e3-547">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="012e3-548">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser</span><span class="sxs-lookup"><span data-stu-id="012e3-548">Changed version name parameters to `sig image-version` to be</span></span> `--image-version -e`
* <span data-ttu-id="012e3-549">Se ha dejado de usar el `sig image-version` argumento `--image-version-name` y se ha reemplazado por</span><span class="sxs-lookup"><span data-stu-id="012e3-549">Deprecated `sig image-version` argument `--image-version-name`, replaced by</span></span> `--image-version`
* <span data-ttu-id="012e3-550">Se ha agregado compatibilidad para usar el disco local del sistema operativo en</span><span class="sxs-lookup"><span data-stu-id="012e3-550">Added support to use local OS disk to</span></span> `[vm|vmss] create --ephemeral-os-disk`
* <span data-ttu-id="012e3-551">Se ha agregado compatibilidad para `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="012e3-551">Added support for `--no-wait` to</span></span> `snapshot create/update`
* <span data-ttu-id="012e3-552">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="012e3-552">Added `snapshot wait` command</span></span>
* <span data-ttu-id="012e3-553">Se ha agregado compatibilidad para usar el nombre de instancia con</span><span class="sxs-lookup"><span data-stu-id="012e3-553">Added support for using instance name with</span></span> `[vm|vmss] extension set --extension-instance-name`

## <a name="november-6-2018"></a><span data-ttu-id="012e3-554">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-554">November 6, 2018</span></span>

<span data-ttu-id="012e3-555">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="012e3-555">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="012e3-556">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-556">Core</span></span>
* <span data-ttu-id="012e3-557">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="012e3-557">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-558">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-558">ACR</span></span>
* <span data-ttu-id="012e3-559">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="012e3-559">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="012e3-560">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="012e3-560">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-561">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-561">ACS</span></span>
* <span data-ttu-id="012e3-562">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="012e3-562">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="012e3-563">Advisor</span><span class="sxs-lookup"><span data-stu-id="012e3-563">Advisor</span></span>
* <span data-ttu-id="012e3-564">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="012e3-564">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="012e3-565">AMS</span><span class="sxs-lookup"><span data-stu-id="012e3-565">AMS</span></span>
* <span data-ttu-id="012e3-566">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="012e3-566">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="012e3-567">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="012e3-567">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="012e3-568">Se ha agregado compatibilidad con los parámetros de cifrado a</span><span class="sxs-lookup"><span data-stu-id="012e3-568">Added encryption parameters support to</span></span> `ams streaming-policy create`
* <span data-ttu-id="012e3-569">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-569">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="012e3-570">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="012e3-570">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="012e3-571">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="012e3-571">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="012e3-572">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="012e3-572">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="012e3-573">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por</span><span class="sxs-lookup"><span data-stu-id="012e3-573">[BREAKING CHANGE] Replaced `ams streaming locator` command with</span></span> `ams streaming-locator`
* <span data-ttu-id="012e3-574">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de</span><span class="sxs-lookup"><span data-stu-id="012e3-574">[BREAKING CHANGE] Updated `--content-keys` argument of</span></span> `ams streaming locator`
* <span data-ttu-id="012e3-575">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="012e3-575">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="012e3-576">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por</span><span class="sxs-lookup"><span data-stu-id="012e3-576">[BREAKING CHANGE] Replaced `ams streaming policy` command with</span></span> `ams streaming-policy`
* <span data-ttu-id="012e3-577">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="012e3-577">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="012e3-578">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="012e3-578">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="012e3-579">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="012e3-579">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="012e3-580">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="012e3-580">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="012e3-581">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="012e3-581">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="012e3-582">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="012e3-582">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-583">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-583">AppService</span></span>
* <span data-ttu-id="012e3-584">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="012e3-584">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="012e3-585">Configuración</span><span class="sxs-lookup"><span data-stu-id="012e3-585">Configure</span></span>
* <span data-ttu-id="012e3-586">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="012e3-586">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="012e3-587">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-587">Container</span></span>
* <span data-ttu-id="012e3-588">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="012e3-588">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="012e3-589">EventHub</span><span class="sxs-lookup"><span data-stu-id="012e3-589">EventHub</span></span>
* <span data-ttu-id="012e3-590">Se ha agregado la marca `--enable-kafka` para admitir Kafka en</span><span class="sxs-lookup"><span data-stu-id="012e3-590">Added `--enable-kafka` flag to support Kafka in</span></span> `eventhub namespace [create|update]`

### <a name="interactive"></a><span data-ttu-id="012e3-591">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-591">Interactive</span></span>
* <span data-ttu-id="012e3-592">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="012e3-592">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-593">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-593">Monitor</span></span>
* <span data-ttu-id="012e3-594">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en</span><span class="sxs-lookup"><span data-stu-id="012e3-594">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="012e3-595">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-595">Network</span></span>
* <span data-ttu-id="012e3-596">Se han dejado de utilizar los nombres de comando `network interface-endpoint` en favor de</span><span class="sxs-lookup"><span data-stu-id="012e3-596">Deprecated `network interface-endpoint` command names in favor of</span></span> `network private-endpoint`
* <span data-ttu-id="012e3-597">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="012e3-597">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="012e3-598">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con</span><span class="sxs-lookup"><span data-stu-id="012e3-598">Fixed issue where `--ip-tags` did not work correctly with</span></span> `public-ip create` 

### <a name="profile"></a><span data-ttu-id="012e3-599">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-599">Profile</span></span>
* <span data-ttu-id="012e3-600">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="012e3-600">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="012e3-601">RDBMS</span><span class="sxs-lookup"><span data-stu-id="012e3-601">RDBMS</span></span>
* <span data-ttu-id="012e3-602">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="012e3-602">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-603">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-603">Resource</span></span>
* <span data-ttu-id="012e3-604">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="012e3-604">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="012e3-605">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-605">Role</span></span>
* <span data-ttu-id="012e3-606">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="012e3-606">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="012e3-607">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="012e3-607">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="012e3-608">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="012e3-608">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-609">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-609">Storage</span></span>
* <span data-ttu-id="012e3-610">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="012e3-610">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-611">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-611">VM</span></span>
* <span data-ttu-id="012e3-612">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="012e3-612">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="012e3-613">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="012e3-613">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="012e3-614">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="012e3-614">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="012e3-615">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="012e3-615">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="012e3-616">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="012e3-616">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="012e3-617">Se ha mejorado la validación de argumentos de</span><span class="sxs-lookup"><span data-stu-id="012e3-617">Improved argument validation for</span></span> `vm create --image`

## <a name="october-23-2018"></a><span data-ttu-id="012e3-618">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-618">October 23, 2018</span></span>

<span data-ttu-id="012e3-619">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="012e3-619">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="012e3-620">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-620">Core</span></span>
* <span data-ttu-id="012e3-621">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en</span><span class="sxs-lookup"><span data-stu-id="012e3-621">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in</span></span> `--ids`
* <span data-ttu-id="012e3-622">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de</span><span class="sxs-lookup"><span data-stu-id="012e3-622">Added explicit warnings when parameters would be ignored by use of</span></span> `--ids`

### <a name="acr"></a><span data-ttu-id="012e3-623">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-623">ACR</span></span>
* <span data-ttu-id="012e3-624">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="012e3-624">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="012e3-625">CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-625">CDN</span></span>
* <span data-ttu-id="012e3-626">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="012e3-626">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="012e3-627">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="012e3-627">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="012e3-628">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-628">Container</span></span>
* <span data-ttu-id="012e3-629">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="012e3-629">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="012e3-630">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-630">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="012e3-631">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="012e3-631">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="012e3-632">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-632">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="012e3-633">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="012e3-633">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="012e3-634">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="012e3-634">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="012e3-635">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="012e3-635">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="012e3-636">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-636">CosmosDB</span></span>
* <span data-ttu-id="012e3-637">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con</span><span class="sxs-lookup"><span data-stu-id="012e3-637">Added `--enable-multiple-write-locations` support to</span></span> `cosmosdb create`

### <a name="interactive"></a><span data-ttu-id="012e3-638">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-638">Interactive</span></span>
* <span data-ttu-id="012e3-639">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="012e3-639">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="012e3-640">IoT Central</span><span class="sxs-lookup"><span data-stu-id="012e3-640">IoT Central</span></span>
* <span data-ttu-id="012e3-641">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="012e3-641">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="012e3-642">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="012e3-642">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-643">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-643">Monitor</span></span>
* <span data-ttu-id="012e3-644">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="012e3-644">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="012e3-645">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="012e3-645">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="012e3-646">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="012e3-646">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="012e3-647">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="012e3-647">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="012e3-648">Se ha agregado `--namespace` como alias para la opción en desuso</span><span class="sxs-lookup"><span data-stu-id="012e3-648">Added `--namespace` as alias for deprecated option</span></span> `--resource-provider`
  * <span data-ttu-id="012e3-649">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="012e3-649">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="012e3-650">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="012e3-650">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="012e3-651">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="012e3-651">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="012e3-652">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="012e3-652">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="012e3-653">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en</span><span class="sxs-lookup"><span data-stu-id="012e3-653">Improved validation for `--event-hub` and `--event-hub-rule` arguments to</span></span> `monitor diagnostic-settings create`

### <a name="network"></a><span data-ttu-id="012e3-654">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-654">Network</span></span>
* <span data-ttu-id="012e3-655">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="012e3-655">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="012e3-656">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="012e3-656">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="012e3-657">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="012e3-657">ServiceBus</span></span>
* <span data-ttu-id="012e3-658">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="012e3-658">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-659">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-659">SQL</span></span>
* <span data-ttu-id="012e3-660">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="012e3-660">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-661">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-661">Storage</span></span>
* <span data-ttu-id="012e3-662">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="012e3-662">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="012e3-663">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="012e3-663">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-664">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-664">VM</span></span>
* <span data-ttu-id="012e3-665">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en</span><span class="sxs-lookup"><span data-stu-id="012e3-665">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in</span></span> `[vm|vmss] create`
* <span data-ttu-id="012e3-666">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para</span><span class="sxs-lookup"><span data-stu-id="012e3-666">Updated supported size list supporting networking accelerator for</span></span> `vm create`
* <span data-ttu-id="012e3-667">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para</span><span class="sxs-lookup"><span data-stu-id="012e3-667">Added strong typed arguments for ultrassd iops and mbps configs for</span></span> `disk create`

## <a name="october-16-2018"></a><span data-ttu-id="012e3-668">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-668">October 16, 2018</span></span>

<span data-ttu-id="012e3-669">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="012e3-669">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-670">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-670">VM</span></span>
* <span data-ttu-id="012e3-671">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="012e3-671">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="012e3-672">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-672">October 9, 2018</span></span>

<span data-ttu-id="012e3-673">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="012e3-673">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="012e3-674">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-674">Core</span></span>
* <span data-ttu-id="012e3-675">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="012e3-675">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-676">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-676">ACR</span></span>
* <span data-ttu-id="012e3-677">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="012e3-677">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-678">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-678">ACS</span></span>
* <span data-ttu-id="012e3-679">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="012e3-679">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="012e3-680">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="012e3-680">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="012e3-681">Se ha cambiado `aks create` para que ya no requiera</span><span class="sxs-lookup"><span data-stu-id="012e3-681">Changed `aks create` to no longer require</span></span> `--aad-tenant-id`
* <span data-ttu-id="012e3-682">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="012e3-682">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="012e3-683">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-683">Container</span></span>
* <span data-ttu-id="012e3-684">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="012e3-684">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="012e3-685">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="012e3-685">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="012e3-686">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="012e3-686">Event Hub</span></span>
* <span data-ttu-id="012e3-687">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="012e3-687">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="012e3-688">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="012e3-688">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="012e3-689">Extensiones</span><span class="sxs-lookup"><span data-stu-id="012e3-689">Extensions</span></span>
* <span data-ttu-id="012e3-690">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="012e3-690">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="012e3-691">HDInsight</span><span class="sxs-lookup"><span data-stu-id="012e3-691">HDInsight</span></span>
* <span data-ttu-id="012e3-692">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="012e3-692">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-693">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-693">IoT</span></span>
* <span data-ttu-id="012e3-694">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="012e3-694">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-695">KeyVault</span><span class="sxs-lookup"><span data-stu-id="012e3-695">KeyVault</span></span>
* <span data-ttu-id="012e3-696">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="012e3-696">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="012e3-697">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-697">Network</span></span>
* <span data-ttu-id="012e3-698">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="012e3-698">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="012e3-699">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="012e3-699">See #6052</span></span>
* <span data-ttu-id="012e3-700">Se ha dejado de utilizar `--remote-vnet-id` para</span><span class="sxs-lookup"><span data-stu-id="012e3-700">Deprecated `--remote-vnet-id` for</span></span> `network vnet peering create`
* <span data-ttu-id="012e3-701">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="012e3-701">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="012e3-702">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet create` con</span><span class="sxs-lookup"><span data-stu-id="012e3-702">Added support for multiple subnet prefixes to `network vnet create` with</span></span> `--subnet-prefixes`
* <span data-ttu-id="012e3-703">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con</span><span class="sxs-lookup"><span data-stu-id="012e3-703">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with</span></span> `--address-prefixes`
* <span data-ttu-id="012e3-704">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="012e3-704">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="012e3-705">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a</span><span class="sxs-lookup"><span data-stu-id="012e3-705">Added `--service-endpoint-policy` convenience argument to</span></span> `network vnet subnet update`

### <a name="role"></a><span data-ttu-id="012e3-706">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-706">Role</span></span>
* <span data-ttu-id="012e3-707">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a</span><span class="sxs-lookup"><span data-stu-id="012e3-707">Added support for listing Azure AD app owners to</span></span> `ad app owner`
* <span data-ttu-id="012e3-708">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a</span><span class="sxs-lookup"><span data-stu-id="012e3-708">Added support for listing Azure AD service principal owners to</span></span> `ad sp owner`
* <span data-ttu-id="012e3-709">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="012e3-709">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="012e3-710">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="012e3-710">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="012e3-711">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="012e3-711">Service Bus</span></span>
* <span data-ttu-id="012e3-712">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="012e3-712">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-713">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-713">VM</span></span>
* <span data-ttu-id="012e3-714">Se ha corregido el campo `accessSas` vacío en</span><span class="sxs-lookup"><span data-stu-id="012e3-714">Fixed empty `accessSas` field in</span></span> `disk grant-access`
* <span data-ttu-id="012e3-715">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="012e3-715">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="012e3-716">Se ha corregido los comandos de actualización de</span><span class="sxs-lookup"><span data-stu-id="012e3-716">Fixed update commands for</span></span> `sig`
* <span data-ttu-id="012e3-717">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en</span><span class="sxs-lookup"><span data-stu-id="012e3-717">Added `--no-wait` support for managing image versions in</span></span> `sig`
* <span data-ttu-id="012e3-718">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="012e3-718">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="012e3-719">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="012e3-719">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="012e3-720">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-720">September 21, 2018</span></span>

<span data-ttu-id="012e3-721">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="012e3-721">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-722">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-722">ACR</span></span>
* <span data-ttu-id="012e3-723">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-723">Added ACR Task commands</span></span>
* <span data-ttu-id="012e3-724">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="012e3-724">Added quick run command</span></span>
* <span data-ttu-id="012e3-725">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="012e3-725">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="012e3-726">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-726">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="012e3-727">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="012e3-727">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="012e3-728">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="012e3-728">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-729">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-729">ACS</span></span>
* <span data-ttu-id="012e3-730">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="012e3-730">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="012e3-731">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="012e3-731">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-732">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-732">AppService</span></span>

* <span data-ttu-id="012e3-733">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="012e3-733">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="012e3-734">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="012e3-734">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="012e3-735">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="012e3-735">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="012e3-736">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="012e3-736">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-737">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-737">Batch</span></span>
* <span data-ttu-id="012e3-738">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="012e3-738">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="012e3-739">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="012e3-739">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="012e3-740">Se ha agregado `--max-tasks-per-node-option` a</span><span class="sxs-lookup"><span data-stu-id="012e3-740">Added `--max-tasks-per-node-option` to</span></span> `batch pool create`
* <span data-ttu-id="012e3-741">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="012e3-741">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="012e3-742">Batch AI</span><span class="sxs-lookup"><span data-stu-id="012e3-742">Batch AI</span></span> 
* <span data-ttu-id="012e3-743">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="012e3-743">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="012e3-744">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="012e3-744">Cognitive Services</span></span>
* <span data-ttu-id="012e3-745">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="012e3-745">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="012e3-746">Se ha agregado el comando</span><span class="sxs-lookup"><span data-stu-id="012e3-746">Added command</span></span> `cognitiveservices account list-usage`
* <span data-ttu-id="012e3-747">Se ha agregado el comando</span><span class="sxs-lookup"><span data-stu-id="012e3-747">Added command</span></span> `cognitiveservices account list-kinds`
* <span data-ttu-id="012e3-748">Se ha agregado el comando</span><span class="sxs-lookup"><span data-stu-id="012e3-748">Added command</span></span> `cognitiveservices account list`
* <span data-ttu-id="012e3-749">En desuso</span><span class="sxs-lookup"><span data-stu-id="012e3-749">Deprecated</span></span> `cognitiveservices list`
* <span data-ttu-id="012e3-750">Se ha cambiado `--name` para que sea opcional para</span><span class="sxs-lookup"><span data-stu-id="012e3-750">Changed `--name` to be optional for</span></span> `cognitiveservices account list-skus`

### <a name="container"></a><span data-ttu-id="012e3-751">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-751">Container</span></span>
* <span data-ttu-id="012e3-752">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="012e3-752">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="012e3-753">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="012e3-753">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="012e3-754">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-754">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="012e3-755">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-755">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="012e3-756">DataLake</span><span class="sxs-lookup"><span data-stu-id="012e3-756">Datalake</span></span>
* <span data-ttu-id="012e3-757">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-757">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="012e3-758">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="012e3-758">Interactive Shell</span></span>
* <span data-ttu-id="012e3-759">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="012e3-759">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="012e3-760">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="012e3-760">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-761">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-761">IoT</span></span>
* <span data-ttu-id="012e3-762">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-762">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="012e3-763">Key Vault</span><span class="sxs-lookup"><span data-stu-id="012e3-763">Key Vault</span></span>
* <span data-ttu-id="012e3-764">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="012e3-764">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="012e3-765">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-765">Network</span></span>
* <span data-ttu-id="012e3-766">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="012e3-766">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="012e3-767">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="012e3-767">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="012e3-768">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="012e3-768">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="012e3-769">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="012e3-769">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="012e3-770">Se ha agregado `--enable-tcp-reset` a</span><span class="sxs-lookup"><span data-stu-id="012e3-770">Add `--enable-tcp-reset` to</span></span> `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* <span data-ttu-id="012e3-771">Se ha agregado `--disable-outbound-snat` a</span><span class="sxs-lookup"><span data-stu-id="012e3-771">Add `--disable-outbound-snat` to</span></span> `network lb rule create/update`
* <span data-ttu-id="012e3-772">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="012e3-772">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="012e3-773">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="012e3-773">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="012e3-774">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="012e3-774">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* `network express-route create/update`<span data-ttu-id="012e3-775">: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="012e3-775">: Add `--allow-global-reach` flag</span></span>
* `network vnet subnet create/update`<span data-ttu-id="012e3-776">: Se ha agregado compatibilidad para</span><span class="sxs-lookup"><span data-stu-id="012e3-776">: Add support for</span></span> `--delegation`
* <span data-ttu-id="012e3-777">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="012e3-777">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="012e3-778">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="012e3-778">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="012e3-779">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="012e3-779">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* `dns record-set * create/update`<span data-ttu-id="012e3-780">: Se ha agregado compatibilidad para</span><span class="sxs-lookup"><span data-stu-id="012e3-780">: Add support for</span></span> `--target-resource`
* <span data-ttu-id="012e3-781">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="012e3-781">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="012e3-782">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="012e3-782">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="012e3-783">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="012e3-783">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="012e3-784">RDBMS</span><span class="sxs-lookup"><span data-stu-id="012e3-784">RDBMS</span></span>
* <span data-ttu-id="012e3-785">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="012e3-785">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="012e3-786">Reserva</span><span class="sxs-lookup"><span data-stu-id="012e3-786">Reservation</span></span>
* <span data-ttu-id="012e3-787">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="012e3-787">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="012e3-788">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="012e3-788">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="012e3-789">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="012e3-789">Manage App</span></span>
* <span data-ttu-id="012e3-790">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="012e3-790">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="012e3-791">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="012e3-791">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="012e3-792">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-792">Role</span></span>
* <span data-ttu-id="012e3-793">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="012e3-793">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="012e3-794">SignalR</span><span class="sxs-lookup"><span data-stu-id="012e3-794">SignalR</span></span>
* <span data-ttu-id="012e3-795">Primera versión</span><span class="sxs-lookup"><span data-stu-id="012e3-795">First release</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-796">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-796">Storage</span></span>
* <span data-ttu-id="012e3-797">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="012e3-797">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="012e3-798">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="012e3-798">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-799">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-799">VM</span></span>
* <span data-ttu-id="012e3-800">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="012e3-800">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="012e3-801">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante</span><span class="sxs-lookup"><span data-stu-id="012e3-801">Added support for shared image gallery through</span></span> `az sig`

## <a name="august-28-2018"></a><span data-ttu-id="012e3-802">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-802">August 28, 2018</span></span>

<span data-ttu-id="012e3-803">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="012e3-803">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="012e3-804">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-804">Core</span></span>

* <span data-ttu-id="012e3-805">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="012e3-805">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="012e3-806">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="012e3-806">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-807">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-807">ACR</span></span>

* <span data-ttu-id="012e3-808">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="012e3-808">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="012e3-809">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="012e3-809">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-810">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-810">ACS</span></span>

* <span data-ttu-id="012e3-811">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="012e3-811">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="012e3-812">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="012e3-812">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-813">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-813">AppService</span></span>

* <span data-ttu-id="012e3-814">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="012e3-814">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="012e3-815">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-815">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="012e3-816">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-816">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="012e3-817">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="012e3-817">Backup</span></span>

* <span data-ttu-id="012e3-818">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-818">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="012e3-819">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="012e3-819">Bot Service</span></span>

* <span data-ttu-id="012e3-820">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="012e3-820">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="012e3-821">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="012e3-821">Cognitive Services</span></span>

* <span data-ttu-id="012e3-822">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="012e3-822">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-823">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-823">IoT</span></span>

* <span data-ttu-id="012e3-824">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="012e3-824">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-825">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-825">Monitor</span></span>

* <span data-ttu-id="012e3-826">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="012e3-826">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="012e3-827">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="012e3-827">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="012e3-828">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-828">Network</span></span>

* <span data-ttu-id="012e3-829">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-829">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-830">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-830">Resource</span></span>

* <span data-ttu-id="012e3-831">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-831">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-832">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-832">Storage</span></span>

* <span data-ttu-id="012e3-833">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-833">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-834">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-834">VM</span></span>

* <span data-ttu-id="012e3-835">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-835">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="012e3-836">Se ha dejado de utilizar `--storage-caching` para</span><span class="sxs-lookup"><span data-stu-id="012e3-836">Deprecated `--storage-caching` for</span></span> `vm create`

## <a name="auguest-14-2018"></a><span data-ttu-id="012e3-837">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-837">Auguest 14, 2018</span></span>

<span data-ttu-id="012e3-838">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="012e3-838">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="012e3-839">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-839">Core</span></span>

* <span data-ttu-id="012e3-840">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="012e3-840">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="012e3-841">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="012e3-841">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="012e3-842">Telemetría</span><span class="sxs-lookup"><span data-stu-id="012e3-842">Telemetry</span></span>

* <span data-ttu-id="012e3-843">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="012e3-843">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-844">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-844">ACR</span></span>

* <span data-ttu-id="012e3-845">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="012e3-845">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="012e3-846">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="012e3-846">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-847">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-847">ACS</span></span>

* <span data-ttu-id="012e3-848">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="012e3-848">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="012e3-849">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="012e3-849">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="012e3-850">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="012e3-850">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="012e3-851">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="012e3-851">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="012e3-852">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="012e3-852">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="012e3-853">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-853">AppService</span></span>

* <span data-ttu-id="012e3-854">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="012e3-854">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="012e3-855">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="012e3-855">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="012e3-856">BatchAI</span><span class="sxs-lookup"><span data-stu-id="012e3-856">BatchAI</span></span>

* <span data-ttu-id="012e3-857">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="012e3-857">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="012e3-858">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-858">Container</span></span>

* <span data-ttu-id="012e3-859">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-859">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="012e3-860">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-860">IoT</span></span>

* <span data-ttu-id="012e3-861">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="012e3-861">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="012e3-862">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="012e3-862">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="012e3-863">Iot Central</span><span class="sxs-lookup"><span data-stu-id="012e3-863">Iot Central</span></span>

* <span data-ttu-id="012e3-864">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="012e3-864">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-865">KeyVault</span><span class="sxs-lookup"><span data-stu-id="012e3-865">KeyVault</span></span>


* <span data-ttu-id="012e3-866">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="012e3-866">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="012e3-867">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="012e3-867">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="012e3-868">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="012e3-868">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="012e3-869">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="012e3-869">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="012e3-870">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="012e3-870">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="012e3-871">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="012e3-871">Relay</span></span>

* <span data-ttu-id="012e3-872">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="012e3-872">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-873">Sql</span><span class="sxs-lookup"><span data-stu-id="012e3-873">Sql</span></span>

* <span data-ttu-id="012e3-874">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="012e3-874">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-875">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-875">Storage</span></span>

* <span data-ttu-id="012e3-876">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="012e3-876">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="012e3-877">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="012e3-877">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="012e3-878">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="012e3-878">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="012e3-879">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="012e3-879">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="012e3-880">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-880">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-881">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-881">VM</span></span>

* <span data-ttu-id="012e3-882">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="012e3-882">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="012e3-883">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-883">July 31, 2018</span></span>

<span data-ttu-id="012e3-884">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="012e3-884">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-885">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-885">ACR</span></span>

* <span data-ttu-id="012e3-886">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="012e3-886">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="012e3-887">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="012e3-887">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-888">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-888">ACS</span></span>

* <span data-ttu-id="012e3-889">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="012e3-889">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-890">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-890">Batch</span></span>

* <span data-ttu-id="012e3-891">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="012e3-891">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="012e3-892">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-892">Container</span></span>

* <span data-ttu-id="012e3-893">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="012e3-893">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="012e3-894">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-894">Network</span></span>

* <span data-ttu-id="012e3-895">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="012e3-895">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="012e3-896">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-896">Resource</span></span>

* <span data-ttu-id="012e3-897">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="012e3-897">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="012e3-898">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="012e3-898">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="012e3-899">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-899">Role</span></span>

* <span data-ttu-id="012e3-900">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="012e3-900">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="012e3-901">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="012e3-901">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="012e3-902">Search</span><span class="sxs-lookup"><span data-stu-id="012e3-902">Search</span></span>

* <span data-ttu-id="012e3-903">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="012e3-903">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="012e3-904">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="012e3-904">Service Bus</span></span>

* <span data-ttu-id="012e3-905">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="012e3-905">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="012e3-906">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="012e3-906">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  `--enable-batched-operations` <span data-ttu-id="012e3-907">y `--enable-dead-lettering-on-message-expiration` en</span><span class="sxs-lookup"><span data-stu-id="012e3-907">and `--enable-dead-lettering-on-message-expiration` in</span></span> `queue`
  *  `--dead-letter-on-filter-exceptions` <span data-ttu-id="012e3-908">bucear</span><span class="sxs-lookup"><span data-stu-id="012e3-908">in</span></span> `subscriptions`

### <a name="storage"></a><span data-ttu-id="012e3-909">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-909">Storage</span></span>

* <span data-ttu-id="012e3-910">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="012e3-910">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="012e3-911">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="012e3-911">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-912">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-912">VM</span></span>

* <span data-ttu-id="012e3-913">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="012e3-913">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="012e3-914">Se ha agregado compatibilidad con</span><span class="sxs-lookup"><span data-stu-id="012e3-914">Added support for</span></span> `StandardSSD_LRS`
* <span data-ttu-id="012e3-915">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="012e3-915">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="012e3-916">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="012e3-916">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="012e3-917">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-917">July 18, 2018</span></span>

<span data-ttu-id="012e3-918">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="012e3-918">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="012e3-919">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-919">Core</span></span>

* <span data-ttu-id="012e3-920">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="012e3-920">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="012e3-921">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="012e3-921">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="012e3-922">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-922">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-923">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-923">ACR</span></span>

* <span data-ttu-id="012e3-924">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="012e3-924">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="012e3-925">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="012e3-925">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="012e3-926">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="012e3-926">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="012e3-927">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="012e3-927">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-928">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-928">ACS</span></span>

* <span data-ttu-id="012e3-929">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="012e3-929">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-930">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-930">AppService</span></span>

* <span data-ttu-id="012e3-931">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="012e3-931">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-932">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-932">Batch</span></span>

* <span data-ttu-id="012e3-933">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="012e3-933">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="012e3-934">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="012e3-934">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="012e3-935">Batch AI</span><span class="sxs-lookup"><span data-stu-id="012e3-935">Batch AI</span></span>

* <span data-ttu-id="012e3-936">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="012e3-936">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="012e3-937">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-937">Container</span></span>

* <span data-ttu-id="012e3-938">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="012e3-938">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="012e3-939">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="012e3-939">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="012e3-940">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-940">Network</span></span>

* <span data-ttu-id="012e3-941">Se ha agregado compatibilidad de `--no-wait` con</span><span class="sxs-lookup"><span data-stu-id="012e3-941">Added `--no-wait` support to</span></span> `network nic [create|update|delete]` 
* <span data-ttu-id="012e3-942">Se agregó</span><span class="sxs-lookup"><span data-stu-id="012e3-942">Added</span></span> `network nic wait`
* <span data-ttu-id="012e3-943">Se ha dejado de utilizar el argumento `--ids` para</span><span class="sxs-lookup"><span data-stu-id="012e3-943">Deprecated `--ids` argument for</span></span> `network vnet [subnet|peering] list`
* <span data-ttu-id="012e3-944">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de</span><span class="sxs-lookup"><span data-stu-id="012e3-944">Added `--include-default` flag to include default security rules in the output of</span></span> `network nsg rule list`  

### <a name="resource"></a><span data-ttu-id="012e3-945">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-945">Resource</span></span>

* <span data-ttu-id="012e3-946">Se ha agregado compatibilidad de `--no-wait` con</span><span class="sxs-lookup"><span data-stu-id="012e3-946">Added `--no-wait` support to</span></span> `group deployment delete`
* <span data-ttu-id="012e3-947">Se ha agregado compatibilidad de `--no-wait` con</span><span class="sxs-lookup"><span data-stu-id="012e3-947">Added `--no-wait` support to</span></span> `deployment delete`
* <span data-ttu-id="012e3-948">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="012e3-948">Added `deployment wait` command</span></span>
* <span data-ttu-id="012e3-949">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="012e3-949">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-950">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-950">SQL</span></span>

* <span data-ttu-id="012e3-951">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="012e3-951">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="012e3-952">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de</span><span class="sxs-lookup"><span data-stu-id="012e3-952">Allow configuring default sql server by executing</span></span> `az configure --defaults sql-server=<name>`
* <span data-ttu-id="012e3-953">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="012e3-953">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-954">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-954">Storage</span></span>

* <span data-ttu-id="012e3-955">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="012e3-955">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-956">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-956">VM</span></span>

* <span data-ttu-id="012e3-957">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="012e3-957">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="012e3-958">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y</span><span class="sxs-lookup"><span data-stu-id="012e3-958">Added `--no-wait` support to `vm extension [set|delete]` and</span></span> `vmss extension [set|delete]`
* <span data-ttu-id="012e3-959">Se agregó</span><span class="sxs-lookup"><span data-stu-id="012e3-959">Added</span></span> `vm extension wait`

## <a name="july-3-2018"></a><span data-ttu-id="012e3-960">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-960">July 3, 2018</span></span>

<span data-ttu-id="012e3-961">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="012e3-961">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="012e3-962">AKS</span><span class="sxs-lookup"><span data-stu-id="012e3-962">AKS</span></span>

* <span data-ttu-id="012e3-963">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="012e3-963">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="012e3-964">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-964">July 3, 2018</span></span>

<span data-ttu-id="012e3-965">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="012e3-965">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="012e3-966">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-966">Core</span></span>

* <span data-ttu-id="012e3-967">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="012e3-967">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-968">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-968">ACR</span></span>

* <span data-ttu-id="012e3-969">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="012e3-969">Added polling build status</span></span>
* <span data-ttu-id="012e3-970">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="012e3-970">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="012e3-971">Se han agregado los parámetros `--top` y `--orderby` para</span><span class="sxs-lookup"><span data-stu-id="012e3-971">Added `--top` and `--orderby` parameters for</span></span> `show-manifests`

### <a name="acs"></a><span data-ttu-id="012e3-972">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-972">ACS</span></span>

* <span data-ttu-id="012e3-973">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="012e3-973">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="012e3-974">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="012e3-974">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="012e3-975">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="012e3-975">Updated options for `aks browse` command.</span></span> <span data-ttu-id="012e3-976">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="012e3-976">Added `--listen-port` support</span></span>
* <span data-ttu-id="012e3-977">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="012e3-977">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="012e3-978">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="012e3-978">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="012e3-979">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="012e3-979">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-980">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-980">AppService</span></span>

* <span data-ttu-id="012e3-981">Se ha agregado compatibilidad para deshabilitar la identidad mediante</span><span class="sxs-lookup"><span data-stu-id="012e3-981">Added support for disabling identity via</span></span> `webapp identity remove`
* <span data-ttu-id="012e3-982">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="012e3-982">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="012e3-983">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="012e3-983">Backup</span></span>

* <span data-ttu-id="012e3-984">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="012e3-984">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="012e3-985">BatchAI</span><span class="sxs-lookup"><span data-stu-id="012e3-985">BatchAI</span></span>

* <span data-ttu-id="012e3-986">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="012e3-986">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="012e3-987">Nube</span><span class="sxs-lookup"><span data-stu-id="012e3-987">Cloud</span></span>

* <span data-ttu-id="012e3-988">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="012e3-988">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="012e3-989">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-989">Container</span></span>

* <span data-ttu-id="012e3-990">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="012e3-990">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="012e3-991">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y</span><span class="sxs-lookup"><span data-stu-id="012e3-991">Added Log Analytics parameters `--log-analytics-workspace` and</span></span> `--log-analytics-workspace-key`
* <span data-ttu-id="012e3-992">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="012e3-992">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-993">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-993">Extension</span></span>

* <span data-ttu-id="012e3-994">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="012e3-994">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="012e3-995">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-995">Network</span></span>

* <span data-ttu-id="012e3-996">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="012e3-996">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="012e3-997">Rdbms</span><span class="sxs-lookup"><span data-stu-id="012e3-997">Rdbms</span></span>

* <span data-ttu-id="012e3-998">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="012e3-998">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-999">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-999">Resource</span></span>

* <span data-ttu-id="012e3-1000">Se ha agregado un nuevo grupo de operaciones</span><span class="sxs-lookup"><span data-stu-id="012e3-1000">Added new operation group</span></span> `deployment`

### <a name="vm"></a><span data-ttu-id="012e3-1001">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1001">VM</span></span>

* <span data-ttu-id="012e3-1002">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="012e3-1002">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="012e3-1003">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1003">June 25, 2018</span></span>

<span data-ttu-id="012e3-1004">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="012e3-1004">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="012e3-1005">CLI</span><span class="sxs-lookup"><span data-stu-id="012e3-1005">CLI</span></span>

* <span data-ttu-id="012e3-1006">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1006">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="012e3-1007">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1007">June 19, 2018</span></span>

<span data-ttu-id="012e3-1008">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="012e3-1008">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1009">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1009">Core</span></span>

* <span data-ttu-id="012e3-1010">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1010">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-1011">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1011">ACR</span></span>

* <span data-ttu-id="012e3-1012">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="012e3-1012">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="012e3-1013">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="012e3-1013">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1014">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1014">ACS</span></span>

* <span data-ttu-id="012e3-1015">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1015">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="012e3-1016">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="012e3-1016">Added `--update` support</span></span>
* <span data-ttu-id="012e3-1017">Se ha cambiado `aks get-credentials --admin` para que no reemplace el contexto de usuario en</span><span class="sxs-lookup"><span data-stu-id="012e3-1017">Changed `aks get-credentials --admin` to not eplace the user context in</span></span> `$HOME/.kube/config`
* <span data-ttu-id="012e3-1018">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="012e3-1018">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="012e3-1019">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="012e3-1019">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="012e3-1020">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1020">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and</span></span> `aks remove-connector`
* <span data-ttu-id="012e3-1021">Se han agregado nuevas regiones de Azure Container Instances para</span><span class="sxs-lookup"><span data-stu-id="012e3-1021">Added new Azure Container Instance regions for</span></span> `aks install-connector`
* <span data-ttu-id="012e3-1022">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a</span><span class="sxs-lookup"><span data-stu-id="012e3-1022">Added the normalized location into the helm release name and node name to</span></span> `aks install-connector`

### <a name="appservice"></a><span data-ttu-id="012e3-1023">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-1023">AppService</span></span>

* <span data-ttu-id="012e3-1024">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="012e3-1024">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="012e3-1025">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="012e3-1025">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-1026">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1026">Batch</span></span>

* <span data-ttu-id="012e3-1027">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="012e3-1027">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="012e3-1028">Batch AI</span><span class="sxs-lookup"><span data-stu-id="012e3-1028">Batch AI</span></span>

* <span data-ttu-id="012e3-1029">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="012e3-1029">Added support for workspaces.</span></span> <span data-ttu-id="012e3-1030">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="012e3-1030">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="012e3-1031">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1031">Added support for experiments.</span></span> <span data-ttu-id="012e3-1032">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="012e3-1032">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="012e3-1033">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="012e3-1033">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="012e3-1034">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1034">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="012e3-1035">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1035">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="012e3-1036">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1036">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="012e3-1037">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="012e3-1037">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="012e3-1038">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1038">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="012e3-1039">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1039">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="012e3-1040">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1040">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="012e3-1041">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1041">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="012e3-1042">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1042">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="012e3-1043">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1043">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="012e3-1044">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="012e3-1044">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="012e3-1045">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1045">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="012e3-1046">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="012e3-1046">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="012e3-1047">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="012e3-1047">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="012e3-1048">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="012e3-1048">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="012e3-1049">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="012e3-1049">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="012e3-1050">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="012e3-1050">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="012e3-1051">Mapas</span><span class="sxs-lookup"><span data-stu-id="012e3-1051">Maps</span></span>

* <span data-ttu-id="012e3-1052">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1052">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1053">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1053">Network</span></span>

* <span data-ttu-id="012e3-1054">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="012e3-1054">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="012e3-1055">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="012e3-1055">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="012e3-1056">N.º 6502</span><span class="sxs-lookup"><span data-stu-id="012e3-1056">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="012e3-1057">Reservations</span><span class="sxs-lookup"><span data-stu-id="012e3-1057">Reservations</span></span>

* <span data-ttu-id="012e3-1058">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1058">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to</span></span> `reservations catalog show`
* <span data-ttu-id="012e3-1059">Se ha agregado el parámetro `Location` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1059">Added parameter `Location`to</span></span> `reservations catalog show`
* <span data-ttu-id="012e3-1060">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de</span><span class="sxs-lookup"><span data-stu-id="012e3-1060">[BREAKING CHANGE] Removed `kind` from</span></span> `ReservationProperties`
* <span data-ttu-id="012e3-1061">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1061">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in</span></span> `Catalog`
* <span data-ttu-id="012e3-1062">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de</span><span class="sxs-lookup"><span data-stu-id="012e3-1062">[BREAKING CHANGE] Removed `size` and `tier` properties from</span></span> `Catalog`
* <span data-ttu-id="012e3-1063">Se ha agregado el parámetro `InstanceFlexibility` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1063">Added parameter `InstanceFlexibility` to</span></span> `reservations reservation update`

### <a name="role"></a><span data-ttu-id="012e3-1064">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-1064">Role</span></span>

* <span data-ttu-id="012e3-1065">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="012e3-1065">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1066">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1066">SQL</span></span>

* <span data-ttu-id="012e3-1067">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="012e3-1067">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1068">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1068">Storage</span></span>

* <span data-ttu-id="012e3-1069">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="012e3-1069">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1070">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1070">VM</span></span>

* <span data-ttu-id="012e3-1071">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en</span><span class="sxs-lookup"><span data-stu-id="012e3-1071">Improved refine vm size check for accelerated networking support in</span></span> `vm create`
* <span data-ttu-id="012e3-1072">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1072">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to</span></span> `Standard_DS1_v2`
* <span data-ttu-id="012e3-1073">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="012e3-1073">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="012e3-1074">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1074">June 13, 2018</span></span>

<span data-ttu-id="012e3-1075">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="012e3-1075">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1076">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1076">Core</span></span>

* <span data-ttu-id="012e3-1077">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="012e3-1077">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="012e3-1078">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1078">June 13, 2018</span></span>

<span data-ttu-id="012e3-1079">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="012e3-1079">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="012e3-1080">AKS</span><span class="sxs-lookup"><span data-stu-id="012e3-1080">AKS</span></span>

* <span data-ttu-id="012e3-1081">Se han agregado opciones de red avanzadas a</span><span class="sxs-lookup"><span data-stu-id="012e3-1081">Added advanced networking options to</span></span> `aks create`
* <span data-ttu-id="012e3-1082">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="012e3-1082">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="012e3-1083">Se ha agregado el argumento `--no-ssh-key` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1083">Added `--no-ssh-key` argument to</span></span> `aks create`
* <span data-ttu-id="012e3-1084">Se ha agregado el argumento `--enable-rbac` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1084">Added `--enable-rbac` argument to</span></span> `aks create`
* <span data-ttu-id="012e3-1085">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para la autenticación de Azure Active Directory a</span><span class="sxs-lookup"><span data-stu-id="012e3-1085">[PREVIEW] Added support for Azure Active Directory authentication to</span></span> `aks create`

### <a name="appservice"></a><span data-ttu-id="012e3-1086">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-1086">AppService</span></span>

* <span data-ttu-id="012e3-1087">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="012e3-1087">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="012e3-1088">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1088">June 5, 2018</span></span>

<span data-ttu-id="012e3-1089">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="012e3-1089">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1090">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1090">Interactive</span></span>

* <span data-ttu-id="012e3-1091">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="012e3-1091">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="012e3-1092">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1092">June 5, 2018</span></span>

<span data-ttu-id="012e3-1093">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="012e3-1093">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1094">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1094">Core</span></span>

* <span data-ttu-id="012e3-1095">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="012e3-1095">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="012e3-1096">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="012e3-1096">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1097">ACR</span></span>

* <span data-ttu-id="012e3-1098">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="012e3-1098">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="012e3-1099">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1099">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="012e3-1100">AKS</span><span class="sxs-lookup"><span data-stu-id="012e3-1100">AKS</span></span>

* <span data-ttu-id="012e3-1101">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="012e3-1101">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-1102">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1102">Batch</span></span>

* <span data-ttu-id="012e3-1103">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="012e3-1103">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-1104">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-1104">IOT</span></span>

* <span data-ttu-id="012e3-1105">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="012e3-1105">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1106">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1106">Network</span></span>

* <span data-ttu-id="012e3-1107">Se ha mejorado</span><span class="sxs-lookup"><span data-stu-id="012e3-1107">Improved</span></span> `network vnet peering`

### <a name="policy-insights"></a><span data-ttu-id="012e3-1108">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="012e3-1108">Policy Insights</span></span>

* <span data-ttu-id="012e3-1109">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="012e3-1109">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="012e3-1110">ARM</span><span class="sxs-lookup"><span data-stu-id="012e3-1110">ARM</span></span>

* <span data-ttu-id="012e3-1111">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1111">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1112">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1112">SQL</span></span>

* <span data-ttu-id="012e3-1113">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="012e3-1113">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="012e3-1114">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="012e3-1114">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="012e3-1115">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1115">Storage</span></span>

* <span data-ttu-id="012e3-1116">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="012e3-1116">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1117">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1117">VM</span></span>

* <span data-ttu-id="012e3-1118">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="012e3-1118">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="012e3-1119">Se ha agregado la opción `--accelerated-networking` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1119">Added `--accelerated-networking` option to</span></span> `vm create`
* <span data-ttu-id="012e3-1120">Se ha agregado `--tags` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1120">Added `--tags` to</span></span> `identity create`

## <a name="may-22-2018"></a><span data-ttu-id="012e3-1121">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1121">May 22, 2018</span></span>

<span data-ttu-id="012e3-1122">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="012e3-1122">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1123">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1123">Core</span></span>

* <span data-ttu-id="012e3-1124">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="012e3-1124">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1125">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1125">ACS</span></span>

* <span data-ttu-id="012e3-1126">Se han agregado los nuevos comandos de Dev-Spaces `aks use-dev-spaces` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1126">Added new Dev-Spaces commands `aks use-dev-spaces` and</span></span> `aks remove-dev-spaces`
* <span data-ttu-id="012e3-1127">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="012e3-1127">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-1128">AppService</span></span>

* <span data-ttu-id="012e3-1129">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="012e3-1129">Improved generic update commands</span></span>
* <span data-ttu-id="012e3-1130">Se ha agregado compatibilidad con el modo asincrónico a</span><span class="sxs-lookup"><span data-stu-id="012e3-1130">Added async support for</span></span> `webapp deployment source config-zip`

### <a name="container"></a><span data-ttu-id="012e3-1131">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1131">Container</span></span>

* <span data-ttu-id="012e3-1132">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="012e3-1132">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="012e3-1133">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-1133">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-1134">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1134">Extension</span></span>

* <span data-ttu-id="012e3-1135">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="012e3-1135">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1136">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1136">Interactive</span></span>

* <span data-ttu-id="012e3-1137">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="012e3-1137">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="012e3-1138">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="012e3-1138">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-1139">KeyVault</span><span class="sxs-lookup"><span data-stu-id="012e3-1139">KeyVault</span></span>

* <span data-ttu-id="012e3-1140">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="012e3-1140">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1141">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1141">Network</span></span>

* <span data-ttu-id="012e3-1142">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="012e3-1142">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="012e3-1143">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="012e3-1143">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1144">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1144">SQL</span></span>

* <span data-ttu-id="012e3-1145">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="012e3-1145">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="012e3-1146">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1146">Renamed `serviceLevelObjective` property to</span></span> `currentServiceObjectiveName`
    * <span data-ttu-id="012e3-1147">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="012e3-1147">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="012e3-1148">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="012e3-1148">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="012e3-1149">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="012e3-1149">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * `requestedServiceObjectiveName`<span data-ttu-id="012e3-1150">.</span><span class="sxs-lookup"><span data-stu-id="012e3-1150">.</span></span>  <span data-ttu-id="012e3-1151">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="012e3-1151">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * `edition`<span data-ttu-id="012e3-1152">.</span><span class="sxs-lookup"><span data-stu-id="012e3-1152">.</span></span> <span data-ttu-id="012e3-1153">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="012e3-1153">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * `elasticPoolName`<span data-ttu-id="012e3-1154">.</span><span class="sxs-lookup"><span data-stu-id="012e3-1154">.</span></span> <span data-ttu-id="012e3-1155">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="012e3-1155">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="012e3-1156">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="012e3-1156">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * `edition`<span data-ttu-id="012e3-1157">.</span><span class="sxs-lookup"><span data-stu-id="012e3-1157">.</span></span> <span data-ttu-id="012e3-1158">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="012e3-1158">To update, use the `--edition` parameter</span></span>
    * `dtu`<span data-ttu-id="012e3-1159">.</span><span class="sxs-lookup"><span data-stu-id="012e3-1159">.</span></span> <span data-ttu-id="012e3-1160">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="012e3-1160">To update, use the `--capacity` parameter</span></span>
    *  `databaseDtuMin`<span data-ttu-id="012e3-1161">.</span><span class="sxs-lookup"><span data-stu-id="012e3-1161">.</span></span> <span data-ttu-id="012e3-1162">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="012e3-1162">To update, use the `--db-min-capacity` parameter</span></span>
    *  `databaseDtuMax`<span data-ttu-id="012e3-1163">.</span><span class="sxs-lookup"><span data-stu-id="012e3-1163">.</span></span> <span data-ttu-id="012e3-1164">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="012e3-1164">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="012e3-1165">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1165">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="012e3-1166">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1166">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1167">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1167">Storage</span></span>

* <span data-ttu-id="012e3-1168">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="012e3-1168">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="012e3-1169">Se ha corregido un problema con</span><span class="sxs-lookup"><span data-stu-id="012e3-1169">Fixed problem with</span></span> `storage entity query`

### <a name="vm"></a><span data-ttu-id="012e3-1170">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1170">VM</span></span>

* <span data-ttu-id="012e3-1171">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1171">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="012e3-1172">Se puede obtener la misma compatibilidad mediante `vm update` o</span><span class="sxs-lookup"><span data-stu-id="012e3-1172">The same support can be accessed through `vm update` or</span></span> `vm disk attach`
* <span data-ttu-id="012e3-1173">Se ha corregido la correspondencia de imágenes de extensión en</span><span class="sxs-lookup"><span data-stu-id="012e3-1173">Fixed extension image matching in</span></span> `[vm|vmss] extension`
* <span data-ttu-id="012e3-1174">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="012e3-1174">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="012e3-1175">Se ha agregado `--license-type` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1175">Added `--license-type` to</span></span> `[vm|vmss] update`

## <a name="may-7-2018"></a><span data-ttu-id="012e3-1176">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1176">May 7, 2018</span></span>

<span data-ttu-id="012e3-1177">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="012e3-1177">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1178">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1178">Core</span></span>

* <span data-ttu-id="012e3-1179">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="012e3-1179">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="012e3-1180">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="012e3-1180">Added limited support for positional arguments</span></span>
* <span data-ttu-id="012e3-1181">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1181">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="012e3-1182">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="012e3-1182">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="012e3-1183">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1183">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="012e3-1184">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="012e3-1184">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="012e3-1185">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1185">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="012e3-1186">Se han mejorado los errores cuando los usuarios escriben</span><span class="sxs-lookup"><span data-stu-id="012e3-1186">Improved error when users type</span></span> `az ''`
* <span data-ttu-id="012e3-1187">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1187">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-1188">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1188">ACR</span></span>

* <span data-ttu-id="012e3-1189">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="012e3-1189">Added ACR Build commands</span></span>
* <span data-ttu-id="012e3-1190">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="012e3-1190">Improved resource not found error messages</span></span>
* <span data-ttu-id="012e3-1191">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="012e3-1191">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="012e3-1192">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="012e3-1192">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="012e3-1193">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="012e3-1193">Improved repository commands error messages</span></span>
* <span data-ttu-id="012e3-1194">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="012e3-1194">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1195">ACS</span></span>

* <span data-ttu-id="012e3-1196">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-1196">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="012e3-1197">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="012e3-1197">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="012e3-1198">AMS</span><span class="sxs-lookup"><span data-stu-id="012e3-1198">AMS</span></span>

* <span data-ttu-id="012e3-1199">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="012e3-1199">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1200">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1200">Appservice</span></span>

* <span data-ttu-id="012e3-1201">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="012e3-1201">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="012e3-1202">Se ha eliminado `--runtime-version` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1202">Removed `--runtime-version` from</span></span> `webapp auth update`
* <span data-ttu-id="012e3-1203">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="012e3-1203">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="012e3-1204">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-1204">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="012e3-1205">Batch AI</span><span class="sxs-lookup"><span data-stu-id="012e3-1205">Batch AI</span></span>

* <span data-ttu-id="012e3-1206">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="012e3-1206">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="012e3-1207">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="012e3-1207">Cognitive Services</span></span>

* <span data-ttu-id="012e3-1208">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="012e3-1208">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="012e3-1209">Consumo</span><span class="sxs-lookup"><span data-stu-id="012e3-1209">Consumption</span></span>

* <span data-ttu-id="012e3-1210">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="012e3-1210">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1211">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1211">Container</span></span>

* <span data-ttu-id="012e3-1212">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="012e3-1212">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="012e3-1213">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="012e3-1213">Cosmos DB</span></span>

* <span data-ttu-id="012e3-1214">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="012e3-1214">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="012e3-1215">DMS</span><span class="sxs-lookup"><span data-stu-id="012e3-1215">DMS</span></span>

* <span data-ttu-id="012e3-1216">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1216">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-1217">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1217">Extension</span></span>

* <span data-ttu-id="012e3-1218">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="012e3-1218">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1219">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1219">Interactive</span></span>

* <span data-ttu-id="012e3-1220">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="012e3-1220">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="012e3-1221">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="012e3-1221">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="012e3-1222">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="012e3-1222">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="012e3-1223">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1223">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="012e3-1224">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-1224">Lab</span></span>

* <span data-ttu-id="012e3-1225">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="012e3-1225">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1226">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1226">Network</span></span>

* <span data-ttu-id="012e3-1227">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="012e3-1227">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="012e3-1228">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1228">Profile</span></span>

* <span data-ttu-id="012e3-1229">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1229">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="012e3-1230">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="012e3-1230">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="012e3-1231">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="012e3-1231">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="012e3-1232">Redis</span><span class="sxs-lookup"><span data-stu-id="012e3-1232">Redis</span></span>

* <span data-ttu-id="012e3-1233">Se ha dejado de usar `redis patch-schedule patch-schedule show` en favor de</span><span class="sxs-lookup"><span data-stu-id="012e3-1233">Deprecated `redis patch-schedule patch-schedule show` in favor of</span></span> `redis patch-schedule show`
* <span data-ttu-id="012e3-1234">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1234">Deprecated `redis list-all`.</span></span> <span data-ttu-id="012e3-1235">Esta funcionalidad se ha situado en</span><span class="sxs-lookup"><span data-stu-id="012e3-1235">This functionality has been folded into</span></span> `redis list`
* <span data-ttu-id="012e3-1236">Se ha dejado de usar `redis import-method` en favor de</span><span class="sxs-lookup"><span data-stu-id="012e3-1236">Deprecated `redis import-method` in favor of</span></span> `redis import`
* <span data-ttu-id="012e3-1237">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1237">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="012e3-1238">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-1238">Role</span></span>

* <span data-ttu-id="012e3-1239">[CAMBIO IMPORTANTE] Se ha dejado de utilizar y se ha eliminado</span><span class="sxs-lookup"><span data-stu-id="012e3-1239">[BREAKING CHANGE] Removed deprecated</span></span> `ad sp reset-credentials`

### <a name="storage"></a><span data-ttu-id="012e3-1240">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1240">Storage</span></span>

* <span data-ttu-id="012e3-1241">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="012e3-1241">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="012e3-1242">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="012e3-1242">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="012e3-1243">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="012e3-1243">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="012e3-1244">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="012e3-1244">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="012e3-1245">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="012e3-1245">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1246">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1246">VM</span></span>

* <span data-ttu-id="012e3-1247">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="012e3-1247">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="012e3-1248">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="012e3-1248">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="012e3-1249">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="012e3-1249">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="012e3-1250">Se ha agregado compatibilidad con la directiva de expulsión a</span><span class="sxs-lookup"><span data-stu-id="012e3-1250">Added support for eviction policy to</span></span> `vmss`
* <span data-ttu-id="012e3-1251">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="012e3-1251">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="012e3-1252">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="012e3-1252">Added write accelerator support</span></span>
* <span data-ttu-id="012e3-1253">Se agregó</span><span class="sxs-lookup"><span data-stu-id="012e3-1253">Added</span></span> `vmss perform-maintenance`
* <span data-ttu-id="012e3-1254">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="012e3-1254">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="012e3-1255">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="012e3-1255">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="012e3-1256">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1256">April 10, 2018</span></span>

<span data-ttu-id="012e3-1257">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="012e3-1257">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1258">ACR</span></span>

* <span data-ttu-id="012e3-1259">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="012e3-1259">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1260">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1260">ACS</span></span>

* <span data-ttu-id="012e3-1261">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="012e3-1261">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1262">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1262">Appservice</span></span>

* [<span data-ttu-id="012e3-1263">CAMBIO IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="012e3-1263">BREAKING CHANGE</span></span>]: Removed `assign-identity`
* <span data-ttu-id="012e3-1264">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="012e3-1264">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="012e3-1265">BatchAI</span><span class="sxs-lookup"><span data-stu-id="012e3-1265">BatchAI</span></span>

* <span data-ttu-id="012e3-1266">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="012e3-1266">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="012e3-1267">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="012e3-1267">Job level mounting</span></span>
  - <span data-ttu-id="012e3-1268">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="012e3-1268">Environment variables with secret values</span></span>
  - <span data-ttu-id="012e3-1269">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1269">Performance counters settings</span></span>
  - <span data-ttu-id="012e3-1270">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="012e3-1270">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="012e3-1271">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="012e3-1271">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="012e3-1272">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="012e3-1272">Usage and limits reporting</span></span>
  - <span data-ttu-id="012e3-1273">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="012e3-1273">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="012e3-1274">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="012e3-1274">Support for custom images</span></span>
  - <span data-ttu-id="012e3-1275">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="012e3-1275">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="012e3-1276">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="012e3-1276">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="012e3-1277">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="012e3-1277">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="012e3-1278">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="012e3-1278">National clouds are supported</span></span>
* <span data-ttu-id="012e3-1279">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="012e3-1279">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="012e3-1280">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="012e3-1280">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="012e3-1281">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="012e3-1281">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="012e3-1282">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="012e3-1282">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="012e3-1283">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="012e3-1283">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="012e3-1284">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="012e3-1284">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="012e3-1285">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1285">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="012e3-1286">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="012e3-1286">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="012e3-1287">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="012e3-1287">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="012e3-1288">Se ha agregado la opción `--generate-ssh-keys` a `cluster create` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1288">Added `--generate-ssh-keys` option to `cluster create` and</span></span> `file-server create`
* <span data-ttu-id="012e3-1289">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1289">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="012e3-1290">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="012e3-1290">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="012e3-1291">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1291">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="012e3-1292">Facturación</span><span class="sxs-lookup"><span data-stu-id="012e3-1292">Billing</span></span>

* <span data-ttu-id="012e3-1293">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="012e3-1293">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="012e3-1294">Consumo</span><span class="sxs-lookup"><span data-stu-id="012e3-1294">Consumption</span></span>

* <span data-ttu-id="012e3-1295">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1295">Added `marketplace` commands</span></span>
* <span data-ttu-id="012e3-1296">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1296">[BREAKING CHANGE] Renamed `reservations summaries` to</span></span> `reservation summary`
* <span data-ttu-id="012e3-1297">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1297">[BREAKING CHANGE] Renamed `reservations details` to</span></span> `reservation detail`
* <span data-ttu-id="012e3-1298">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="012e3-1298">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="012e3-1299">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="012e3-1299">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="012e3-1300">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="012e3-1300">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1301">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1301">Container</span></span>

* <span data-ttu-id="012e3-1302">Se han agregado los parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1302">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and</span></span> `--gitrepo-mount-path`
* <span data-ttu-id="012e3-1303">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="012e3-1303">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-1304">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1304">Extension</span></span>

* <span data-ttu-id="012e3-1305">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="012e3-1305">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1306">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1306">Interactive</span></span>

* <span data-ttu-id="012e3-1307">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="012e3-1307">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="012e3-1308">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1308">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="012e3-1309">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="012e3-1309">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1310">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1310">Network</span></span>

* <span data-ttu-id="012e3-1311">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1311">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="012e3-1312">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1312">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="012e3-1313">N.º 4910</span><span class="sxs-lookup"><span data-stu-id="012e3-1313">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="012e3-1314">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="012e3-1314">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="012e3-1315">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="012e3-1315">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="012e3-1316">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1316">Fixed issue with `--disable-bgp-route-propagation` flag in</span></span> `network route-table [create|update]`
* <span data-ttu-id="012e3-1317">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de</span><span class="sxs-lookup"><span data-stu-id="012e3-1317">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for</span></span> `network lb [create|update]`
* <span data-ttu-id="012e3-1318">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1318">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and</span></span> `network dns record-set txt add-record`

### <a name="profile"></a><span data-ttu-id="012e3-1319">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1319">Profile</span></span>

* <span data-ttu-id="012e3-1320">Se ha agregado compatibilidad para las cuentas de Azure clásico en</span><span class="sxs-lookup"><span data-stu-id="012e3-1320">Added support for Azure Classic accounts in</span></span> `account list`
* <span data-ttu-id="012e3-1321">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="012e3-1321">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="012e3-1322">RDBMS</span><span class="sxs-lookup"><span data-stu-id="012e3-1322">RDBMS</span></span>

* <span data-ttu-id="012e3-1323">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1323">Added `georestore` command</span></span>
* <span data-ttu-id="012e3-1324">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1324">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1325">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1325">Resource</span></span>

* <span data-ttu-id="012e3-1326">Se ha agregado compatibilidad para `--metadata` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1326">Added support for `--metadata` to</span></span> `policy definition create`
* <span data-ttu-id="012e3-1327">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1327">Added support for `--metadata`, `--set`, `--add`, `--remove` to</span></span> `policy definition update`

### <a name="sql"></a><span data-ttu-id="012e3-1328">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1328">SQL</span></span>

* <span data-ttu-id="012e3-1329">Se han agregado `sql elastic-pool op list` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1329">Added `sql elastic-pool op list` and</span></span> `sql elastic-pool op cancel`

### <a name="storage"></a><span data-ttu-id="012e3-1330">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1330">Storage</span></span>

* <span data-ttu-id="012e3-1331">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="012e3-1331">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1332">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1332">VM</span></span>

* <span data-ttu-id="012e3-1333">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en</span><span class="sxs-lookup"><span data-stu-id="012e3-1333">Added support to configure platform fault domain count to</span></span> `vmss create`
* <span data-ttu-id="012e3-1334">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="012e3-1334">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [<span data-ttu-id="012e3-1335">CAMBIO IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="012e3-1335">BREAKING CHANGE</span></span>]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="012e3-1336">Se ha agregado compatibilidad para la SKU de IP pública a</span><span class="sxs-lookup"><span data-stu-id="012e3-1336">Added support for Public-IP SKU to</span></span> `vm create`
* <span data-ttu-id="012e3-1337">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="012e3-1337">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="012e3-1338">N.º 5718</span><span class="sxs-lookup"><span data-stu-id="012e3-1338">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="012e3-1339">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="012e3-1339">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="012e3-1340">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1340">March 27, 2018</span></span>

<span data-ttu-id="012e3-1341">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="012e3-1341">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1342">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1342">Core</span></span>

* <span data-ttu-id="012e3-1343">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="012e3-1343">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1344">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1344">ACS</span></span>

* <span data-ttu-id="012e3-1345">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="012e3-1345">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1346">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1346">Appservice</span></span>

* <span data-ttu-id="012e3-1347">Se ha agregado compatibilidad solo para HTTPS a</span><span class="sxs-lookup"><span data-stu-id="012e3-1347">Added HTTPS-only support to</span></span> `webapp update`
* <span data-ttu-id="012e3-1348">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1348">Added support for slots to `az webapp identity [assign|show]` and</span></span> `az functionapp identity [assign|show]`

### <a name="backup"></a><span data-ttu-id="012e3-1349">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="012e3-1349">Backup</span></span>

* <span data-ttu-id="012e3-1350">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1350">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="012e3-1351">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1351">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="012e3-1352">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="012e3-1352">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="012e3-1353">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="012e3-1353">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1354">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1354">Container</span></span>

* <span data-ttu-id="012e3-1355">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1355">Added `container exec` command.</span></span> <span data-ttu-id="012e3-1356">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="012e3-1356">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="012e3-1357">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-1357">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-1358">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1358">Extension</span></span>

* <span data-ttu-id="012e3-1359">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-1359">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="012e3-1360">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con</span><span class="sxs-lookup"><span data-stu-id="012e3-1360">Changed `extension list-available` to show full extension data with</span></span> `--show-details`
* <span data-ttu-id="012e3-1361">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="012e3-1361">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1362">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1362">Interactive</span></span>

* <span data-ttu-id="012e3-1363">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1363">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="012e3-1364">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="012e3-1364">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="012e3-1365">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1365">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="012e3-1366">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="012e3-1366">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="012e3-1367">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-1367">Lab</span></span>

* <span data-ttu-id="012e3-1368">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="012e3-1368">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-1369">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1369">Monitor</span></span>

* <span data-ttu-id="012e3-1370">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="012e3-1370">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="012e3-1371">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="012e3-1371">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="012e3-1372">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="012e3-1372">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1373">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1373">Network</span></span>

* <span data-ttu-id="012e3-1374">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="012e3-1374">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="012e3-1375">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1375">Profile</span></span>

* <span data-ttu-id="012e3-1376">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1376">Added warning for `--identity-port` and `--msi-port` to</span></span> `login`

### <a name="rdbms"></a><span data-ttu-id="012e3-1377">RDBMS</span><span class="sxs-lookup"><span data-stu-id="012e3-1377">RDBMS</span></span>

* <span data-ttu-id="012e3-1378">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="012e3-1378">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1379">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1379">Resource</span></span>

* [<span data-ttu-id="012e3-1380">CAMBIO IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="012e3-1380">BREAKING CHANGE</span></span>]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="012e3-1381">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-1381">Role</span></span>

* <span data-ttu-id="012e3-1382">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a</span><span class="sxs-lookup"><span data-stu-id="012e3-1382">Added support for required access configurations and native clients to</span></span> `az ad app create`
* <span data-ttu-id="012e3-1383">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="012e3-1383">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="012e3-1384">Se agregaron comandos de administración de credenciales</span><span class="sxs-lookup"><span data-stu-id="012e3-1384">Added credential management commands</span></span> `ad sp credential [reset|list|delete]`
* <span data-ttu-id="012e3-1385">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="012e3-1385">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="012e3-1386">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1386">Added support for `dataActions` and `notDataActions` permissions to</span></span> `role definition`

### <a name="storage"></a><span data-ttu-id="012e3-1387">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1387">Storage</span></span>

* <span data-ttu-id="012e3-1388">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="012e3-1388">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="012e3-1389">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="012e3-1389">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1390">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1390">VM</span></span>

* <span data-ttu-id="012e3-1391">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="012e3-1391">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="012e3-1392">Se ha agregado compatibilidad con zonas resistentes a</span><span class="sxs-lookup"><span data-stu-id="012e3-1392">Added zone resilient support to</span></span> `vm [snapshot|image]`
* <span data-ttu-id="012e3-1393">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="012e3-1393">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="012e3-1394">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="012e3-1394">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="012e3-1395">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1395">March 13, 2018</span></span>

<span data-ttu-id="012e3-1396">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="012e3-1396">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-1397">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1397">ACR</span></span>

* <span data-ttu-id="012e3-1398">Se ha agregado compatibilidad con el parámetro `--image` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1398">Added support for `--image` parameter to</span></span> `repository delete`
* <span data-ttu-id="012e3-1399">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="012e3-1399">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="012e3-1400">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1400">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1401">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1401">ACS</span></span>

* <span data-ttu-id="012e3-1402">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="012e3-1402">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="012e3-1403">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="012e3-1403">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="012e3-1404">Advisor</span><span class="sxs-lookup"><span data-stu-id="012e3-1404">Advisor</span></span>

* <span data-ttu-id="012e3-1405">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1405">[BREAKING CHANGE] Renamed `advisor configuration get` to</span></span> `advisor configuration list`
* <span data-ttu-id="012e3-1406">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1406">[BREAKING CHANGE] Renamed `advisor configuration set` to</span></span> `advisor configuration update`
* <span data-ttu-id="012e3-1407">[CAMBIO IMPORTANTE] Se ha quitado</span><span class="sxs-lookup"><span data-stu-id="012e3-1407">[BREAKING CHANGE] Removed</span></span> `advisor recommendation generate`
* <span data-ttu-id="012e3-1408">Se ha agregado el parámetro `--refresh` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1408">Added `--refresh` parameter to</span></span> `advisor recommendation list`
* <span data-ttu-id="012e3-1409">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1409">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1410">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1410">Appservice</span></span>

* <span data-ttu-id="012e3-1411">En desuso</span><span class="sxs-lookup"><span data-stu-id="012e3-1411">Deprecated</span></span> `[webapp|functionapp] assign-identity`
* <span data-ttu-id="012e3-1412">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1412">Added managed identity commands `webapp identity [assign|show]` and</span></span> `functionapp identity [assign|show]`

### <a name="eventhubs"></a><span data-ttu-id="012e3-1413">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="012e3-1413">Eventhubs</span></span>

* <span data-ttu-id="012e3-1414">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="012e3-1414">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-1415">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1415">Extension</span></span>

* <span data-ttu-id="012e3-1416">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="012e3-1416">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1417">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1417">Interactive</span></span>

* <span data-ttu-id="012e3-1418">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="012e3-1418">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="012e3-1419">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="012e3-1419">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="012e3-1420">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="012e3-1420">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="012e3-1421">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="012e3-1421">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-1422">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1422">Monitor</span></span>

* <span data-ttu-id="012e3-1423">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="012e3-1423">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="012e3-1424">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1424">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="012e3-1425">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1425">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="012e3-1426">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1426">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1427">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1427">Network</span></span>

* <span data-ttu-id="012e3-1428">[CAMBIO IMPORTANTE] Se ha quitado el parámetro `--tags` de</span><span class="sxs-lookup"><span data-stu-id="012e3-1428">[BREAKING CHANGE] Removed `--tags` parameter from</span></span>  `route-filter rule create`
* <span data-ttu-id="012e3-1429">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="012e3-1429">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="012e3-1430">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1430">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="012e3-1431">Se han agregado los parámetros `--vnet` y `--subnet` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1431">Added `--vnet` and `--subnet` parameters to</span></span> `network watcher show-topology`

### <a name="profile"></a><span data-ttu-id="012e3-1432">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1432">Profile</span></span>

* <span data-ttu-id="012e3-1433">Se ha dejado de utilizar el parámetro `--msi` para</span><span class="sxs-lookup"><span data-stu-id="012e3-1433">Deprecated `--msi` parameter for</span></span> `az login`
* <span data-ttu-id="012e3-1434">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a</span><span class="sxs-lookup"><span data-stu-id="012e3-1434">Added `--identity` parameter for `az login` to replace</span></span> `--msi`

### <a name="rdbms"></a><span data-ttu-id="012e3-1435">RDBMS</span><span class="sxs-lookup"><span data-stu-id="012e3-1435">RDBMS</span></span>

* <span data-ttu-id="012e3-1436">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="012e3-1436">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="012e3-1437">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="012e3-1437">Service Bus</span></span>

* <span data-ttu-id="012e3-1438">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="012e3-1438">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1439">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1439">Storage</span></span>

* <span data-ttu-id="012e3-1440">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="012e3-1440">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="012e3-1441">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="012e3-1441">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1442">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1442">VM</span></span>

* <span data-ttu-id="012e3-1443">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="012e3-1443">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="012e3-1444">Se han dejado de utilizar `[vm|vmss] assign-identity` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1444">Deprecated `[vm|vmss] assign-identity` and</span></span> `[vm|vmss] remove-identity`
* <span data-ttu-id="012e3-1445">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="012e3-1445">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="012e3-1446">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="012e3-1446">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="012e3-1447">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1447">February 27, 2018</span></span>

<span data-ttu-id="012e3-1448">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="012e3-1448">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1449">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1449">Core</span></span>

* <span data-ttu-id="012e3-1450">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="012e3-1450">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="012e3-1451">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="012e3-1451">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="012e3-1452">Se ha agregado el registro de HTTP a</span><span class="sxs-lookup"><span data-stu-id="012e3-1452">Added HTTP logging to</span></span> `--debug`

### <a name="acs"></a><span data-ttu-id="012e3-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1453">ACS</span></span>

* <span data-ttu-id="012e3-1454">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="012e3-1454">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="012e3-1455">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="012e3-1455">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="012e3-1456">Se han agregado los parámetros `--aci-container-group`, `--location` y `--image-tag` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1456">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to</span></span> `aks install-connector`
* <span data-ttu-id="012e3-1457">Se ha eliminado el aviso de desuso de</span><span class="sxs-lookup"><span data-stu-id="012e3-1457">Removed deprecation notice from</span></span> `aks get-versions`

### <a name="appservice"></a><span data-ttu-id="012e3-1458">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1458">Appservice</span></span>

* <span data-ttu-id="012e3-1459">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="012e3-1459">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="012e3-1460">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="012e3-1460">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="012e3-1461">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="012e3-1461">Cognitive Services</span></span>

* <span data-ttu-id="012e3-1462">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="012e3-1462">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="012e3-1463">Consumo</span><span class="sxs-lookup"><span data-stu-id="012e3-1463">Consumption</span></span>

* <span data-ttu-id="012e3-1464">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="012e3-1464">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="012e3-1465">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="012e3-1465">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1466">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1466">Container</span></span>

* <span data-ttu-id="012e3-1467">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="012e3-1467">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1468">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1468">Network</span></span>

* <span data-ttu-id="012e3-1469">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): Falta el cliente en</span><span class="sxs-lookup"><span data-stu-id="012e3-1469">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in</span></span> `network vnet-gateway vpn-client generate`

### <a name="resource"></a><span data-ttu-id="012e3-1470">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1470">Resource</span></span>

* <span data-ttu-id="012e3-1471">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="012e3-1471">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="012e3-1472">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-1472">Role</span></span>

* <span data-ttu-id="012e3-1473">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="012e3-1473">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1474">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1474">SQL</span></span>

* <span data-ttu-id="012e3-1475">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="012e3-1475">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1476">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1476">Storage</span></span>

* <span data-ttu-id="012e3-1477">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para</span><span class="sxs-lookup"><span data-stu-id="012e3-1477">Enabled specifying destination-path/prefix for</span></span> `storage blob [upload-batch|download-batch]`

### <a name="vm"></a><span data-ttu-id="012e3-1478">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1478">VM</span></span>

* <span data-ttu-id="012e3-1479">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="012e3-1479">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="012e3-1480">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1480">February 13, 2018</span></span>

<span data-ttu-id="012e3-1481">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="012e3-1481">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1482">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1482">Core</span></span>

* <span data-ttu-id="012e3-1483">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="012e3-1483">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1484">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1484">ACS</span></span>

* <span data-ttu-id="012e3-1485">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1485">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="012e3-1486">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para</span><span class="sxs-lookup"><span data-stu-id="012e3-1486">Changed `aks get-versions` to show Kubernetes versions available for</span></span> `aks create`
* <span data-ttu-id="012e3-1487">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="012e3-1487">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="012e3-1488">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="012e3-1488">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="012e3-1489">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="012e3-1489">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="012e3-1490">Se ha mejorado la confiabilidad al localizar el pod del panel en</span><span class="sxs-lookup"><span data-stu-id="012e3-1490">Improved reliability when locating the dashboard pod for</span></span> `az aks browse`
* <span data-ttu-id="012e3-1491">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="012e3-1491">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="012e3-1492">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1492">Added a message to `az aks install-cli` to help get `kubectl` in</span></span> `$PATH`

### <a name="appservice"></a><span data-ttu-id="012e3-1493">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1493">Appservice</span></span>

* <span data-ttu-id="012e3-1494">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="012e3-1494">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="012e3-1495">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante</span><span class="sxs-lookup"><span data-stu-id="012e3-1495">Added support for default app service plans through</span></span> `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a><span data-ttu-id="012e3-1496">CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-1496">CDN</span></span>

* <span data-ttu-id="012e3-1497">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1497">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1498">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1498">Container</span></span>

* <span data-ttu-id="012e3-1499">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="012e3-1499">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="012e3-1500">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-1500">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="012e3-1501">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-1501">CosmosDB</span></span>

* <span data-ttu-id="012e3-1502">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="012e3-1502">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-1503">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1503">Extension</span></span>

* <span data-ttu-id="012e3-1504">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="012e3-1504">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="012e3-1505">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="012e3-1505">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="012e3-1506">Comentarios</span><span class="sxs-lookup"><span data-stu-id="012e3-1506">Feedback</span></span>

* <span data-ttu-id="012e3-1507">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="012e3-1507">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1508">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1508">Interactive</span></span>

* <span data-ttu-id="012e3-1509">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="012e3-1509">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="012e3-1510">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="012e3-1510">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-1511">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-1511">IoT</span></span>

* <span data-ttu-id="012e3-1512">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="012e3-1512">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="012e3-1513">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="012e3-1513">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="012e3-1514">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1514">Added `--no-wait` support to `iot dps access policy [create|update]` and</span></span> `iot dps linked-hub [create|update]`
* <span data-ttu-id="012e3-1515">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="012e3-1515">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-1516">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1516">Monitor</span></span>

* <span data-ttu-id="012e3-1517">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1517">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1518">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1518">Network</span></span>

* <span data-ttu-id="012e3-1519">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="012e3-1519">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="012e3-1520">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1520">Profile</span></span>

* <span data-ttu-id="012e3-1521">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="012e3-1521">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1522">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1522">Resource</span></span>

* <span data-ttu-id="012e3-1523">Se ha agregado de nuevo</span><span class="sxs-lookup"><span data-stu-id="012e3-1523">Added back</span></span> `feature show`

### <a name="role"></a><span data-ttu-id="012e3-1524">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-1524">Role</span></span>

* <span data-ttu-id="012e3-1525">Se ha agregado el argumento `--available-to-other-tenants` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1525">Added `--available-to-other-tenants` argument to</span></span> `ad app update`

### <a name="sql"></a><span data-ttu-id="012e3-1526">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1526">SQL</span></span>

* <span data-ttu-id="012e3-1527">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1527">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="012e3-1528">Se agregó</span><span class="sxs-lookup"><span data-stu-id="012e3-1528">Added</span></span> `sql db rename`
* <span data-ttu-id="012e3-1529">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="012e3-1529">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1530">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1530">Storage</span></span>

* <span data-ttu-id="012e3-1531">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="012e3-1531">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1532">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1532">VM</span></span>

* <span data-ttu-id="012e3-1533">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="012e3-1533">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="012e3-1534">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="012e3-1534">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="012e3-1535">Corregido</span><span class="sxs-lookup"><span data-stu-id="012e3-1535">Fixed</span></span> `vm boot-diagnostics get-boot-log`


## <a name="january-31-2018"></a><span data-ttu-id="012e3-1536">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1536">January 31, 2018</span></span>

<span data-ttu-id="012e3-1537">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="012e3-1537">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1538">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1538">Core</span></span>

* <span data-ttu-id="012e3-1539">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="012e3-1539">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="012e3-1540">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="012e3-1540">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="012e3-1541">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="012e3-1541">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="012e3-1542">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="012e3-1542">Use `--verbose` to see</span></span>
* <span data-ttu-id="012e3-1543">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="012e3-1543">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1544">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1544">ACS</span></span>

* <span data-ttu-id="012e3-1545">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="012e3-1545">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="012e3-1546">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="012e3-1546">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1547">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1547">Appservice</span></span>

* <span data-ttu-id="012e3-1548">Corregido</span><span class="sxs-lookup"><span data-stu-id="012e3-1548">Fixed</span></span> `webapp log [tail|download]`
* <span data-ttu-id="012e3-1549">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="012e3-1549">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="012e3-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-1550">CDN</span></span>

* <span data-ttu-id="012e3-1551">Se ha corregido un problema de cliente no encontrado en</span><span class="sxs-lookup"><span data-stu-id="012e3-1551">Fixed missing client issue with</span></span> `cdn custom-domain create`

### <a name="cosmosdb"></a><span data-ttu-id="012e3-1552">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-1552">CosmosDB</span></span>

* <span data-ttu-id="012e3-1553">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="012e3-1553">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1554">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1554">Interactive</span></span>

* <span data-ttu-id="012e3-1555">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="012e3-1555">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1556">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1556">Network</span></span>

* <span data-ttu-id="012e3-1557">Se ha agregado protección para `--cert-password` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1557">Added protection for `--cert-password` to</span></span> `application-gateway create`
* <span data-ttu-id="012e3-1558">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="012e3-1558">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="012e3-1559">Se ha agregado protección para `--shared-key` y `--authorization-key` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1559">Added protection for `--shared-key` and `--authorization-key` to</span></span> `vpn-connection create`
* <span data-ttu-id="012e3-1560">Se ha corregido un problema de cliente no encontrado en</span><span class="sxs-lookup"><span data-stu-id="012e3-1560">Fixed missing client issue with</span></span> `asg create`
* <span data-ttu-id="012e3-1561">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en</span><span class="sxs-lookup"><span data-stu-id="012e3-1561">Added `--file-name / -f` parameter for exported names to</span></span> `dns zone export`
* <span data-ttu-id="012e3-1562">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="012e3-1562">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="012e3-1563">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="012e3-1563">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="012e3-1564">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="012e3-1564">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="012e3-1565">Se ha corregido un problema por el que algunos registros se importaban dos veces en</span><span class="sxs-lookup"><span data-stu-id="012e3-1565">Fixed issue where certain records were imported twice with</span></span> `dns zone import`
* <span data-ttu-id="012e3-1566">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="012e3-1566">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="012e3-1567">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1567">Profile</span></span>

* <span data-ttu-id="012e3-1568">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="012e3-1568">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1569">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1569">Resource</span></span>

* <span data-ttu-id="012e3-1570">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="012e3-1570">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1571">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1571">Storage</span></span>

* <span data-ttu-id="012e3-1572">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="012e3-1572">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="012e3-1573">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="012e3-1573">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="012e3-1574">Se ha corregido un error en la opción "-n" en</span><span class="sxs-lookup"><span data-stu-id="012e3-1574">Fixed bug preventing "-n" arg option with</span></span> `storage account check-name`
* <span data-ttu-id="012e3-1575">Se ha agregado la columna "snapshot" a la salida de tabla de</span><span class="sxs-lookup"><span data-stu-id="012e3-1575">Added 'snapshot' column to table output for</span></span> `blob [list|show]`
* <span data-ttu-id="012e3-1576">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="012e3-1576">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1577">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1577">VM</span></span>

* <span data-ttu-id="012e3-1578">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="012e3-1578">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="012e3-1579">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="012e3-1579">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="012e3-1580">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="012e3-1580">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="012e3-1581">Se ha agregado protección para `--admin-password` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1581">Added protection for `--admin-password` to</span></span> `[vm|vmss] create`


## <a name="january-17-2018"></a><span data-ttu-id="012e3-1582">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="012e3-1582">January 17, 2018</span></span>

<span data-ttu-id="012e3-1583">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="012e3-1583">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-1584">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1584">ACR</span></span>

* <span data-ttu-id="012e3-1585">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="012e3-1585">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="012e3-1586">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="012e3-1586">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1587">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1587">ACS</span></span>

* <span data-ttu-id="012e3-1588">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="012e3-1588">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="012e3-1589">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="012e3-1589">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1590">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1590">Appservice</span></span>

* <span data-ttu-id="012e3-1591">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="012e3-1591">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="012e3-1592">Se ha agregado compatibilidad con direcciones URL personalizadas para</span><span class="sxs-lookup"><span data-stu-id="012e3-1592">Added support for custom URLs to</span></span> `browse`
* <span data-ttu-id="012e3-1593">Se ha corregido la compatibilidad con ranuras en</span><span class="sxs-lookup"><span data-stu-id="012e3-1593">Fixed slot support for</span></span> `log tail`

### <a name="backup"></a><span data-ttu-id="012e3-1594">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="012e3-1594">Backup</span></span>

* <span data-ttu-id="012e3-1595">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="012e3-1595">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="012e3-1596">Se han agregado opciones de la cuenta de almacenamiento a</span><span class="sxs-lookup"><span data-stu-id="012e3-1596">Added storage account options to</span></span> `backup restore restore-disks`
* <span data-ttu-id="012e3-1597">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="012e3-1597">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="012e3-1598">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="012e3-1598">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="012e3-1599">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="012e3-1599">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-1600">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1600">Batch</span></span>

* <span data-ttu-id="012e3-1601">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="012e3-1601">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="012e3-1602">Nube</span><span class="sxs-lookup"><span data-stu-id="012e3-1602">Cloud</span></span>

* <span data-ttu-id="012e3-1603">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="012e3-1603">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="012e3-1604">Consumo</span><span class="sxs-lookup"><span data-stu-id="012e3-1604">Consumption</span></span>

* <span data-ttu-id="012e3-1605">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1605">Added new commands for reservations: `consumption reservations summaries` and</span></span> `consumption reservations details`

### <a name="event-grid"></a><span data-ttu-id="012e3-1606">Event Grid</span><span class="sxs-lookup"><span data-stu-id="012e3-1606">Event Grid</span></span>

* <span data-ttu-id="012e3-1607">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1607">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="012e3-1608">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1608">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="012e3-1609">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1609">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="012e3-1610">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="012e3-1610">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="012e3-1611">Se ha agregado el comando</span><span class="sxs-lookup"><span data-stu-id="012e3-1611">Added command</span></span> `eventgrid topic update`
* <span data-ttu-id="012e3-1612">Se ha agregado el comando</span><span class="sxs-lookup"><span data-stu-id="012e3-1612">Added command</span></span> `eventgrid event-subscription update`
* <span data-ttu-id="012e3-1613">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="012e3-1613">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="012e3-1614">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="012e3-1614">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-1615">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-1615">Interactive</span></span>

* <span data-ttu-id="012e3-1616">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="012e3-1616">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="012e3-1617">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="012e3-1617">Fixed errors on startup</span></span>
* <span data-ttu-id="012e3-1618">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="012e3-1618">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-1619">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-1619">IoT</span></span>

* <span data-ttu-id="012e3-1620">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="012e3-1620">Added support for device provisioning service</span></span>
* <span data-ttu-id="012e3-1621">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1621">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="012e3-1622">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-1622">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-1623">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1623">Monitor</span></span>

* <span data-ttu-id="012e3-1624">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1624">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="012e3-1625">El parámetro `--name` ahora es obligatorio en</span><span class="sxs-lookup"><span data-stu-id="012e3-1625">The `--name` parameter is now required for</span></span> `az monitor diagnostic-settings create`
* <span data-ttu-id="012e3-1626">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="012e3-1626">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1627">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1627">Network</span></span>

* <span data-ttu-id="012e3-1628">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con</span><span class="sxs-lookup"><span data-stu-id="012e3-1628">Fixed issue when trying to change to/from active-standby mode with</span></span> `vnet-gateway update`
* <span data-ttu-id="012e3-1629">Se ha agregado compatibilidad con HTTP2 a</span><span class="sxs-lookup"><span data-stu-id="012e3-1629">Added support for HTTP2 to</span></span> `application-gateway [create|update]`

### <a name="profile"></a><span data-ttu-id="012e3-1630">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1630">Profile</span></span>

* <span data-ttu-id="012e3-1631">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="012e3-1631">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="012e3-1632">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-1632">Role</span></span>

* <span data-ttu-id="012e3-1633">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="012e3-1633">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="012e3-1634">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="012e3-1634">Service Fabric</span></span>

* <span data-ttu-id="012e3-1635">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="012e3-1635">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="012e3-1636">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="012e3-1636">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1637">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1637">VM</span></span>

* <span data-ttu-id="012e3-1638">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para</span><span class="sxs-lookup"><span data-stu-id="012e3-1638">[PREVIEW] Cross-zone support for</span></span> `vmss`
* <span data-ttu-id="012e3-1639">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="012e3-1639">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="012e3-1640">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="012e3-1640">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="012e3-1641">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="012e3-1641">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="012e3-1642">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="012e3-1642">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="012e3-1643">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1643">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to</span></span> `[vm|vmss] create`
* <span data-ttu-id="012e3-1644">Se han corregido problemas de error en</span><span class="sxs-lookup"><span data-stu-id="012e3-1644">Fixed error issues with</span></span> `[vm|vmss] create`
* <span data-ttu-id="012e3-1645">Se ha corregido el uso excesivo de recursos producido por</span><span class="sxs-lookup"><span data-stu-id="012e3-1645">Fixed excessive resource usage caused by</span></span> `vm image list --all`

## <a name="december-19-2017"></a><span data-ttu-id="012e3-1646">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1646">December 19, 2017</span></span>

<span data-ttu-id="012e3-1647">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="012e3-1647">Version 2.0.23</span></span>

* <span data-ttu-id="012e3-1648">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="012e3-1648">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1649">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1649">Container</span></span>

* <span data-ttu-id="012e3-1650">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1650">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1651">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1651">Network</span></span>

* <span data-ttu-id="012e3-1652">Se ha agregado el argumento `--disable-bgp-route-propagation` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1652">Added `--disable-bgp-route-propagation` argument to</span></span> `route-table [create|update]`
* <span data-ttu-id="012e3-1653">Se ha agregado el argumento `--ip-tags` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1653">Added `--ip-tags` argument to</span></span> `public-ip [create|update]`

### <a name="storage"></a><span data-ttu-id="012e3-1654">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1654">Storage</span></span>

* <span data-ttu-id="012e3-1655">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="012e3-1655">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1656">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1656">VM</span></span>

* <span data-ttu-id="012e3-1657">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="012e3-1657">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="012e3-1658">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1658">December 5, 2017</span></span>

<span data-ttu-id="012e3-1659">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="012e3-1659">Version 2.0.22</span></span>

* <span data-ttu-id="012e3-1660">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1660">Removed `az component` commands.</span></span> <span data-ttu-id="012e3-1661">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="012e3-1661">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1662">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1662">Core</span></span>
* <span data-ttu-id="012e3-1663">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="012e3-1663">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="012e3-1664">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="012e3-1664">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1665">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1665">ACS</span></span>

* <span data-ttu-id="012e3-1666">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="012e3-1666">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="012e3-1667">Se mejoraron los informes de errores de</span><span class="sxs-lookup"><span data-stu-id="012e3-1667">Improved error reporting for</span></span> `acs create`
* <span data-ttu-id="012e3-1668">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="012e3-1668">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="012e3-1669">Advisor</span><span class="sxs-lookup"><span data-stu-id="012e3-1669">Advisor</span></span>

* <span data-ttu-id="012e3-1670">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="012e3-1670">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1671">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1671">Appservice</span></span>

* <span data-ttu-id="012e3-1672">Se ha corregido la generación de nombres de certificado con</span><span class="sxs-lookup"><span data-stu-id="012e3-1672">Fixed cert name generation with</span></span> `webapp config ssl upload`
* <span data-ttu-id="012e3-1673">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="012e3-1673">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="012e3-1674">Se ha agregado el valor predeterminado para</span><span class="sxs-lookup"><span data-stu-id="012e3-1674">Added default value for</span></span> `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a><span data-ttu-id="012e3-1675">Consumo</span><span class="sxs-lookup"><span data-stu-id="012e3-1675">Consumption</span></span>

* <span data-ttu-id="012e3-1676">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="012e3-1676">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1677">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1677">Container</span></span>

* <span data-ttu-id="012e3-1678">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="012e3-1678">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-1679">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1679">Monitor</span></span>

* <span data-ttu-id="012e3-1680">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="012e3-1680">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1681">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1681">Resource</span></span>

* <span data-ttu-id="012e3-1682">Se ha agregado el argumento `--include-response-body` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1682">Added `--include-response-body` argument to</span></span> `resource show`

### <a name="role"></a><span data-ttu-id="012e3-1683">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-1683">Role</span></span>

* <span data-ttu-id="012e3-1684">Se ha agregado la presentación de las asignaciones predeterminadas de los administradores "clásicos" a</span><span class="sxs-lookup"><span data-stu-id="012e3-1684">Added display of default assignments for "classic" administraors to</span></span> `role assignment list`
* <span data-ttu-id="012e3-1685">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="012e3-1685">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="012e3-1686">Se mejoraron los informes de errores de</span><span class="sxs-lookup"><span data-stu-id="012e3-1686">Improved error reporting for</span></span> `ad sp create-for-rbac`

### <a name="sql"></a><span data-ttu-id="012e3-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1687">SQL</span></span>

* <span data-ttu-id="012e3-1688">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="012e3-1688">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="012e3-1689">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="012e3-1689">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1690">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1690">VM</span></span>

* <span data-ttu-id="012e3-1691">Se ha agregado información de zona a</span><span class="sxs-lookup"><span data-stu-id="012e3-1691">Added zone information to</span></span> `az vm list-skus`


## <a name="november-14-2017"></a><span data-ttu-id="012e3-1692">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1692">November 14, 2017</span></span>

<span data-ttu-id="012e3-1693">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="012e3-1693">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-1694">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1694">ACR</span></span>

* <span data-ttu-id="012e3-1695">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="012e3-1695">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="012e3-1696">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1696">ACS</span></span>

* <span data-ttu-id="012e3-1697">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="012e3-1697">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="012e3-1698">Se ha dejado de usar la opción `--orchestrator-release` para</span><span class="sxs-lookup"><span data-stu-id="012e3-1698">Deprecated `--orchestrator-release` option for</span></span> `acs create`
* <span data-ttu-id="012e3-1699">Se ha cambiado el tamaño de máquina virtual predeterminado para AKS a</span><span class="sxs-lookup"><span data-stu-id="012e3-1699">Changed default VM size for AKS to</span></span> `Standard_D1_v2`
* <span data-ttu-id="012e3-1700">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="012e3-1700">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="012e3-1701">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="012e3-1701">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1702">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1702">Appservice</span></span>

* <span data-ttu-id="012e3-1703">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="012e3-1703">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="012e3-1704">Se ha agregado la opción `--docker-container-logging` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1704">Added `--docker-container-logging` option to</span></span> `az webapp log config`
* <span data-ttu-id="012e3-1705">Se ha quitado la opción `storage` del parámetro `--web-server-logging` de</span><span class="sxs-lookup"><span data-stu-id="012e3-1705">Removed the `storage` option from the parameter `--web-server-logging` of</span></span> `az webapp log config`
* <span data-ttu-id="012e3-1706">Se mejoraron los mensajes de error de</span><span class="sxs-lookup"><span data-stu-id="012e3-1706">Improved error messages for</span></span> `deployment user set`
* <span data-ttu-id="012e3-1707">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="012e3-1707">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="012e3-1708">Corregido</span><span class="sxs-lookup"><span data-stu-id="012e3-1708">Fixed</span></span> `list-locations`

### <a name="batch"></a><span data-ttu-id="012e3-1709">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1709">Batch</span></span>

* <span data-ttu-id="012e3-1710">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="012e3-1710">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="012e3-1711">Batchai</span><span class="sxs-lookup"><span data-stu-id="012e3-1711">Batchai</span></span>

* <span data-ttu-id="012e3-1712">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1712">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="012e3-1713">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1713">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="012e3-1714">Se ha corregido la documentación de `job list-files` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1714">Fixed documentation for `job list-files` and</span></span> `job stream-file`
* <span data-ttu-id="012e3-1715">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="012e3-1715">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="012e3-1716">Nube</span><span class="sxs-lookup"><span data-stu-id="012e3-1716">Cloud</span></span>

* <span data-ttu-id="012e3-1717">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="012e3-1717">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1718">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1718">Container</span></span>

* <span data-ttu-id="012e3-1719">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="012e3-1719">Added support to open multiple ports</span></span>
* <span data-ttu-id="012e3-1720">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="012e3-1720">Added container group restart policy</span></span>
* <span data-ttu-id="012e3-1721">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="012e3-1721">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="012e3-1722">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="012e3-1722">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="012e3-1723">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="012e3-1723">Data Lake Analytics</span></span>

* <span data-ttu-id="012e3-1724">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="012e3-1724">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="012e3-1725">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="012e3-1725">Data Lake Store</span></span>

* <span data-ttu-id="012e3-1726">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="012e3-1726">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="012e3-1727">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1727">Extension</span></span>

* <span data-ttu-id="012e3-1728">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="012e3-1728">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="012e3-1729">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="012e3-1729">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-1730">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-1730">IoT</span></span>

* <span data-ttu-id="012e3-1731">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="012e3-1731">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-1732">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1732">Monitor</span></span>

* <span data-ttu-id="012e3-1733">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1733">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1734">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1734">Network</span></span>

* <span data-ttu-id="012e3-1735">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="012e3-1735">Added support for CAA DNS records</span></span>
* <span data-ttu-id="012e3-1736">Se ha corregido un problema por el que los puntos de conexión no se podían actualizar con</span><span class="sxs-lookup"><span data-stu-id="012e3-1736">Fixed issue where endpoints could not be updated with</span></span> `traffic-manager profile update`
* <span data-ttu-id="012e3-1737">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1737">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="012e3-1738">Se ha corregido un problema por el que no se importaban correctamente los nombres DNS relativos con</span><span class="sxs-lookup"><span data-stu-id="012e3-1738">Fixed issue where relative DNS names were incorrectly imported by</span></span> `dns zone import`

### <a name="reservations"></a><span data-ttu-id="012e3-1739">Reservations</span><span class="sxs-lookup"><span data-stu-id="012e3-1739">Reservations</span></span>

* <span data-ttu-id="012e3-1740">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="012e3-1740">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1741">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1741">Resource</span></span>

* <span data-ttu-id="012e3-1742">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1742">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1743">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1743">SQL</span></span>

* <span data-ttu-id="012e3-1744">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1744">Added `--ignore-missing-vnet-service-endpoint` parameter to</span></span> `sql server vnet-rule [create|update]`

### <a name="storage"></a><span data-ttu-id="012e3-1745">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1745">Storage</span></span>

* <span data-ttu-id="012e3-1746">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="012e3-1746">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="012e3-1747">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="012e3-1747">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="012e3-1748">Se ha corregido un error que impedía el uso de `--source-uri` con</span><span class="sxs-lookup"><span data-stu-id="012e3-1748">Fixed bug that prevented using `--source-uri` with</span></span> `storage [blob|file] copy start-batch`
* <span data-ttu-id="012e3-1749">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con</span><span class="sxs-lookup"><span data-stu-id="012e3-1749">Added commands to glob and delete multiple objects with</span></span> `storage [blob|file] delete-batch`
* <span data-ttu-id="012e3-1750">Se ha corregido un problema al habilitar las métricas con</span><span class="sxs-lookup"><span data-stu-id="012e3-1750">Fixed issue when enabling metrics with</span></span> `storage metrics update`
* <span data-ttu-id="012e3-1751">Se ha corregido un problema con los archivos de más de 200 GB cuando se usa</span><span class="sxs-lookup"><span data-stu-id="012e3-1751">Fixed issue with files over 200GB when using</span></span> `storage blob upload-batch`
* <span data-ttu-id="012e3-1752">Se ha corregido un problema por el que se ignoraba `--bypass` y `--default-action` en</span><span class="sxs-lookup"><span data-stu-id="012e3-1752">Fixed issue where `--bypass` and `--default-action` were ignored by</span></span> `storage account [create|update]`

### <a name="vm"></a><span data-ttu-id="012e3-1753">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1753">VM</span></span>

* <span data-ttu-id="012e3-1754">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="012e3-1754">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="012e3-1755">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="012e3-1755">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="012e3-1756">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="012e3-1756">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="012e3-1757">Se ha cambiado el nombre de `vm format-secret` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1757">Renamed `vm format-secret` to</span></span> `vm secret format`
* <span data-ttu-id="012e3-1758">Se ha agregado el argumento `--encrypt format` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1758">Added `--encrypt format` argument to</span></span> `vm encryption enable`

## <a name="october-24-2017"></a><span data-ttu-id="012e3-1759">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1759">October 24, 2017</span></span>

<span data-ttu-id="012e3-1760">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="012e3-1760">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1761">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1761">Core</span></span>

* <span data-ttu-id="012e3-1762">Se actualizó `2017-03-09-profile` para que utilice la API `MGMT_STORAGE` de la versión</span><span class="sxs-lookup"><span data-stu-id="012e3-1762">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version</span></span> `2016-01-01`

### <a name="acr"></a><span data-ttu-id="012e3-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-1763">ACR</span></span>

* <span data-ttu-id="012e3-1764">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="012e3-1764">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="012e3-1765">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="012e3-1765">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="012e3-1766">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="012e3-1766">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1767">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1767">ACS</span></span>

* <span data-ttu-id="012e3-1768">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="012e3-1768">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="012e3-1769">En Kubernetes, se ha corregido</span><span class="sxs-lookup"><span data-stu-id="012e3-1769">Fixed kubernetes</span></span> `get-credentials`

### <a name="appservice"></a><span data-ttu-id="012e3-1770">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1770">Appservice</span></span>

* <span data-ttu-id="012e3-1771">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="012e3-1771">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="012e3-1772">Componente</span><span class="sxs-lookup"><span data-stu-id="012e3-1772">Component</span></span>

* <span data-ttu-id="012e3-1773">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="012e3-1773">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-1774">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-1774">Monitor</span></span>

* <span data-ttu-id="012e3-1775">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1775">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1776">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1776">Resource</span></span>

* <span data-ttu-id="012e3-1777">Se ha corregido la incompatibilidad con la versión más reciente de la dependencia msrest en</span><span class="sxs-lookup"><span data-stu-id="012e3-1777">Fixed incompatibility with most recent version of msrest dependency in</span></span> `group export`
* <span data-ttu-id="012e3-1778">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="012e3-1778">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1779">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1779">VM</span></span>

* <span data-ttu-id="012e3-1780">Se ha agregado el argumento `--accelerated-networking` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1780">Added `--accelerated-networking` argument to</span></span> `vmss create`


## <a name="october-9-2017"></a><span data-ttu-id="012e3-1781">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1781">October 9, 2017</span></span>

<span data-ttu-id="012e3-1782">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="012e3-1782">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1783">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1783">Core</span></span>

* <span data-ttu-id="012e3-1784">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="012e3-1784">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1785">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1785">Appservice</span></span>

* <span data-ttu-id="012e3-1786">Se ha agregado una actualización genérica con el nuevo comando</span><span class="sxs-lookup"><span data-stu-id="012e3-1786">Added generic update with new command</span></span> `webapp update`

### <a name="batch"></a><span data-ttu-id="012e3-1787">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1787">Batch</span></span>

* <span data-ttu-id="012e3-1788">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="012e3-1788">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="012e3-1789">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="012e3-1789">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="012e3-1790">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1790">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="012e3-1791">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="012e3-1791">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="012e3-1792">Batchai</span><span class="sxs-lookup"><span data-stu-id="012e3-1792">Batchai</span></span>

* <span data-ttu-id="012e3-1793">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1793">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-1794">Keyvault</span><span class="sxs-lookup"><span data-stu-id="012e3-1794">Keyvault</span></span>

* <span data-ttu-id="012e3-1795">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="012e3-1795">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="012e3-1796">N.º 4448</span><span class="sxs-lookup"><span data-stu-id="012e3-1796">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="012e3-1797">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1797">Network</span></span>

* <span data-ttu-id="012e3-1798">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="012e3-1798">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="012e3-1799">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="012e3-1799">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1800">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1800">Resource</span></span>

* <span data-ttu-id="012e3-1801">Se ha agregado compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso a</span><span class="sxs-lookup"><span data-stu-id="012e3-1801">Added support for `--resource-group/-g` options for resource group name to</span></span> `group`
* <span data-ttu-id="012e3-1802">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="012e3-1802">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="012e3-1803">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="012e3-1803">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="012e3-1804">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1804">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1805">Sql</span><span class="sxs-lookup"><span data-stu-id="012e3-1805">Sql</span></span>

* <span data-ttu-id="012e3-1806">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="012e3-1806">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="012e3-1807">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="012e3-1807">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="012e3-1808">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="012e3-1808">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1809">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1809">Storage</span></span>

* <span data-ttu-id="012e3-1810">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="012e3-1810">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1811">Vm</span><span class="sxs-lookup"><span data-stu-id="012e3-1811">Vm</span></span>

* <span data-ttu-id="012e3-1812">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="012e3-1812">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="012e3-1813">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a</span><span class="sxs-lookup"><span data-stu-id="012e3-1813">[PREVIEW] Added support for rolling upgrade to</span></span> `vmss create`
* <span data-ttu-id="012e3-1814">Se ha agregado compatibilidad para actualizar la configuración de cifrado con</span><span class="sxs-lookup"><span data-stu-id="012e3-1814">Added support for updating encryption settings with</span></span> `vm encryption enable`
* <span data-ttu-id="012e3-1815">Se ha agregado el parámetro `--os-disk-size-gb` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1815">Added `--os-disk-size-gb` parameter to</span></span> `vm create`
* <span data-ttu-id="012e3-1816">Se ha agregado el parámetro `--license-type` para Windows a</span><span class="sxs-lookup"><span data-stu-id="012e3-1816">Added `--license-type` parameter for Windows to</span></span> `vmss create`


## <a name="september-22-2017"></a><span data-ttu-id="012e3-1817">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1817">September 22, 2017</span></span>

<span data-ttu-id="012e3-1818">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="012e3-1818">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-1819">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1819">Resource</span></span>

* <span data-ttu-id="012e3-1820">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="012e3-1820">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="012e3-1821">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="012e3-1821">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="012e3-1822">Se ha agregado compatibilidad para las plantillas y definiciones de interfaz de usuario a</span><span class="sxs-lookup"><span data-stu-id="012e3-1822">Added support for UI definitions and templates to</span></span> `managedapp definition create`
* <span data-ttu-id="012e3-1823">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y de `applianceDefinitions` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1823">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to</span></span> `applicationDefinitions`

### <a name="network"></a><span data-ttu-id="012e3-1824">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1824">Network</span></span>

* <span data-ttu-id="012e3-1825">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="012e3-1825">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="012e3-1826">Se ha agregado compatibilidad con el emparejamiento de Microsoft IPv6 a</span><span class="sxs-lookup"><span data-stu-id="012e3-1826">Added support for IPv6 Microsoft Peering to</span></span> `express-route`
* <span data-ttu-id="012e3-1827">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="012e3-1827">Added `asg` application security group commands</span></span>
* <span data-ttu-id="012e3-1828">Se ha agregado el argumento `--application-security-groups` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1828">Added `--application-security-groups` argument to</span></span> `nic [create|ip-config create|ip-config update]`
* <span data-ttu-id="012e3-1829">Se han agregado los argumentos `--source-asgs` y `--destination-asgs` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1829">Added `--source-asgs` and `--destination-asgs` arguments to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="012e3-1830">Se han agregado los argumentos `--ddos-protection` y `--vm-protection` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1830">Added `--ddos-protection` and `--vm-protection` arguments to</span></span> `vnet [create|update]`
* <span data-ttu-id="012e3-1831">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1831">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1832">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1832">Storage</span></span>

* <span data-ttu-id="012e3-1833">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="012e3-1833">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="012e3-1834">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="012e3-1834">Eventgrid</span></span>

* <span data-ttu-id="012e3-1835">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="012e3-1835">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1836">SQL</span></span>

* <span data-ttu-id="012e3-1837">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="012e3-1837">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="012e3-1838">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="012e3-1838">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="012e3-1839">Se ha agregado el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1839">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and</span></span> `dw [create|update]`

### <a name="keyvault"></a><span data-ttu-id="012e3-1840">Keyvault</span><span class="sxs-lookup"><span data-stu-id="012e3-1840">Keyvault</span></span>

* <span data-ttu-id="012e3-1841">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="012e3-1841">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1842">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1842">VM</span></span>

* <span data-ttu-id="012e3-1843">Se ha agregado compatibilidad con las zonas de disponibilidad a</span><span class="sxs-lookup"><span data-stu-id="012e3-1843">Added for support to availability zone to</span></span> `[vm|vmss|disk] create`
* <span data-ttu-id="012e3-1844">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="012e3-1844">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="012e3-1845">Se ha agregado el argumento `--asgs` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1845">Added `--asgs` argument to</span></span> `vm create`
* <span data-ttu-id="012e3-1846">Se ha agregado compatibilidad para ejecutar comandos en máquinas virtuales con</span><span class="sxs-lookup"><span data-stu-id="012e3-1846">Added support for running commands on VMs with</span></span> `vm run-command`
* <span data-ttu-id="012e3-1847">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el cifrado de disco VMSS con</span><span class="sxs-lookup"><span data-stu-id="012e3-1847">[PREVIEW] Added support for VMSS disk encryption with</span></span> `vmss encryption`
* <span data-ttu-id="012e3-1848">Se ha agregado compatibilidad para realizar el mantenimiento en máquinas virtuales con</span><span class="sxs-lookup"><span data-stu-id="012e3-1848">Added support for performing maintenance on VMs with</span></span> `vm perform-maintenance`

### <a name="acs"></a><span data-ttu-id="012e3-1849">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1849">ACS</span></span>

* <span data-ttu-id="012e3-1850">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1850">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1851">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1851">Appservice</span></span>

* <span data-ttu-id="012e3-1852">Se ha agregado la capacidad para actualizar y mostrar la configuración de autenticación con</span><span class="sxs-lookup"><span data-stu-id="012e3-1852">Added ability to update and show authentication settings with</span></span> `webapp auth [update|show]`

### <a name="backup"></a><span data-ttu-id="012e3-1853">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="012e3-1853">Backup</span></span>

* <span data-ttu-id="012e3-1854">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-1854">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="012e3-1855">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1855">September 11, 2017</span></span>

<span data-ttu-id="012e3-1856">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="012e3-1856">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="012e3-1857">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1857">Core</span></span>

* <span data-ttu-id="012e3-1858">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="012e3-1858">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="012e3-1859">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="012e3-1859">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1860">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1860">Acs</span></span>

* <span data-ttu-id="012e3-1861">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1861">Added `acs list-locations` command</span></span>
* <span data-ttu-id="012e3-1862">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="012e3-1862">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1863">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1863">Appservice</span></span>

* <span data-ttu-id="012e3-1864">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="012e3-1864">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="012e3-1865">CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-1865">CDN</span></span>

* <span data-ttu-id="012e3-1866">Se ha corregido el error "No se puede iterar en CustomDomain" para</span><span class="sxs-lookup"><span data-stu-id="012e3-1866">Fixed 'CustomDomain is not interable' bug for</span></span> `cdn custom-domain create`

### <a name="extension"></a><span data-ttu-id="012e3-1867">Extensión</span><span class="sxs-lookup"><span data-stu-id="012e3-1867">Extension</span></span>

* <span data-ttu-id="012e3-1868">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="012e3-1868">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-1869">Keyvault</span><span class="sxs-lookup"><span data-stu-id="012e3-1869">Keyvault</span></span>

* <span data-ttu-id="012e3-1870">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para</span><span class="sxs-lookup"><span data-stu-id="012e3-1870">Fixed issue where permissions were case sensitive for</span></span> `keyvault set-policy`

### <a name="network"></a><span data-ttu-id="012e3-1871">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1871">Network</span></span>

* <span data-ttu-id="012e3-1872">Se ha cambiado el nombre de `vnet list-private-access-services` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1872">Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="012e3-1873">Se ha cambiado el nombre del argumento `--private-access-services` a `--service-endpoints` para</span><span class="sxs-lookup"><span data-stu-id="012e3-1873">Renamed `--private-access-services` argument to `--service-endpoints` for</span></span> `vnet subnet create/update`
* <span data-ttu-id="012e3-1874">Se ha agregado compatibilidad para varios intervalos de direcciones IP y puertos a</span><span class="sxs-lookup"><span data-stu-id="012e3-1874">Added support for multiple IP ranges and port ranges to</span></span> `nsg rule create/update`
* <span data-ttu-id="012e3-1875">Se ha agregado compatibilidad para SKU a</span><span class="sxs-lookup"><span data-stu-id="012e3-1875">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="012e3-1876">Se ha agregado compatibilidad para SKU a</span><span class="sxs-lookup"><span data-stu-id="012e3-1876">Added support for SKU to</span></span> `public-ip create`

### <a name="resource"></a><span data-ttu-id="012e3-1877">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-1877">Resource</span></span>

* <span data-ttu-id="012e3-1878">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y</span><span class="sxs-lookup"><span data-stu-id="012e3-1878">Allow passing in resource policy parameter definitions in `policy definition create`, and</span></span> `policy definition update`
* <span data-ttu-id="012e3-1879">Se permite pasar valores de parámetro para</span><span class="sxs-lookup"><span data-stu-id="012e3-1879">Allow passing in parameter values for</span></span> `policy assignment create`
* <span data-ttu-id="012e3-1880">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="012e3-1880">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="012e3-1881">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="012e3-1881">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-1882">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-1882">SQL</span></span>

* <span data-ttu-id="012e3-1883">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1883">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1884">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1884">VM</span></span>

* <span data-ttu-id="012e3-1885">Problema corregido: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1885">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="012e3-1886">Problema corregido: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="012e3-1886">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="012e3-1887">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1887">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="012e3-1888">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="012e3-1888">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="012e3-1889">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="012e3-1889">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="012e3-1890">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1890">August 31, 2017</span></span>

<span data-ttu-id="012e3-1891">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="012e3-1891">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-1892">Keyvault</span><span class="sxs-lookup"><span data-stu-id="012e3-1892">Keyvault</span></span>

* <span data-ttu-id="012e3-1893">Se ha corregido el error que se producía al intentar resolver automáticamente la codificación del secreto con</span><span class="sxs-lookup"><span data-stu-id="012e3-1893">Fixed bug when trying to automatically resolve secret encoding with</span></span> `secret download`

### <a name="sf"></a><span data-ttu-id="012e3-1894">Sf</span><span class="sxs-lookup"><span data-stu-id="012e3-1894">Sf</span></span>

* <span data-ttu-id="012e3-1895">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="012e3-1895">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1896">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1896">Storage</span></span>

* <span data-ttu-id="012e3-1897">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="012e3-1897">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="012e3-1898">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="012e3-1898">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="012e3-1899">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1899">August 28, 2017</span></span>

<span data-ttu-id="012e3-1900">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="012e3-1900">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="012e3-1901">CLI</span><span class="sxs-lookup"><span data-stu-id="012e3-1901">CLI</span></span>

* <span data-ttu-id="012e3-1902">Se ha agregado una nota legal a</span><span class="sxs-lookup"><span data-stu-id="012e3-1902">Added legal note to</span></span> `--version`

### <a name="acs"></a><span data-ttu-id="012e3-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1903">ACS</span></span>

* <span data-ttu-id="012e3-1904">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-1904">Corrected preview regions</span></span>
* <span data-ttu-id="012e3-1905">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="012e3-1905">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="012e3-1906">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="012e3-1906">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1907">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1907">Appservice</span></span>

* <span data-ttu-id="012e3-1908">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de</span><span class="sxs-lookup"><span data-stu-id="012e3-1908">[BREAKING CHANGE] Fixed inconsistencies in the output of</span></span> `az webapp config appsettings [delete|set]`
* <span data-ttu-id="012e3-1909">Se ha agregado un nuevo alias de `-i` para</span><span class="sxs-lookup"><span data-stu-id="012e3-1909">Added a new alias of `-i` for</span></span> `az webapp config container set --docker-custom-image-name`
* <span data-ttu-id="012e3-1910">Se ha expuesto</span><span class="sxs-lookup"><span data-stu-id="012e3-1910">Exposed</span></span> `az webapp log show`
* <span data-ttu-id="012e3-1911">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="012e3-1911">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="012e3-1912">Problema corregido: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="012e3-1912">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-1913">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-1913">IoT</span></span>

* <span data-ttu-id="012e3-1914">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="012e3-1914">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1915">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1915">Network</span></span>

* <span data-ttu-id="012e3-1916">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a</span><span class="sxs-lookup"><span data-stu-id="012e3-1916">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="012e3-1917">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para</span><span class="sxs-lookup"><span data-stu-id="012e3-1917">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for</span></span> `vnet subnet [create|update]`
* <span data-ttu-id="012e3-1918">Se ha agregado compatibilidad con varios intervalos de direcciones IP y puertos a</span><span class="sxs-lookup"><span data-stu-id="012e3-1918">Added support for multiple IP and port ranges to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="012e3-1919">Se ha agregado compatibilidad para SKU a</span><span class="sxs-lookup"><span data-stu-id="012e3-1919">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="012e3-1920">Se ha agregado compatibilidad para SKU a</span><span class="sxs-lookup"><span data-stu-id="012e3-1920">Added support for SKU to</span></span> `public-ip create`

### <a name="profile"></a><span data-ttu-id="012e3-1921">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1921">Profile</span></span>

* <span data-ttu-id="012e3-1922">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="012e3-1922">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="012e3-1923">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="012e3-1923">Service Fabric</span></span>

* <span data-ttu-id="012e3-1924">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-1924">Preview release</span></span>
* <span data-ttu-id="012e3-1925">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1925">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="012e3-1926">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="012e3-1926">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="012e3-1927">Se ha agregado compatibilidad para</span><span class="sxs-lookup"><span data-stu-id="012e3-1927">Added support for empty</span></span> `registry_cred`

### <a name="storage"></a><span data-ttu-id="012e3-1928">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1928">Storage</span></span>

* <span data-ttu-id="012e3-1929">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="012e3-1929">Enabled setting blob tier</span></span>
* <span data-ttu-id="012e3-1930">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="012e3-1930">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="012e3-1931">Se han incorporado comandos para agregar reglas de red virtual y reglas basadas en IP a</span><span class="sxs-lookup"><span data-stu-id="012e3-1931">Added commands to add VNET rules and IP based rules to</span></span> `storage account network-rule`
* <span data-ttu-id="012e3-1932">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="012e3-1932">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="012e3-1933">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="012e3-1933">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="012e3-1934">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="012e3-1934">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1935">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1935">VM</span></span>

* <span data-ttu-id="012e3-1936">Se ha corregido el problema por el que se mostraba información errónea para `vmss get-instance-view` al usar</span><span class="sxs-lookup"><span data-stu-id="012e3-1936">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using</span></span> `--instance-id *`
* <span data-ttu-id="012e3-1937">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1937">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="012e3-1938">Se han quitado los nombres de personas de la lista de nombres de administrador no permitidos para</span><span class="sxs-lookup"><span data-stu-id="012e3-1938">Removed human names from the admin name blacklist for</span></span> `[vm|vmss] create`
* <span data-ttu-id="012e3-1939">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="012e3-1939">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="012e3-1940">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="012e3-1940">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="012e3-1941">Se ha corregido un problema por el que el argumento `--no-wait` no funcionaba con</span><span class="sxs-lookup"><span data-stu-id="012e3-1941">Fixed issue where `--no-wait` argument did not work wth</span></span> `vm availability-set create`


## <a name="august-15-2017"></a><span data-ttu-id="012e3-1942">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1942">August 15, 2017</span></span>

<span data-ttu-id="012e3-1943">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="012e3-1943">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1944">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1944">ACS</span></span>

* <span data-ttu-id="012e3-1945">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="012e3-1945">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-1946">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-1946">Appservice</span></span>

* <span data-ttu-id="012e3-1947">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="012e3-1947">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="012e3-1948">Event Grid</span><span class="sxs-lookup"><span data-stu-id="012e3-1948">Event Grid</span></span>

* <span data-ttu-id="012e3-1949">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="012e3-1949">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="012e3-1950">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1950">August 11, 2017</span></span>

<span data-ttu-id="012e3-1951">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="012e3-1951">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-1952">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-1952">ACS</span></span>

* <span data-ttu-id="012e3-1953">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-1953">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="012e3-1954">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-1954">Batch</span></span>

* <span data-ttu-id="012e3-1955">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="012e3-1955">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="012e3-1956">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="012e3-1956">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="012e3-1957">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1957">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="012e3-1958">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="012e3-1958">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="012e3-1959">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="012e3-1959">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="012e3-1960">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="012e3-1960">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="012e3-1961">Componente</span><span class="sxs-lookup"><span data-stu-id="012e3-1961">Component</span></span>

* <span data-ttu-id="012e3-1962">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="012e3-1962">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="012e3-1963">Contenedor</span><span class="sxs-lookup"><span data-stu-id="012e3-1963">Container</span></span>

* `create`<span data-ttu-id="012e3-1964">: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="012e3-1964">: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="012e3-1965">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="012e3-1965">Data Lake Store</span></span>

* <span data-ttu-id="012e3-1966">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="012e3-1966">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="012e3-1967">Event Grid</span><span class="sxs-lookup"><span data-stu-id="012e3-1967">Event Grid</span></span>

* <span data-ttu-id="012e3-1968">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="012e3-1968">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="012e3-1969">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-1969">Network</span></span>

* `lb`<span data-ttu-id="012e3-1970">: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="012e3-1970">: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* `application-gateway {subresource} delete`<span data-ttu-id="012e3-1971">: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1971">: Fixed issue where `--no-wait` was not honored</span></span>
* `application-gateway http-settings update`<span data-ttu-id="012e3-1972">: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="012e3-1972">: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="012e3-1973">Se ha corregido un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con</span><span class="sxs-lookup"><span data-stu-id="012e3-1973">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with</span></span> `az network vpn-connection ipsec-policy add`

### <a name="profile"></a><span data-ttu-id="012e3-1974">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-1974">Profile</span></span>

* `account list`<span data-ttu-id="012e3-1975">: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="012e3-1975">: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-1976">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-1976">Storage</span></span>

* <span data-ttu-id="012e3-1977">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="012e3-1977">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-1978">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-1978">VM</span></span>

* `availability-set`<span data-ttu-id="012e3-1979">: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="012e3-1979">: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="012e3-1980">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="012e3-1980">Exposed `list-skus` command</span></span>
* <span data-ttu-id="012e3-1981">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="012e3-1981">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="012e3-1982">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="012e3-1982">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="012e3-1983">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="012e3-1983">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="012e3-1984">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-1984">July 28, 2017</span></span>

<span data-ttu-id="012e3-1985">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="012e3-1985">Version 2.0.12</span></span>

* <span data-ttu-id="012e3-1986">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="012e3-1986">Added container commands</span></span>
* <span data-ttu-id="012e3-1987">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="012e3-1987">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="012e3-1988">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-1988">Core</span></span>

* <span data-ttu-id="012e3-1989">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="012e3-1989">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="012e3-1990">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="012e3-1990">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="012e3-1991">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="012e3-1991">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="012e3-1992">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="012e3-1992">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="012e3-1993">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="012e3-1993">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="012e3-1994">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="012e3-1994">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="012e3-1995">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="012e3-1995">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="012e3-1996">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="012e3-1996">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="012e3-1997">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="012e3-1997">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="012e3-1998">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="012e3-1998">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="012e3-1999">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="012e3-1999">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="012e3-2000">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="012e3-2000">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="012e3-2001">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="012e3-2001">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="012e3-2002">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="012e3-2002">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="012e3-2003">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="012e3-2003">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="012e3-2004">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="012e3-2004">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="012e3-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="012e3-2005">ACR</span></span>

* <span data-ttu-id="012e3-2006">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="012e3-2006">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="012e3-2007">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="012e3-2007">Support SKU update for managed registries</span></span>
* <span data-ttu-id="012e3-2008">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="012e3-2008">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="012e3-2009">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="012e3-2009">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="012e3-2010">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="012e3-2010">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="012e3-2011">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="012e3-2011">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-2012">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-2012">ACS</span></span>

* <span data-ttu-id="012e3-2013">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="012e3-2013">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-2014">Appservice</span><span class="sxs-lookup"><span data-stu-id="012e3-2014">Appservice</span></span>

* <span data-ttu-id="012e3-2015">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="012e3-2015">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="012e3-2016">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="012e3-2016">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="012e3-2017">Se han quitado todos los comandos en</span><span class="sxs-lookup"><span data-stu-id="012e3-2017">Remove all commands under</span></span> `appservice web`
* <span data-ttu-id="012e3-2018">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="012e3-2018">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="012e3-2019">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="012e3-2019">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="012e3-2020">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="012e3-2020">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="012e3-2021">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="012e3-2021">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="012e3-2022">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="012e3-2022">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="012e3-2023">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="012e3-2023">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="012e3-2024">En su lugar, se usa</span><span class="sxs-lookup"><span data-stu-id="012e3-2024">Instead use</span></span> `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a><span data-ttu-id="012e3-2025">Batch</span><span class="sxs-lookup"><span data-stu-id="012e3-2025">Batch</span></span>

* <span data-ttu-id="012e3-2026">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="012e3-2026">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="012e3-2027">Se ha cambiado el nombre de la opción `--target-dedicated` de `pool create` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2027">Renamed `pool create` option `--target-dedicated` to</span></span> `--target-dedicated-nodes`
* <span data-ttu-id="012e3-2028">Se han agregado las opciones de `pool create` `--target-low-priority-nodes` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2028">Added `pool create` options `--target-low-priority-nodes` and</span></span> `--application-licenses`

### <a name="cdn"></a><span data-ttu-id="012e3-2029">CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-2029">CDN</span></span>

* <span data-ttu-id="012e3-2030">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="012e3-2030">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="012e3-2031">Nube</span><span class="sxs-lookup"><span data-stu-id="012e3-2031">Cloud</span></span>

* <span data-ttu-id="012e3-2032">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="012e3-2032">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="012e3-2033">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="012e3-2033">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="012e3-2034">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="012e3-2034">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="012e3-2035">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="012e3-2035">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="012e3-2036">Se ha expuesto</span><span class="sxs-lookup"><span data-stu-id="012e3-2036">Exposed</span></span> `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a><span data-ttu-id="012e3-2037">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-2037">CosmosDB</span></span>

* <span data-ttu-id="012e3-2038">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="012e3-2038">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="012e3-2039">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="012e3-2039">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="012e3-2040">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="012e3-2040">Data Lake Analytics</span></span>

* <span data-ttu-id="012e3-2041">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2041">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="012e3-2042">Se agregó</span><span class="sxs-lookup"><span data-stu-id="012e3-2042">Added</span></span> `dla job pipeline show`
* <span data-ttu-id="012e3-2043">Se agregó</span><span class="sxs-lookup"><span data-stu-id="012e3-2043">Added</span></span> `dla job recurrence list`

### <a name="data-lake-store"></a><span data-ttu-id="012e3-2044">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="012e3-2044">Data Lake Store</span></span>

* <span data-ttu-id="012e3-2045">Se ha agregado compatibilidad para la rotación de claves de almacenes de claves administrados por el usuario en</span><span class="sxs-lookup"><span data-stu-id="012e3-2045">Added support for user managed key vault key rotation in</span></span> `dls account update`
* <span data-ttu-id="012e3-2046">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="012e3-2046">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="012e3-2047">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2047">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="012e3-2048">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="012e3-2048">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="012e3-2049">Interactive</span><span class="sxs-lookup"><span data-stu-id="012e3-2049">Interactive</span></span>

* <span data-ttu-id="012e3-2050">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="012e3-2050">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="012e3-2051">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="012e3-2051">Increased test coverage</span></span>
* <span data-ttu-id="012e3-2052">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="012e3-2052">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="012e3-2053">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="012e3-2053">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="012e3-2054">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="012e3-2054">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="012e3-2055">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="012e3-2055">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="012e3-2056">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="012e3-2056">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="012e3-2057">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2057">Added `--progress` flag</span></span>
* <span data-ttu-id="012e3-2058">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="012e3-2058">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="012e3-2059">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="012e3-2059">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="012e3-2060">IoT</span><span class="sxs-lookup"><span data-stu-id="012e3-2060">IoT</span></span>

* <span data-ttu-id="012e3-2061">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="012e3-2061">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="012e3-2062">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="012e3-2062">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="012e3-2063">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="012e3-2063">Key vault</span></span>

* <span data-ttu-id="012e3-2064">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="012e3-2064">Added commands for key vault recovery features:</span></span>
  * `keyvault` <span data-ttu-id="012e3-2065">subcomandos `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2065">subcommands `purge`, `recover`,</span></span> `keyvault list-deleted`
  * `keyvault secret` <span data-ttu-id="012e3-2066">subcomandos `backup` `restore`, `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2066">subcommands `backup`, `restore`, `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault certificate` <span data-ttu-id="012e3-2067">subcomandos `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2067">subcommands `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault key` <span data-ttu-id="012e3-2068">subcomandos `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2068">subcommands `purge`, `recover`,</span></span> `list-deleted`
* <span data-ttu-id="012e3-2069">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="012e3-2069">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="012e3-2070">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="012e3-2070">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="012e3-2071">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="012e3-2071">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="012e3-2072">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-2072">Lab</span></span>

* <span data-ttu-id="012e3-2073">Se ha agregado compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante</span><span class="sxs-lookup"><span data-stu-id="012e3-2073">Added support for claiming any vm in the lab through</span></span> `az lab vm claim`
* <span data-ttu-id="012e3-2074">Se ha agregado un formateador de tablas de salida para `az lab vm list` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2074">Added table output formatter for `az lab vm list` and</span></span> `az lab vm show`

### <a name="monitor"></a><span data-ttu-id="012e3-2075">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-2075">Monitor</span></span>

* <span data-ttu-id="012e3-2076">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="012e3-2076">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="012e3-2077">Se ha cambiado el nombre de `monitor alert-rule-incidents list` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2077">Renamed `monitor alert-rule-incidents list` to</span></span> `monitor alert list-incidents`
* <span data-ttu-id="012e3-2078">Se ha cambiado el nombre de `monitor alert-rule-incidents show` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2078">Renamed `monitor alert-rule-incidents show` to</span></span> `monitor alert show-incident`
* <span data-ttu-id="012e3-2079">Se ha cambiado el nombre de `monitor metric-defintions list` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2079">Renamed `monitor metric-defintions list` to</span></span> `monitor metrics list-definitions`
* <span data-ttu-id="012e3-2080">Se ha cambiado el nombre de `monitor alert-rules` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2080">Renamed `monitor alert-rules` to</span></span> `monitor alert`
* <span data-ttu-id="012e3-2081">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="012e3-2081">Changed `monitor alert create`:</span></span>
  * `condition` <span data-ttu-id="012e3-2082">y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="012e3-2082">and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="012e3-2083">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="012e3-2083">Add numerous parameters to simplify the rule creation process</span></span>
  * `location` <span data-ttu-id="012e3-2084">ya no es necesario</span><span class="sxs-lookup"><span data-stu-id="012e3-2084">no longer required</span></span>
  * <span data-ttu-id="012e3-2085">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="012e3-2085">Add name and ID support for target</span></span>
  * <span data-ttu-id="012e3-2086">Remove</span><span class="sxs-lookup"><span data-stu-id="012e3-2086">Remove</span></span> `--alert-rule-resource-name`
  * <span data-ttu-id="012e3-2087">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="012e3-2087">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * `description` <span data-ttu-id="012e3-2088">toma un valor predeterminado basado en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="012e3-2088">defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="012e3-2089">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="012e3-2089">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="012e3-2090">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2090">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="012e3-2091">Se han agregado argumentos y ejemplos a</span><span class="sxs-lookup"><span data-stu-id="012e3-2091">Added convenience arguments and examples to</span></span> `monitor alert rule update`

### <a name="network"></a><span data-ttu-id="012e3-2092">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-2092">Network</span></span>

* <span data-ttu-id="012e3-2093">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2093">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="012e3-2094">Se ha agregado el argumento `--private-access-services` a `vnet subnet create` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2094">Added `--private-access-services` argument to `vnet subnet create` and</span></span> `vnet subnet update`
* <span data-ttu-id="012e3-2095">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="012e3-2095">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="012e3-2096">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="012e3-2096">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="012e3-2097">Se ha corregido el error al usar el argumento `--servers` con `application-gateway address-pool create` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2097">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and</span></span> `application-gateway address-pool update`
* <span data-ttu-id="012e3-2098">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2098">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="012e3-2099">Se han agregado comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2099">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`,</span></span> `predefined show`
* <span data-ttu-id="012e3-2100">Se han agregado argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2100">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`,</span></span> `--min-protocol-version`
* <span data-ttu-id="012e3-2101">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="012e3-2101">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="012e3-2102">Se han agregado argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2102">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`,</span></span> `--redirect-config`
* <span data-ttu-id="012e3-2103">Se ha agregado el argumento `--redirect-config` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2103">Added argument `--redirect-config` to</span></span> `application-gateway url-path-map rule create`
* <span data-ttu-id="012e3-2104">Se ha agregado compatibilidad para `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2104">Added support for `--no-wait` to</span></span> `application-gateway url-path-map rule delete`
* <span data-ttu-id="012e3-2105">Se han agregado argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span><span class="sxs-lookup"><span data-stu-id="012e3-2105">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span></span> `--match-status-codes`
* <span data-ttu-id="012e3-2106">Se ha agregado el argumento `--redirect-config` a `application-gateway rule create` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2106">Added argument `--redirect-config` to `application-gateway rule create` and</span></span> `application-gateway rule update`
* <span data-ttu-id="012e3-2107">Se ha agregado compatibilidad para `--accelerated-networking` a `nic create` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2107">Added support for `--accelerated-networking` to `nic create` and</span></span> `nic update`
* <span data-ttu-id="012e3-2108">Se ha quitado el argumento `--internal-dns-name-suffix` de</span><span class="sxs-lookup"><span data-stu-id="012e3-2108">Removed `--internal-dns-name-suffix` argument from</span></span> `nic create`
* <span data-ttu-id="012e3-2109">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="012e3-2109">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="012e3-2110">Se ha corregido el error por el que `local-gateway create` pasaba por alto</span><span class="sxs-lookup"><span data-stu-id="012e3-2110">Fixed bug where `local-gateway create` ignored</span></span> `--local-address-prefixes`
* <span data-ttu-id="012e3-2111">Se ha agregado compatibilidad para `--dns-servers` a</span><span class="sxs-lookup"><span data-stu-id="012e3-2111">Added support for `--dns-servers` to</span></span> `vnet update`
* <span data-ttu-id="012e3-2112">Se ha corregido el error al crear un emparejamiento sin filtrado de rutas con</span><span class="sxs-lookup"><span data-stu-id="012e3-2112">Fixed bug when creating a peering without route filtering with</span></span> `express-route peering create`
* <span data-ttu-id="012e3-2113">Se ha corregido el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con</span><span class="sxs-lookup"><span data-stu-id="012e3-2113">Fixed bug where `--provider` and `--bandwidth` arguments did not work with</span></span> `express-route update`
* <span data-ttu-id="012e3-2114">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2114">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="012e3-2115">Se ha mejorado el formato de salida de</span><span class="sxs-lookup"><span data-stu-id="012e3-2115">Improved output formatting for</span></span> `network list-usages`
* <span data-ttu-id="012e3-2116">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="012e3-2116">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="012e3-2117">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="012e3-2117">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="012e3-2118">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="012e3-2118">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="012e3-2119">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="012e3-2119">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="012e3-2120">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-2120">Profile</span></span>

* <span data-ttu-id="012e3-2121">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="012e3-2121">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="012e3-2122">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="012e3-2122">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="012e3-2123">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="012e3-2123">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="012e3-2124">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="012e3-2124">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="012e3-2125">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="012e3-2125">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="012e3-2126">RDBMS</span><span class="sxs-lookup"><span data-stu-id="012e3-2126">RDBMS</span></span>

* <span data-ttu-id="012e3-2127">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="012e3-2127">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="012e3-2128">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="012e3-2128">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="012e3-2129">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="012e3-2129">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="012e3-2130">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="012e3-2130">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-2131">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-2131">Resource</span></span>

* <span data-ttu-id="012e3-2132">Se han mejorado los mensajes de parámetros que faltan para</span><span class="sxs-lookup"><span data-stu-id="012e3-2132">Improved prompts for missing parameters for</span></span> `group deployment create`
* <span data-ttu-id="012e3-2133">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2133">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="012e3-2134">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2134">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="012e3-2135">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2135">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="012e3-2136">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="012e3-2136">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="012e3-2137">Se ha corregido el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2137">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and</span></span> `<resource-type>`
* <span data-ttu-id="012e3-2138">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="012e3-2138">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="012e3-2139">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2139">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="012e3-2140">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-2140">Role</span></span>

* <span data-ttu-id="012e3-2141">Compatibilidad para la salida en formato de archivo de autenticación del SDK para</span><span class="sxs-lookup"><span data-stu-id="012e3-2141">Support output in SDK auth file format for</span></span> `create-for-rbac`
* <span data-ttu-id="012e3-2142">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="012e3-2142">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="012e3-2143">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2143">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="012e3-2144">Se muestran advertencias acerca del desuso cuando se utiliza</span><span class="sxs-lookup"><span data-stu-id="012e3-2144">Show deprecation warnings when using</span></span> `--expanded-view`
* <span data-ttu-id="012e3-2145">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2145">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="012e3-2146">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="012e3-2146">Service Fabric</span></span>
* <span data-ttu-id="012e3-2147">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="012e3-2147">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="012e3-2148">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="012e3-2148">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="012e3-2149">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="012e3-2149">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-2150">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-2150">SQL</span></span>

* <span data-ttu-id="012e3-2151">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="012e3-2151">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="012e3-2152">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="012e3-2152">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="012e3-2153">Se han agregado los comandos `sql db list-editions` y</span><span class="sxs-lookup"><span data-stu-id="012e3-2153">Added commands `sql db list-editions` and</span></span> `sql elastic-pool list-editions`

### <a name="storage"></a><span data-ttu-id="012e3-2154">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-2154">Storage</span></span>

* <span data-ttu-id="012e3-2155">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="012e3-2155">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="012e3-2156">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="012e3-2156">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="012e3-2157">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="012e3-2157">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="012e3-2158">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="012e3-2158">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="012e3-2159">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="012e3-2159">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="012e3-2160">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="012e3-2160">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-2161">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-2161">VM</span></span>

* <span data-ttu-id="012e3-2162">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="012e3-2162">Support configuring nsg</span></span>
* <span data-ttu-id="012e3-2163">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="012e3-2163">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="012e3-2164">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="012e3-2164">Support managed service identities</span></span>
* <span data-ttu-id="012e3-2165">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería</span><span class="sxs-lookup"><span data-stu-id="012e3-2165">Fixed issue where `cmss create` with an existing load balancer required</span></span> `--backend-pool-name`
* <span data-ttu-id="012e3-2166">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="012e3-2166">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="012e3-2167">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-2167">May 10, 2017</span></span>

<span data-ttu-id="012e3-2168">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="012e3-2168">Version 2.0.6</span></span>

* <span data-ttu-id="012e3-2169">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="012e3-2169">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="012e3-2170">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="012e3-2170">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="012e3-2171">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="012e3-2171">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="012e3-2172">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="012e3-2172">Include Cognitive Services module</span></span>
* <span data-ttu-id="012e3-2173">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="012e3-2173">Include Service Fabric module</span></span>
* <span data-ttu-id="012e3-2174">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="012e3-2174">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="012e3-2175">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="012e3-2175">Add support for CDN commands</span></span>
* <span data-ttu-id="012e3-2176">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="012e3-2176">Remove Container module</span></span>
* <span data-ttu-id="012e3-2177">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="012e3-2177">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="012e3-2178">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="012e3-2178">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="012e3-2179">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-2179">Core</span></span>

* <span data-ttu-id="012e3-2180">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="012e3-2180">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="012e3-2181">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="012e3-2181">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="012e3-2182">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="012e3-2182">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="012e3-2183">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="012e3-2183">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="012e3-2184">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="012e3-2184">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="012e3-2185">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="012e3-2185">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="012e3-2186">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="012e3-2186">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="012e3-2187">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="012e3-2187">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="012e3-2188">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="012e3-2188">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="012e3-2189">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="012e3-2189">core: Improved performance</span></span>
* <span data-ttu-id="012e3-2190">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="012e3-2190">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="012e3-2191">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="012e3-2191">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-2192">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-2192">ACS</span></span>

* <span data-ttu-id="012e3-2193">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="012e3-2193">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="012e3-2194">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="012e3-2194">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="012e3-2195">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="012e3-2195">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="012e3-2196">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="012e3-2196">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-2197">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-2197">AppService</span></span>

* <span data-ttu-id="012e3-2198">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="012e3-2198">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="012e3-2199">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="012e3-2199">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="012e3-2200">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="012e3-2200">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="012e3-2201">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="012e3-2201">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="012e3-2202">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="012e3-2202">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="012e3-2203">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="012e3-2203">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="012e3-2204">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="012e3-2204">support slot swap with preview</span></span>
* <span data-ttu-id="012e3-2205">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="012e3-2205">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="012e3-2206">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="012e3-2206">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="012e3-2207">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-2207">CosmosDB</span></span>

* <span data-ttu-id="012e3-2208">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="012e3-2208">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="012e3-2209">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="012e3-2209">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="012e3-2210">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="012e3-2210">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="012e3-2211">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="012e3-2211">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="012e3-2212">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="012e3-2212">Data Lake Analytics</span></span>

* <span data-ttu-id="012e3-2213">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="012e3-2213">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="012e3-2214">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="012e3-2214">Add support for new catalog item type: package.</span></span> <span data-ttu-id="012e3-2215">al que se accede a través de:</span><span class="sxs-lookup"><span data-stu-id="012e3-2215">accessed through:</span></span> `az dla catalog package`
* <span data-ttu-id="012e3-2216">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="012e3-2216">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="012e3-2217">Tabla</span><span class="sxs-lookup"><span data-stu-id="012e3-2217">Table</span></span>
  * <span data-ttu-id="012e3-2218">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="012e3-2218">Table valued function</span></span>
  * <span data-ttu-id="012e3-2219">Ver</span><span class="sxs-lookup"><span data-stu-id="012e3-2219">View</span></span>
  * <span data-ttu-id="012e3-2220">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="012e3-2220">Table Statistics.</span></span> <span data-ttu-id="012e3-2221">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="012e3-2221">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="012e3-2222">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="012e3-2222">Data Lake Store</span></span>

* <span data-ttu-id="012e3-2223">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="012e3-2223">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="012e3-2224">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="012e3-2224">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="012e3-2225">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="012e3-2225">missed help for access show.</span></span> <span data-ttu-id="012e3-2226">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="012e3-2226">adding it.</span></span> <span data-ttu-id="012e3-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="012e3-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="012e3-2228">Buscar</span><span class="sxs-lookup"><span data-stu-id="012e3-2228">Find</span></span>

* <span data-ttu-id="012e3-2229">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="012e3-2229">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="012e3-2230">KeyVault</span><span class="sxs-lookup"><span data-stu-id="012e3-2230">KeyVault</span></span>

* <span data-ttu-id="012e3-2231">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="012e3-2231">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="012e3-2232">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="012e3-2232">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="012e3-2233">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="012e3-2233">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="012e3-2234">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="012e3-2234">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="012e3-2235">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="012e3-2235">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="012e3-2236">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-2236">Lab</span></span>

* <span data-ttu-id="012e3-2237">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-2237">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="012e3-2238">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-2238">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="012e3-2239">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-2239">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="012e3-2240">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-2240">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="012e3-2241">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="012e3-2241">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="012e3-2242">Supervisión</span><span class="sxs-lookup"><span data-stu-id="012e3-2242">Monitor</span></span>

* <span data-ttu-id="012e3-2243">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="012e3-2243">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="012e3-2244">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="012e3-2244">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="012e3-2245">Red</span><span class="sxs-lookup"><span data-stu-id="012e3-2245">Network</span></span>

* <span data-ttu-id="012e3-2246">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="012e3-2246">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="012e3-2247">Se ha agregado compatibilidad con el parámetro `--filters` para</span><span class="sxs-lookup"><span data-stu-id="012e3-2247">Add support for `--filters` parameter for</span></span> `network watcher packet-capture create`
* <span data-ttu-id="012e3-2248">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="012e3-2248">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="012e3-2249">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="012e3-2249">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="012e3-2250">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="012e3-2250">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="012e3-2251">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="012e3-2251">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="012e3-2252">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="012e3-2252">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="012e3-2253">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="012e3-2253">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="012e3-2254">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="012e3-2254">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="012e3-2255">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="012e3-2255">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="012e3-2256">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="012e3-2256">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="012e3-2257">BC: Se ha corregido el error en la salida de</span><span class="sxs-lookup"><span data-stu-id="012e3-2257">BC: Fix bug in the output of</span></span> `vpn-connection create`
* <span data-ttu-id="012e3-2258">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="012e3-2258">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="012e3-2259">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="012e3-2259">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="012e3-2260">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="012e3-2260">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="012e3-2261">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="012e3-2261">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="012e3-2262">Perfil</span><span class="sxs-lookup"><span data-stu-id="012e3-2262">Profile</span></span>

* <span data-ttu-id="012e3-2263">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="012e3-2263">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="012e3-2264">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="012e3-2264">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="012e3-2265">Redis</span><span class="sxs-lookup"><span data-stu-id="012e3-2265">Redis</span></span>

* <span data-ttu-id="012e3-2266">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="012e3-2266">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="012e3-2267">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="012e3-2267">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="012e3-2268">Recurso</span><span class="sxs-lookup"><span data-stu-id="012e3-2268">Resource</span></span>

* <span data-ttu-id="012e3-2269">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="012e3-2269">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="012e3-2270">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="012e3-2270">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="012e3-2271">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="012e3-2271">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="012e3-2272">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="012e3-2272">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="012e3-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="012e3-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="012e3-2274">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="012e3-2274">Add docs for az lock update.</span></span> <span data-ttu-id="012e3-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="012e3-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="012e3-2276">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="012e3-2276">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="012e3-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="012e3-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="012e3-2278">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="012e3-2278">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="012e3-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="012e3-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="012e3-2280">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="012e3-2280">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="012e3-2281">Rol</span><span class="sxs-lookup"><span data-stu-id="012e3-2281">Role</span></span>

* <span data-ttu-id="012e3-2282">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="012e3-2282">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="012e3-2283">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="012e3-2283">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="012e3-2284">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="012e3-2284">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="012e3-2285">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="012e3-2285">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="012e3-2286">SQL</span><span class="sxs-lookup"><span data-stu-id="012e3-2286">SQL</span></span>

* <span data-ttu-id="012e3-2287">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="012e3-2287">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="012e3-2288">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="012e3-2288">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="012e3-2289">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-2289">Storage</span></span>

* <span data-ttu-id="012e3-2290">Ubicación predeterminada del grupo de recursos para</span><span class="sxs-lookup"><span data-stu-id="012e3-2290">Default location to resource group location for</span></span> `storage account create`
* <span data-ttu-id="012e3-2291">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="012e3-2291">Add support for incremental blob copy</span></span>
* <span data-ttu-id="012e3-2292">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="012e3-2292">Add support for large block blob upload</span></span>
* <span data-ttu-id="012e3-2293">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="012e3-2293">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-2294">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-2294">VM</span></span>

* <span data-ttu-id="012e3-2295">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="012e3-2295">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="012e3-2296">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="012e3-2296">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="012e3-2297">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="012e3-2297">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="012e3-2298">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="012e3-2298">az vm/vmss disk</span></span>
  3. <span data-ttu-id="012e3-2299">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="012e3-2299">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="012e3-2300">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="012e3-2300">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="012e3-2301">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="012e3-2301">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="012e3-2302">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-2302">April 3, 2017</span></span>

<span data-ttu-id="012e3-2303">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="012e3-2303">Version 2.0.2</span></span>

<span data-ttu-id="012e3-2304">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="012e3-2304">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="012e3-2305">Núcleo</span><span class="sxs-lookup"><span data-stu-id="012e3-2305">Core</span></span>

* <span data-ttu-id="012e3-2306">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="012e3-2306">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="012e3-2307">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="012e3-2307">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="012e3-2308">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="012e3-2308">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="012e3-2309">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="012e3-2309">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="012e3-2310">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="012e3-2310">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="012e3-2311">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="012e3-2311">Add prompting for missing template parameters.</span></span> <span data-ttu-id="012e3-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="012e3-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="012e3-2313">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="012e3-2313">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="012e3-2314">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="012e3-2314">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="012e3-2315">ACS</span><span class="sxs-lookup"><span data-stu-id="012e3-2315">ACS</span></span>

* <span data-ttu-id="012e3-2316">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="012e3-2316">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="012e3-2317">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="012e3-2317">Add support for ssh key password prompting.</span></span> <span data-ttu-id="012e3-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="012e3-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="012e3-2319">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="012e3-2319">Add support for windows clusters.</span></span> <span data-ttu-id="012e3-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="012e3-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="012e3-2321">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="012e3-2321">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="012e3-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="012e3-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="012e3-2323">AppService</span><span class="sxs-lookup"><span data-stu-id="012e3-2323">AppService</span></span>

* <span data-ttu-id="012e3-2324">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="012e3-2324">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="012e3-2325">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="012e3-2325">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="012e3-2326">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="012e3-2326">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="012e3-2327">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="012e3-2327">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="012e3-2328">DataLake</span><span class="sxs-lookup"><span data-stu-id="012e3-2328">DataLake</span></span>

* <span data-ttu-id="012e3-2329">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="012e3-2329">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="012e3-2330">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="012e3-2330">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="012e3-2331">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="012e3-2331">DocuemntDB</span></span>

* <span data-ttu-id="012e3-2332">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="012e3-2332">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="012e3-2333">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="012e3-2333">VM</span></span>

* <span data-ttu-id="012e3-2334">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="012e3-2334">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="012e3-2335">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="012e3-2335">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="012e3-2336">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="012e3-2336">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="012e3-2337">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="012e3-2337">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="012e3-2338">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="012e3-2338">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="012e3-2339">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="012e3-2339">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="012e3-2340">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="012e3-2340">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="012e3-2341">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="012e3-2341">February 27, 2017</span></span>

<span data-ttu-id="012e3-2342">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="012e3-2342">Version 2.0.0</span></span>

<span data-ttu-id="012e3-2343">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="012e3-2343">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="012e3-2344">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="012e3-2344">Container Service (acs)</span></span>
- <span data-ttu-id="012e3-2345">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="012e3-2345">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="012e3-2346">Redes</span><span class="sxs-lookup"><span data-stu-id="012e3-2346">Networking</span></span>
- <span data-ttu-id="012e3-2347">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="012e3-2347">Storage</span></span>

<span data-ttu-id="012e3-2348">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="012e3-2348">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="012e3-2349">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="012e3-2349">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="012e3-2350">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="012e3-2350">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="012e3-2351">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="012e3-2351">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="012e3-2352">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="012e3-2352">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="012e3-2353">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="012e3-2353">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="012e3-2354">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="012e3-2354">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="012e3-2355">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="012e3-2355">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="012e3-2356">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="012e3-2356">Provide feedback from the command line with the `az feedback` command</span></span>

