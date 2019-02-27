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
ms.openlocfilehash: 1c6b2cc57b80256faff0a174bec5f13bd84f5a1b
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158731"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="be8ce-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="be8ce-103">Azure CLI release notes</span></span>
## <a name="february-12-2019"></a><span data-ttu-id="be8ce-104">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="be8ce-104">February 12, 2019</span></span>

<span data-ttu-id="be8ce-105">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="be8ce-105">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-106">Core</span></span>

* <span data-ttu-id="be8ce-107">`az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="be8ce-107">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="be8ce-108">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="be8ce-108">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-109">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-109">ACR</span></span>
* <span data-ttu-id="be8ce-110">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-110">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="be8ce-111">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-111">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-112">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-112">ACS</span></span>
* <span data-ttu-id="be8ce-113">Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.</span><span class="sxs-lookup"><span data-stu-id="be8ce-113">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="be8ce-114">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-114">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="be8ce-115">Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-115">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="be8ce-116">AMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-116">AMS</span></span>
* <span data-ttu-id="be8ce-117">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-117">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="be8ce-118">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-118">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-119">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-119">Appservice</span></span>
* <span data-ttu-id="be8ce-120">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="be8ce-120">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="be8ce-121">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="be8ce-121">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="be8ce-122">Se ha mejorado la ayuda de `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-122">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="be8ce-123">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="be8ce-123">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="be8ce-124">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="be8ce-124">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="be8ce-125">Botservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-125">Botservice</span></span>
* <span data-ttu-id="be8ce-126">Se ha mejorado la experiencia de usuario de `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-126">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="be8ce-127">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-127">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="be8ce-128">Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-128">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="be8ce-129">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="be8ce-129">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="be8ce-130">[EN DESUSO] Se ha dejado de usar el argumento `--proj-name` en favor de `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-130">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="be8ce-131">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="be8ce-131">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="be8ce-132">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="be8ce-132">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="be8ce-133">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="be8ce-133">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="be8ce-134">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="be8ce-134">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="be8ce-135">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="be8ce-135">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="be8ce-136">Key Vault</span><span class="sxs-lookup"><span data-stu-id="be8ce-136">Key Vault</span></span>
* <span data-ttu-id="be8ce-137">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-137">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-138">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-138">Monitor</span></span>
* <span data-ttu-id="be8ce-139">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-139">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-140">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-140">Network</span></span>
* <span data-ttu-id="be8ce-141">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-141">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="be8ce-142">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="be8ce-142">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="be8ce-143">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="be8ce-143">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="be8ce-144">Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-144">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="be8ce-145">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="be8ce-145">Policy Insights</span></span>
* <span data-ttu-id="be8ce-146">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-146">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-147">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-147">RDBMS</span></span>
* <span data-ttu-id="be8ce-148">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="be8ce-148">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="be8ce-149">Redis</span><span class="sxs-lookup"><span data-stu-id="be8ce-149">Redis</span></span>
* <span data-ttu-id="be8ce-150">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="be8ce-150">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="be8ce-151">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="be8ce-151">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="be8ce-152">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="be8ce-152">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="be8ce-153">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="be8ce-153">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="be8ce-154">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-154">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="be8ce-155">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="be8ce-155">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="be8ce-156">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-156">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-157">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-157">Role</span></span>
* <span data-ttu-id="be8ce-158">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-158">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="be8ce-159">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-159">SQL VM</span></span>
* <span data-ttu-id="be8ce-160">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="be8ce-160">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-161">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-161">VM</span></span>
* <span data-ttu-id="be8ce-162">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-162">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="be8ce-163">Se agregó `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-163">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="be8ce-164">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="be8ce-164">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="be8ce-165">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-165">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="be8ce-166">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="be8ce-166">January 31, 2019</span></span>

<span data-ttu-id="be8ce-167">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="be8ce-167">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-168">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-168">Core</span></span>

* <span data-ttu-id="be8ce-169">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="be8ce-169">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="be8ce-170">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="be8ce-170">January 28, 2019</span></span>

<span data-ttu-id="be8ce-171">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="be8ce-171">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-172">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-172">ACR</span></span>
* <span data-ttu-id="be8ce-173">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="be8ce-173">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-174">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-174">ACS</span></span>
* <span data-ttu-id="be8ce-175">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="be8ce-175">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="be8ce-176">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="be8ce-176">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="be8ce-177">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-177">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="be8ce-178">AMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-178">AMS</span></span>
* <span data-ttu-id="be8ce-179">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="be8ce-179">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="be8ce-180">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="be8ce-180">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-181">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-181">Appservice</span></span>
* <span data-ttu-id="be8ce-182">Se ha agregado compatibilidad para App Insights en `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-182">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="be8ce-183">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="be8ce-183">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="be8ce-184">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="be8ce-184">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-185">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-185">Container</span></span>
* <span data-ttu-id="be8ce-186">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-186">Added `container start` command</span></span>
* <span data-ttu-id="be8ce-187">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="be8ce-187">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="be8ce-188">EventGrid</span><span class="sxs-lookup"><span data-stu-id="be8ce-188">EventGrid</span></span>
* <span data-ttu-id="be8ce-189">Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-189">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="be8ce-190">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="be8ce-190">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="be8ce-191">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-191">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="be8ce-192">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-192">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="be8ce-193">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="be8ce-193">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="be8ce-194">HDInsight</span><span class="sxs-lookup"><span data-stu-id="be8ce-194">HDInsight</span></span>
* <span data-ttu-id="be8ce-195">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-195">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="be8ce-196">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="be8ce-196">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="be8ce-197">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-197">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="be8ce-198">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-198">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="be8ce-199">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-199">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="be8ce-200">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-200">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-201">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-201">IoT</span></span>
* <span data-ttu-id="be8ce-202">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="be8ce-202">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="be8ce-203">Kusto</span><span class="sxs-lookup"><span data-stu-id="be8ce-203">Kusto</span></span>
* <span data-ttu-id="be8ce-204">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-204">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-205">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-205">Monitor</span></span>
* <span data-ttu-id="be8ce-206">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-206">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-207">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-207">Profile</span></span>
* <span data-ttu-id="be8ce-208">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-208">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-209">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-209">Network</span></span>
* <span data-ttu-id="be8ce-210">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-210">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="be8ce-211">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="be8ce-211">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-212">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-212">Resource</span></span>
* <span data-ttu-id="be8ce-213">Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-213">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="be8ce-214">Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-214">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="be8ce-215">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-215">SQL Virtual Machine</span></span>
* <span data-ttu-id="be8ce-216">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-216">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-217">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-217">Storage</span></span>
* <span data-ttu-id="be8ce-218">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="be8ce-218">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="be8ce-219">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="be8ce-219">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-220">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-220">VM</span></span>
* <span data-ttu-id="be8ce-221">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="be8ce-221">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="be8ce-222">Se ha agregado la marca `--force` a `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-222">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="be8ce-223">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="be8ce-223">January 15, 2019</span></span>

<span data-ttu-id="be8ce-224">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="be8ce-224">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-225">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-225">ACR</span></span>
* <span data-ttu-id="be8ce-226">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="be8ce-226">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="be8ce-227">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="be8ce-227">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="be8ce-228">[EN DESUSO] El parámetro `--resource-group` está en desuso en los comandos:</span><span class="sxs-lookup"><span data-stu-id="be8ce-228">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="be8ce-229">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-229">ACS</span></span>
* <span data-ttu-id="be8ce-230">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="be8ce-230">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-231">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-231">Appservice</span></span>
* <span data-ttu-id="be8ce-232">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="be8ce-232">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="be8ce-233">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="be8ce-233">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="be8ce-234">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="be8ce-234">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="be8ce-235">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-235">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="be8ce-236">Botservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-236">Botservice</span></span>
* <span data-ttu-id="be8ce-237">Se han agregado actualizaciones al estado de implementación a `bot create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-237">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="be8ce-238">Configuración</span><span class="sxs-lookup"><span data-stu-id="be8ce-238">Configure</span></span>
* <span data-ttu-id="be8ce-239">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="be8ce-239">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be8ce-240">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-240">CosmosDB</span></span>
* <span data-ttu-id="be8ce-241">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="be8ce-241">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="be8ce-242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="be8ce-242">HDInsight</span></span>
* <span data-ttu-id="be8ce-243">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="be8ce-243">Added commands for managing applications</span></span>
* <span data-ttu-id="be8ce-244">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="be8ce-244">Added commands for managing script actions</span></span>
* <span data-ttu-id="be8ce-245">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="be8ce-245">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="be8ce-246">Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-246">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="be8ce-247">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-247">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-248">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-248">Network</span></span>
* <span data-ttu-id="be8ce-249">Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-249">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="be8ce-250">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="be8ce-250">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="be8ce-251">Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-251">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="be8ce-252">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-252">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-253">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-253">Role</span></span>
* <span data-ttu-id="be8ce-254">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-254">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="be8ce-255">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="be8ce-255">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="be8ce-256">Seguridad</span><span class="sxs-lookup"><span data-stu-id="be8ce-256">Security</span></span>
* <span data-ttu-id="be8ce-257">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="be8ce-257">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-258">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-258">Storage</span></span>
* <span data-ttu-id="be8ce-259">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="be8ce-259">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="be8ce-260">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="be8ce-260">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="be8ce-261">Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-261">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="be8ce-262">Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-262">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="be8ce-263">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-263">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-264">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-264">VM</span></span>
* <span data-ttu-id="be8ce-265">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="be8ce-265">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="be8ce-266">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-266">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="be8ce-267">Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-267">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="be8ce-268">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="be8ce-268">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="be8ce-269">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="be8ce-269">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="be8ce-270">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-270">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="be8ce-271">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-271">December 20, 2018</span></span>

<span data-ttu-id="be8ce-272">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="be8ce-272">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="be8ce-273">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-273">Appservice</span></span>
* <span data-ttu-id="be8ce-274">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="be8ce-274">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="be8ce-275">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="be8ce-275">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="be8ce-276">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="be8ce-276">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="be8ce-277">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="be8ce-277">IoTCentral</span></span>
* <span data-ttu-id="be8ce-278">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="be8ce-278">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-279">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-279">Role</span></span>
* <span data-ttu-id="be8ce-280">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-280">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-281">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-281">SQL</span></span>
* <span data-ttu-id="be8ce-282">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-282">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-283">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-283">VM</span></span>
* <span data-ttu-id="be8ce-284">Se ha agregado el parámetro `---os-type` a `disk create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-284">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="be8ce-285">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-285">December 18, 2018</span></span>

<span data-ttu-id="be8ce-286">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="be8ce-286">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="be8ce-287">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-287">ACR</span></span>
* <span data-ttu-id="be8ce-288">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-288">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="be8ce-289">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-289">Condensed the table layout for task list</span></span>
* <span data-ttu-id="be8ce-290">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="be8ce-290">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-291">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-291">ACS</span></span>
* <span data-ttu-id="be8ce-292">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="be8ce-292">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="be8ce-293">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-293">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="be8ce-294">[EN DESUSO] Se han dejado de utilizar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-294">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="be8ce-295">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="be8ce-295">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="be8ce-296">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="be8ce-296">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="be8ce-297">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="be8ce-297">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-298">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-298">Appservice</span></span>
* <span data-ttu-id="be8ce-299">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-299">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="be8ce-300">Botservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-300">Botservice</span></span>
* <span data-ttu-id="be8ce-301">Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-301">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="be8ce-302">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="be8ce-302">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="be8ce-303">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-303">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="be8ce-304">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="be8ce-304">Reduced Kudu network calls</span></span>
* <span data-ttu-id="be8ce-305">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="be8ce-305">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="be8ce-306">Consumo</span><span class="sxs-lookup"><span data-stu-id="be8ce-306">Consumption</span></span>
* <span data-ttu-id="be8ce-307">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="be8ce-307">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be8ce-308">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-308">CosmosDB</span></span>
* <span data-ttu-id="be8ce-309">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="be8ce-309">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="be8ce-310">Mapas</span><span class="sxs-lookup"><span data-stu-id="be8ce-310">Maps</span></span>
* <span data-ttu-id="be8ce-311">Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-311">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-312">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-312">Network</span></span>
* <span data-ttu-id="be8ce-313">Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="be8ce-313">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="be8ce-314">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="be8ce-314">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-315">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-315">Resource</span></span>
* <span data-ttu-id="be8ce-316">Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-316">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="be8ce-317">Se ha agregado un nuevo comando `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-317">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-318">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-318">Storage</span></span>
*  <span data-ttu-id="be8ce-319">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-319">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-320">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-320">VM</span></span>
* <span data-ttu-id="be8ce-321">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-321">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="be8ce-322">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-322">December 4, 2018</span></span>

<span data-ttu-id="be8ce-323">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="be8ce-323">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="be8ce-324">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-324">Core</span></span>
* <span data-ttu-id="be8ce-325">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="be8ce-325">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="be8ce-326">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="be8ce-326">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-327">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-327">Appservice</span></span>
* <span data-ttu-id="be8ce-328">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="be8ce-328">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="be8ce-329">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="be8ce-329">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-330">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-330">Network</span></span>
* <span data-ttu-id="be8ce-331">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="be8ce-331">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-332">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-332">Role</span></span>
* <span data-ttu-id="be8ce-333">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="be8ce-333">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="be8ce-334">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-334">VM</span></span>
* <span data-ttu-id="be8ce-335">[EN DESUSO] El parámetro `vm extension [show|wait] --expand` está en desuso</span><span class="sxs-lookup"><span data-stu-id="be8ce-335">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="be8ce-336">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="be8ce-336">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="be8ce-337">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="be8ce-337">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="be8ce-338">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="be8ce-338">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="be8ce-339">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-339">November 20, 2018</span></span>

<span data-ttu-id="be8ce-340">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="be8ce-340">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="be8ce-341">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-341">Core</span></span>
* <span data-ttu-id="be8ce-342">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="be8ce-342">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-343">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-343">ACR</span></span>
* <span data-ttu-id="be8ce-344">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="be8ce-344">Added context token to task step</span></span>
* <span data-ttu-id="be8ce-345">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="be8ce-345">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="be8ce-346">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-346">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-347">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-347">Appservice</span></span>
* <span data-ttu-id="be8ce-348">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="be8ce-348">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="be8ce-349">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-349">Updated the default `node_version`.</span></span> <span data-ttu-id="be8ce-350">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="be8ce-350">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="be8ce-351">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="be8ce-351">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="be8ce-352">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="be8ce-352">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="be8ce-353">IotCentral</span><span class="sxs-lookup"><span data-stu-id="be8ce-353">IotCentral</span></span>
* <span data-ttu-id="be8ce-354">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="be8ce-354">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-355">KeyVault</span><span class="sxs-lookup"><span data-stu-id="be8ce-355">KeyVault</span></span>
* <span data-ttu-id="be8ce-356">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="be8ce-356">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-357">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-357">Network</span></span>
* <span data-ttu-id="be8ce-358">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="be8ce-358">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="be8ce-359">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="be8ce-359">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="be8ce-360">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="be8ce-360">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="be8ce-361">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-361">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-362">Rdbms</span><span class="sxs-lookup"><span data-stu-id="be8ce-362">Rdbms</span></span>
* <span data-ttu-id="be8ce-363">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="be8ce-363">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="be8ce-364">Rbac</span><span class="sxs-lookup"><span data-stu-id="be8ce-364">Rbac</span></span>
* <span data-ttu-id="be8ce-365">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-365">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="be8ce-366">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-366">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="be8ce-367">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-367">Storage</span></span>
* <span data-ttu-id="be8ce-368">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="be8ce-368">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="be8ce-369">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-369">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="be8ce-370">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="be8ce-370">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="be8ce-371">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-371">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-372">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-372">VM</span></span>
* <span data-ttu-id="be8ce-373">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="be8ce-373">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="be8ce-374">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-374">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="be8ce-375">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-375">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="be8ce-376">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-376">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="be8ce-377">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-377">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="be8ce-378">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-378">Added `snapshot wait` command</span></span>
* <span data-ttu-id="be8ce-379">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-379">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="be8ce-380">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-380">November 6, 2018</span></span>

<span data-ttu-id="be8ce-381">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="be8ce-381">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-382">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-382">Core</span></span>
* <span data-ttu-id="be8ce-383">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="be8ce-383">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-384">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-384">ACR</span></span>
* <span data-ttu-id="be8ce-385">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="be8ce-385">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="be8ce-386">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="be8ce-386">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-387">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-387">ACS</span></span>
* <span data-ttu-id="be8ce-388">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="be8ce-388">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="be8ce-389">Advisor</span><span class="sxs-lookup"><span data-stu-id="be8ce-389">Advisor</span></span>
* <span data-ttu-id="be8ce-390">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="be8ce-390">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="be8ce-391">AMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-391">AMS</span></span>
* <span data-ttu-id="be8ce-392">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="be8ce-392">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="be8ce-393">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="be8ce-393">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="be8ce-394">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-394">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="be8ce-395">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-395">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="be8ce-396">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="be8ce-396">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="be8ce-397">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="be8ce-397">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="be8ce-398">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="be8ce-398">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="be8ce-399">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="be8ce-399">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="be8ce-400">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="be8ce-400">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="be8ce-401">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="be8ce-401">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="be8ce-402">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="be8ce-402">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="be8ce-403">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-403">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="be8ce-404">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="be8ce-404">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="be8ce-405">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="be8ce-405">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="be8ce-406">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-406">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="be8ce-407">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="be8ce-407">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="be8ce-408">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="be8ce-408">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-409">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-409">AppService</span></span>
* <span data-ttu-id="be8ce-410">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="be8ce-410">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="be8ce-411">Configuración</span><span class="sxs-lookup"><span data-stu-id="be8ce-411">Configure</span></span>
* <span data-ttu-id="be8ce-412">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="be8ce-412">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-413">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-413">Container</span></span>
* <span data-ttu-id="be8ce-414">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="be8ce-414">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="be8ce-415">EventHub</span><span class="sxs-lookup"><span data-stu-id="be8ce-415">EventHub</span></span>
* <span data-ttu-id="be8ce-416">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-416">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-417">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-417">Interactive</span></span>
* <span data-ttu-id="be8ce-418">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="be8ce-418">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-419">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-419">Monitor</span></span>
* <span data-ttu-id="be8ce-420">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-420">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-421">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-421">Network</span></span>
* <span data-ttu-id="be8ce-422">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="be8ce-422">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="be8ce-423">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="be8ce-423">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="be8ce-424">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-424">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="be8ce-425">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-425">Profile</span></span>
* <span data-ttu-id="be8ce-426">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="be8ce-426">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-427">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-427">RDBMS</span></span>
* <span data-ttu-id="be8ce-428">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="be8ce-428">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-429">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-429">Resource</span></span>
* <span data-ttu-id="be8ce-430">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="be8ce-430">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-431">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-431">Role</span></span>
* <span data-ttu-id="be8ce-432">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="be8ce-432">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="be8ce-433">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="be8ce-433">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="be8ce-434">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="be8ce-434">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-435">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-435">Storage</span></span>
* <span data-ttu-id="be8ce-436">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="be8ce-436">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-437">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-437">VM</span></span>
* <span data-ttu-id="be8ce-438">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="be8ce-438">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="be8ce-439">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="be8ce-439">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="be8ce-440">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="be8ce-440">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="be8ce-441">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="be8ce-441">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="be8ce-442">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="be8ce-442">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="be8ce-443">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="be8ce-443">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="be8ce-444">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-444">October 23, 2018</span></span>

<span data-ttu-id="be8ce-445">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="be8ce-445">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-446">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-446">Core</span></span>
* <span data-ttu-id="be8ce-447">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="be8ce-447">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="be8ce-448">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="be8ce-448">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-449">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-449">ACR</span></span>
* <span data-ttu-id="be8ce-450">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="be8ce-450">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="be8ce-451">CDN</span><span class="sxs-lookup"><span data-stu-id="be8ce-451">CDN</span></span>
* <span data-ttu-id="be8ce-452">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="be8ce-452">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="be8ce-453">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="be8ce-453">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-454">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-454">Container</span></span>
* <span data-ttu-id="be8ce-455">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="be8ce-455">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="be8ce-456">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-456">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="be8ce-457">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="be8ce-457">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="be8ce-458">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-458">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="be8ce-459">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="be8ce-459">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="be8ce-460">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="be8ce-460">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="be8ce-461">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="be8ce-461">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be8ce-462">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-462">CosmosDB</span></span>
* <span data-ttu-id="be8ce-463">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-463">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-464">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-464">Interactive</span></span>
* <span data-ttu-id="be8ce-465">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="be8ce-465">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="be8ce-466">IoT Central</span><span class="sxs-lookup"><span data-stu-id="be8ce-466">IoT Central</span></span>
* <span data-ttu-id="be8ce-467">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="be8ce-467">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="be8ce-468">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="be8ce-468">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-469">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-469">Monitor</span></span>
* <span data-ttu-id="be8ce-470">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="be8ce-470">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="be8ce-471">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="be8ce-471">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="be8ce-472">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="be8ce-472">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="be8ce-473">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="be8ce-473">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="be8ce-474">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="be8ce-474">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="be8ce-475">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="be8ce-475">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="be8ce-476">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="be8ce-476">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="be8ce-477">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="be8ce-477">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="be8ce-478">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="be8ce-478">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="be8ce-479">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-479">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-480">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-480">Network</span></span>
* <span data-ttu-id="be8ce-481">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="be8ce-481">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="be8ce-482">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="be8ce-482">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="be8ce-483">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="be8ce-483">ServiceBus</span></span>
* <span data-ttu-id="be8ce-484">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="be8ce-484">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-485">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-485">SQL</span></span>
* <span data-ttu-id="be8ce-486">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="be8ce-486">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-487">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-487">Storage</span></span>
* <span data-ttu-id="be8ce-488">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="be8ce-488">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="be8ce-489">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="be8ce-489">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-490">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-490">VM</span></span>
* <span data-ttu-id="be8ce-491">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-491">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="be8ce-492">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-492">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="be8ce-493">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-493">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="be8ce-494">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-494">October 16, 2018</span></span>

<span data-ttu-id="be8ce-495">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="be8ce-495">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-496">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-496">VM</span></span>
* <span data-ttu-id="be8ce-497">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="be8ce-497">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="be8ce-498">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-498">October 9, 2018</span></span>

<span data-ttu-id="be8ce-499">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="be8ce-499">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-500">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-500">Core</span></span>
* <span data-ttu-id="be8ce-501">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="be8ce-501">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-502">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-502">ACR</span></span>
* <span data-ttu-id="be8ce-503">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="be8ce-503">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-504">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-504">ACS</span></span>
* <span data-ttu-id="be8ce-505">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="be8ce-505">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="be8ce-506">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="be8ce-506">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="be8ce-507">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="be8ce-507">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="be8ce-508">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="be8ce-508">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-509">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-509">Container</span></span>
* <span data-ttu-id="be8ce-510">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="be8ce-510">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="be8ce-511">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="be8ce-511">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="be8ce-512">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="be8ce-512">Event Hub</span></span>
* <span data-ttu-id="be8ce-513">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-513">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="be8ce-514">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="be8ce-514">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="be8ce-515">Extensiones</span><span class="sxs-lookup"><span data-stu-id="be8ce-515">Extensions</span></span>
* <span data-ttu-id="be8ce-516">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="be8ce-516">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="be8ce-517">HDInsight</span><span class="sxs-lookup"><span data-stu-id="be8ce-517">HDInsight</span></span>
* <span data-ttu-id="be8ce-518">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="be8ce-518">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-519">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-519">IoT</span></span>
* <span data-ttu-id="be8ce-520">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="be8ce-520">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-521">KeyVault</span><span class="sxs-lookup"><span data-stu-id="be8ce-521">KeyVault</span></span>
* <span data-ttu-id="be8ce-522">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="be8ce-522">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-523">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-523">Network</span></span>
* <span data-ttu-id="be8ce-524">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-524">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="be8ce-525">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="be8ce-525">See #6052</span></span>
* <span data-ttu-id="be8ce-526">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-526">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="be8ce-527">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="be8ce-527">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="be8ce-528">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="be8ce-528">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="be8ce-529">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="be8ce-529">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="be8ce-530">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="be8ce-530">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="be8ce-531">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-531">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-532">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-532">Role</span></span>
* <span data-ttu-id="be8ce-533">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="be8ce-533">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="be8ce-534">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="be8ce-534">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="be8ce-535">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="be8ce-535">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="be8ce-536">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="be8ce-536">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="be8ce-537">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="be8ce-537">Service Bus</span></span>
* <span data-ttu-id="be8ce-538">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="be8ce-538">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-539">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-539">VM</span></span>
* <span data-ttu-id="be8ce-540">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="be8ce-540">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="be8ce-541">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="be8ce-541">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="be8ce-542">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="be8ce-542">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="be8ce-543">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="be8ce-543">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="be8ce-544">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="be8ce-544">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="be8ce-545">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="be8ce-545">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="be8ce-546">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-546">September 21, 2018</span></span>

<span data-ttu-id="be8ce-547">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="be8ce-547">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-548">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-548">ACR</span></span>
* <span data-ttu-id="be8ce-549">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-549">Added ACR Task commands</span></span>
* <span data-ttu-id="be8ce-550">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="be8ce-550">Added quick run command</span></span>
* <span data-ttu-id="be8ce-551">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="be8ce-551">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="be8ce-552">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-552">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="be8ce-553">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="be8ce-553">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="be8ce-554">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="be8ce-554">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-555">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-555">ACS</span></span>
* <span data-ttu-id="be8ce-556">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="be8ce-556">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="be8ce-557">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="be8ce-557">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-558">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-558">AppService</span></span>

* <span data-ttu-id="be8ce-559">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="be8ce-559">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="be8ce-560">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="be8ce-560">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="be8ce-561">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="be8ce-561">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="be8ce-562">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="be8ce-562">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-563">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-563">Batch</span></span>
* <span data-ttu-id="be8ce-564">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="be8ce-564">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="be8ce-565">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="be8ce-565">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="be8ce-566">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-566">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="be8ce-567">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="be8ce-567">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="be8ce-568">Batch AI</span><span class="sxs-lookup"><span data-stu-id="be8ce-568">Batch AI</span></span> 
* <span data-ttu-id="be8ce-569">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-569">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="be8ce-570">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="be8ce-570">Cognitive Services</span></span>
* <span data-ttu-id="be8ce-571">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="be8ce-571">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="be8ce-572">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="be8ce-572">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="be8ce-573">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="be8ce-573">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="be8ce-574">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-574">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="be8ce-575">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-575">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="be8ce-576">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="be8ce-576">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-577">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-577">Container</span></span>
* <span data-ttu-id="be8ce-578">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="be8ce-578">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="be8ce-579">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="be8ce-579">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="be8ce-580">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-580">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="be8ce-581">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-581">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="be8ce-582">DataLake</span><span class="sxs-lookup"><span data-stu-id="be8ce-582">Datalake</span></span>
* <span data-ttu-id="be8ce-583">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-583">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="be8ce-584">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="be8ce-584">Interactive Shell</span></span>
* <span data-ttu-id="be8ce-585">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="be8ce-585">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="be8ce-586">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="be8ce-586">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-587">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-587">IoT</span></span>
* <span data-ttu-id="be8ce-588">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-588">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="be8ce-589">Key Vault</span><span class="sxs-lookup"><span data-stu-id="be8ce-589">Key Vault</span></span>
* <span data-ttu-id="be8ce-590">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="be8ce-590">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-591">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-591">Network</span></span>
* <span data-ttu-id="be8ce-592">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="be8ce-592">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="be8ce-593">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="be8ce-593">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="be8ce-594">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="be8ce-594">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="be8ce-595">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="be8ce-595">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="be8ce-596">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-596">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="be8ce-597">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-597">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="be8ce-598">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="be8ce-598">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="be8ce-599">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="be8ce-599">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="be8ce-600">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="be8ce-600">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="be8ce-601">`network express-route create/update`: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="be8ce-601">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="be8ce-602">`network vnet subnet create/update`: Se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="be8ce-602">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="be8ce-603">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-603">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="be8ce-604">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="be8ce-604">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="be8ce-605">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="be8ce-605">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="be8ce-606">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="be8ce-606">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="be8ce-607">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="be8ce-607">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="be8ce-608">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="be8ce-608">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="be8ce-609">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="be8ce-609">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-610">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-610">RDBMS</span></span>
* <span data-ttu-id="be8ce-611">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-611">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="be8ce-612">Reserva</span><span class="sxs-lookup"><span data-stu-id="be8ce-612">Reservation</span></span>
* <span data-ttu-id="be8ce-613">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="be8ce-613">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="be8ce-614">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-614">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="be8ce-615">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="be8ce-615">Manage App</span></span>
* <span data-ttu-id="be8ce-616">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="be8ce-616">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="be8ce-617">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="be8ce-617">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-618">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-618">Role</span></span>
* <span data-ttu-id="be8ce-619">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="be8ce-619">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="be8ce-620">SignalR</span><span class="sxs-lookup"><span data-stu-id="be8ce-620">SignalR</span></span>
* <span data-ttu-id="be8ce-621">Primera versión</span><span class="sxs-lookup"><span data-stu-id="be8ce-621">First release</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-622">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-622">Storage</span></span>
* <span data-ttu-id="be8ce-623">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="be8ce-623">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="be8ce-624">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="be8ce-624">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-625">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-625">VM</span></span>
* <span data-ttu-id="be8ce-626">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="be8ce-626">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="be8ce-627">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="be8ce-627">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="be8ce-628">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-628">August 28, 2018</span></span>

<span data-ttu-id="be8ce-629">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="be8ce-629">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-630">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-630">Core</span></span>

* <span data-ttu-id="be8ce-631">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="be8ce-631">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="be8ce-632">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="be8ce-632">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-633">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-633">ACR</span></span>

* <span data-ttu-id="be8ce-634">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="be8ce-634">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="be8ce-635">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="be8ce-635">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-636">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-636">ACS</span></span>

* <span data-ttu-id="be8ce-637">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="be8ce-637">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="be8ce-638">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="be8ce-638">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-639">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-639">AppService</span></span>

* <span data-ttu-id="be8ce-640">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="be8ce-640">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="be8ce-641">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-641">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="be8ce-642">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-642">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="be8ce-643">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="be8ce-643">Backup</span></span>

* <span data-ttu-id="be8ce-644">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-644">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="be8ce-645">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="be8ce-645">Bot Service</span></span>

* <span data-ttu-id="be8ce-646">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="be8ce-646">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="be8ce-647">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="be8ce-647">Cognitive Services</span></span>

* <span data-ttu-id="be8ce-648">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="be8ce-648">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-649">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-649">IoT</span></span>

* <span data-ttu-id="be8ce-650">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="be8ce-650">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-651">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-651">Monitor</span></span>

* <span data-ttu-id="be8ce-652">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="be8ce-652">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="be8ce-653">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="be8ce-653">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-654">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-654">Network</span></span>

* <span data-ttu-id="be8ce-655">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-655">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-656">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-656">Resource</span></span>

* <span data-ttu-id="be8ce-657">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-657">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-658">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-658">Storage</span></span>

* <span data-ttu-id="be8ce-659">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-659">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-660">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-660">VM</span></span>

* <span data-ttu-id="be8ce-661">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-661">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="be8ce-662">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-662">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="be8ce-663">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-663">Auguest 14, 2018</span></span>

<span data-ttu-id="be8ce-664">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="be8ce-664">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-665">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-665">Core</span></span>

* <span data-ttu-id="be8ce-666">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="be8ce-666">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="be8ce-667">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="be8ce-667">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="be8ce-668">Telemetría</span><span class="sxs-lookup"><span data-stu-id="be8ce-668">Telemetry</span></span>

* <span data-ttu-id="be8ce-669">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="be8ce-669">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-670">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-670">ACR</span></span>

* <span data-ttu-id="be8ce-671">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-671">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="be8ce-672">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="be8ce-672">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-673">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-673">ACS</span></span>

* <span data-ttu-id="be8ce-674">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="be8ce-674">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="be8ce-675">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="be8ce-675">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="be8ce-676">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="be8ce-676">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="be8ce-677">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="be8ce-677">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="be8ce-678">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="be8ce-678">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="be8ce-679">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-679">AppService</span></span>

* <span data-ttu-id="be8ce-680">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="be8ce-680">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="be8ce-681">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="be8ce-681">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="be8ce-682">BatchAI</span><span class="sxs-lookup"><span data-stu-id="be8ce-682">BatchAI</span></span>

* <span data-ttu-id="be8ce-683">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="be8ce-683">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="be8ce-684">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-684">Container</span></span>

* <span data-ttu-id="be8ce-685">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-685">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="be8ce-686">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-686">IoT</span></span>

* <span data-ttu-id="be8ce-687">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="be8ce-687">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="be8ce-688">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="be8ce-688">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="be8ce-689">Iot Central</span><span class="sxs-lookup"><span data-stu-id="be8ce-689">Iot Central</span></span>

* <span data-ttu-id="be8ce-690">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="be8ce-690">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-691">KeyVault</span><span class="sxs-lookup"><span data-stu-id="be8ce-691">KeyVault</span></span>


* <span data-ttu-id="be8ce-692">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="be8ce-692">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="be8ce-693">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="be8ce-693">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="be8ce-694">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="be8ce-694">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="be8ce-695">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="be8ce-695">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="be8ce-696">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="be8ce-696">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="be8ce-697">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-697">Relay</span></span>

* <span data-ttu-id="be8ce-698">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="be8ce-698">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-699">Sql</span><span class="sxs-lookup"><span data-stu-id="be8ce-699">Sql</span></span>

* <span data-ttu-id="be8ce-700">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-700">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-701">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-701">Storage</span></span>

* <span data-ttu-id="be8ce-702">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="be8ce-702">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="be8ce-703">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="be8ce-703">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="be8ce-704">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="be8ce-704">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="be8ce-705">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="be8ce-705">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="be8ce-706">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-706">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-707">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-707">VM</span></span>

* <span data-ttu-id="be8ce-708">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="be8ce-708">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="be8ce-709">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-709">July 31, 2018</span></span>

<span data-ttu-id="be8ce-710">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="be8ce-710">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-711">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-711">ACR</span></span>

* <span data-ttu-id="be8ce-712">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-712">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="be8ce-713">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-713">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-714">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-714">ACS</span></span>

* <span data-ttu-id="be8ce-715">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="be8ce-715">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-716">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-716">Batch</span></span>

* <span data-ttu-id="be8ce-717">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="be8ce-717">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-718">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-718">Container</span></span>

* <span data-ttu-id="be8ce-719">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="be8ce-719">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-720">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-720">Network</span></span>

* <span data-ttu-id="be8ce-721">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="be8ce-721">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="be8ce-722">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-722">Resource</span></span>

* <span data-ttu-id="be8ce-723">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="be8ce-723">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="be8ce-724">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="be8ce-724">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-725">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-725">Role</span></span>

* <span data-ttu-id="be8ce-726">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="be8ce-726">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="be8ce-727">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="be8ce-727">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="be8ce-728">Search</span><span class="sxs-lookup"><span data-stu-id="be8ce-728">Search</span></span>

* <span data-ttu-id="be8ce-729">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="be8ce-729">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="be8ce-730">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="be8ce-730">Service Bus</span></span>

* <span data-ttu-id="be8ce-731">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="be8ce-731">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="be8ce-732">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="be8ce-732">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="be8ce-733">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="be8ce-733">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="be8ce-734">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="be8ce-734">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-735">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-735">Storage</span></span>

* <span data-ttu-id="be8ce-736">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="be8ce-736">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="be8ce-737">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-737">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-738">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-738">VM</span></span>

* <span data-ttu-id="be8ce-739">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="be8ce-739">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="be8ce-740">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="be8ce-740">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="be8ce-741">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="be8ce-741">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="be8ce-742">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="be8ce-742">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="be8ce-743">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-743">July 18, 2018</span></span>

<span data-ttu-id="be8ce-744">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="be8ce-744">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-745">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-745">Core</span></span>

* <span data-ttu-id="be8ce-746">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="be8ce-746">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="be8ce-747">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="be8ce-747">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="be8ce-748">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-748">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-749">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-749">ACR</span></span>

* <span data-ttu-id="be8ce-750">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="be8ce-750">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="be8ce-751">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="be8ce-751">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="be8ce-752">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="be8ce-752">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="be8ce-753">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="be8ce-753">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-754">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-754">ACS</span></span>

* <span data-ttu-id="be8ce-755">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="be8ce-755">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-756">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-756">AppService</span></span>

* <span data-ttu-id="be8ce-757">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="be8ce-757">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-758">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-758">Batch</span></span>

* <span data-ttu-id="be8ce-759">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="be8ce-759">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="be8ce-760">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="be8ce-760">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="be8ce-761">Batch AI</span><span class="sxs-lookup"><span data-stu-id="be8ce-761">Batch AI</span></span>

* <span data-ttu-id="be8ce-762">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="be8ce-762">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-763">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-763">Container</span></span>

* <span data-ttu-id="be8ce-764">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="be8ce-764">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="be8ce-765">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="be8ce-765">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-766">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-766">Network</span></span>

* <span data-ttu-id="be8ce-767">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-767">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="be8ce-768">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-768">Added `network nic wait`</span></span>
* <span data-ttu-id="be8ce-769">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="be8ce-769">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="be8ce-770">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-770">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="be8ce-771">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-771">Resource</span></span>

* <span data-ttu-id="be8ce-772">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="be8ce-772">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="be8ce-773">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="be8ce-773">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="be8ce-774">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-774">Added `deployment wait` command</span></span>
* <span data-ttu-id="be8ce-775">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="be8ce-775">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-776">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-776">SQL</span></span>

* <span data-ttu-id="be8ce-777">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-777">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="be8ce-778">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="be8ce-778">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="be8ce-779">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="be8ce-779">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-780">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-780">Storage</span></span>

* <span data-ttu-id="be8ce-781">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="be8ce-781">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-782">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-782">VM</span></span>

* <span data-ttu-id="be8ce-783">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="be8ce-783">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="be8ce-784">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-784">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="be8ce-785">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-785">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="be8ce-786">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-786">July 3, 2018</span></span>

<span data-ttu-id="be8ce-787">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="be8ce-787">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="be8ce-788">AKS</span><span class="sxs-lookup"><span data-stu-id="be8ce-788">AKS</span></span>

* <span data-ttu-id="be8ce-789">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="be8ce-789">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="be8ce-790">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-790">July 3, 2018</span></span>

<span data-ttu-id="be8ce-791">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="be8ce-791">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-792">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-792">Core</span></span>

* <span data-ttu-id="be8ce-793">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="be8ce-793">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-794">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-794">ACR</span></span>

* <span data-ttu-id="be8ce-795">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="be8ce-795">Added polling build status</span></span>
* <span data-ttu-id="be8ce-796">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="be8ce-796">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="be8ce-797">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="be8ce-797">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-798">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-798">ACS</span></span>

* <span data-ttu-id="be8ce-799">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-799">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="be8ce-800">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="be8ce-800">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="be8ce-801">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-801">Updated options for `aks browse` command.</span></span> <span data-ttu-id="be8ce-802">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="be8ce-802">Added `--listen-port` support</span></span>
* <span data-ttu-id="be8ce-803">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-803">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="be8ce-804">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="be8ce-804">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="be8ce-805">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="be8ce-805">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-806">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-806">AppService</span></span>

* <span data-ttu-id="be8ce-807">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="be8ce-807">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="be8ce-808">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="be8ce-808">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="be8ce-809">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="be8ce-809">Backup</span></span>

* <span data-ttu-id="be8ce-810">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="be8ce-810">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="be8ce-811">BatchAI</span><span class="sxs-lookup"><span data-stu-id="be8ce-811">BatchAI</span></span>

* <span data-ttu-id="be8ce-812">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-812">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="be8ce-813">Nube</span><span class="sxs-lookup"><span data-stu-id="be8ce-813">Cloud</span></span>

* <span data-ttu-id="be8ce-814">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="be8ce-814">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-815">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-815">Container</span></span>

* <span data-ttu-id="be8ce-816">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="be8ce-816">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="be8ce-817">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="be8ce-817">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="be8ce-818">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="be8ce-818">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-819">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-819">Extension</span></span>

* <span data-ttu-id="be8ce-820">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="be8ce-820">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-821">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-821">Network</span></span>

* <span data-ttu-id="be8ce-822">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="be8ce-822">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-823">Rdbms</span><span class="sxs-lookup"><span data-stu-id="be8ce-823">Rdbms</span></span>

* <span data-ttu-id="be8ce-824">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-824">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-825">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-825">Resource</span></span>

* <span data-ttu-id="be8ce-826">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="be8ce-826">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-827">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-827">VM</span></span>

* <span data-ttu-id="be8ce-828">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="be8ce-828">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="be8ce-829">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-829">June 25, 2018</span></span>

<span data-ttu-id="be8ce-830">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="be8ce-830">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="be8ce-831">CLI</span><span class="sxs-lookup"><span data-stu-id="be8ce-831">CLI</span></span>

* <span data-ttu-id="be8ce-832">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-832">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="be8ce-833">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-833">June 19, 2018</span></span>

<span data-ttu-id="be8ce-834">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="be8ce-834">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-835">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-835">Core</span></span>

* <span data-ttu-id="be8ce-836">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-836">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-837">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-837">ACR</span></span>

* <span data-ttu-id="be8ce-838">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="be8ce-838">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="be8ce-839">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="be8ce-839">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-840">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-840">ACS</span></span>

* <span data-ttu-id="be8ce-841">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-841">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="be8ce-842">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-842">Added `--update` support</span></span>
* <span data-ttu-id="be8ce-843">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="be8ce-843">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="be8ce-844">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="be8ce-844">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="be8ce-845">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="be8ce-845">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="be8ce-846">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="be8ce-846">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="be8ce-847">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="be8ce-847">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="be8ce-848">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="be8ce-848">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-849">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-849">AppService</span></span>

* <span data-ttu-id="be8ce-850">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="be8ce-850">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="be8ce-851">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="be8ce-851">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-852">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-852">Batch</span></span>

* <span data-ttu-id="be8ce-853">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="be8ce-853">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="be8ce-854">Batch AI</span><span class="sxs-lookup"><span data-stu-id="be8ce-854">Batch AI</span></span>

* <span data-ttu-id="be8ce-855">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-855">Added support for workspaces.</span></span> <span data-ttu-id="be8ce-856">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="be8ce-856">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="be8ce-857">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-857">Added support for experiments.</span></span> <span data-ttu-id="be8ce-858">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="be8ce-858">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="be8ce-859">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="be8ce-859">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="be8ce-860">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-860">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="be8ce-861">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-861">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="be8ce-862">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-862">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="be8ce-863">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-863">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="be8ce-864">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-864">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="be8ce-865">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-865">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="be8ce-866">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-866">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="be8ce-867">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-867">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="be8ce-868">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-868">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="be8ce-869">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-869">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="be8ce-870">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-870">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="be8ce-871">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-871">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="be8ce-872">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="be8ce-872">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="be8ce-873">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="be8ce-873">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="be8ce-874">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="be8ce-874">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="be8ce-875">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="be8ce-875">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="be8ce-876">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="be8ce-876">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="be8ce-877">Mapas</span><span class="sxs-lookup"><span data-stu-id="be8ce-877">Maps</span></span>

* <span data-ttu-id="be8ce-878">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-878">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-879">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-879">Network</span></span>

* <span data-ttu-id="be8ce-880">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="be8ce-880">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="be8ce-881">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-881">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="be8ce-882">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="be8ce-882">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="be8ce-883">Reservations</span><span class="sxs-lookup"><span data-stu-id="be8ce-883">Reservations</span></span>

* <span data-ttu-id="be8ce-884">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-884">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="be8ce-885">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-885">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="be8ce-886">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-886">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="be8ce-887">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-887">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="be8ce-888">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-888">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="be8ce-889">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-889">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-890">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-890">Role</span></span>

* <span data-ttu-id="be8ce-891">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="be8ce-891">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-892">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-892">SQL</span></span>

* <span data-ttu-id="be8ce-893">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="be8ce-893">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-894">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-894">Storage</span></span>

* <span data-ttu-id="be8ce-895">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="be8ce-895">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-896">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-896">VM</span></span>

* <span data-ttu-id="be8ce-897">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-897">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="be8ce-898">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="be8ce-898">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="be8ce-899">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="be8ce-899">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="be8ce-900">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-900">June 13, 2018</span></span>

<span data-ttu-id="be8ce-901">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="be8ce-901">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-902">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-902">Core</span></span>

* <span data-ttu-id="be8ce-903">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="be8ce-903">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="be8ce-904">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-904">June 13, 2018</span></span>

<span data-ttu-id="be8ce-905">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="be8ce-905">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="be8ce-906">AKS</span><span class="sxs-lookup"><span data-stu-id="be8ce-906">AKS</span></span>

* <span data-ttu-id="be8ce-907">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-907">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="be8ce-908">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="be8ce-908">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="be8ce-909">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-909">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="be8ce-910">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-910">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="be8ce-911">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-911">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-912">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-912">AppService</span></span>

* <span data-ttu-id="be8ce-913">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="be8ce-913">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="be8ce-914">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-914">June 5, 2018</span></span>

<span data-ttu-id="be8ce-915">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="be8ce-915">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-916">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-916">Interactive</span></span>

* <span data-ttu-id="be8ce-917">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="be8ce-917">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="be8ce-918">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-918">June 5, 2018</span></span>

<span data-ttu-id="be8ce-919">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="be8ce-919">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-920">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-920">Core</span></span>

* <span data-ttu-id="be8ce-921">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="be8ce-921">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="be8ce-922">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="be8ce-922">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-923">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-923">ACR</span></span>

* <span data-ttu-id="be8ce-924">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="be8ce-924">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="be8ce-925">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-925">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="be8ce-926">AKS</span><span class="sxs-lookup"><span data-stu-id="be8ce-926">AKS</span></span>

* <span data-ttu-id="be8ce-927">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="be8ce-927">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-928">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-928">Batch</span></span>

* <span data-ttu-id="be8ce-929">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="be8ce-929">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-930">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-930">IOT</span></span>

* <span data-ttu-id="be8ce-931">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="be8ce-931">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-932">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-932">Network</span></span>

* <span data-ttu-id="be8ce-933">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="be8ce-933">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="be8ce-934">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="be8ce-934">Policy Insights</span></span>

* <span data-ttu-id="be8ce-935">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="be8ce-935">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="be8ce-936">ARM</span><span class="sxs-lookup"><span data-stu-id="be8ce-936">ARM</span></span>

* <span data-ttu-id="be8ce-937">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-937">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-938">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-938">SQL</span></span>

* <span data-ttu-id="be8ce-939">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="be8ce-939">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="be8ce-940">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="be8ce-940">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="be8ce-941">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-941">Storage</span></span>

* <span data-ttu-id="be8ce-942">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="be8ce-942">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-943">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-943">VM</span></span>

* <span data-ttu-id="be8ce-944">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="be8ce-944">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="be8ce-945">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-945">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="be8ce-946">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-946">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="be8ce-947">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-947">May 22, 2018</span></span>

<span data-ttu-id="be8ce-948">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="be8ce-948">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-949">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-949">Core</span></span>

* <span data-ttu-id="be8ce-950">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="be8ce-950">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-951">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-951">ACS</span></span>

* <span data-ttu-id="be8ce-952">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="be8ce-952">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="be8ce-953">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="be8ce-953">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-954">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-954">AppService</span></span>

* <span data-ttu-id="be8ce-955">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="be8ce-955">Improved generic update commands</span></span>
* <span data-ttu-id="be8ce-956">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="be8ce-956">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-957">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-957">Container</span></span>

* <span data-ttu-id="be8ce-958">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="be8ce-958">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="be8ce-959">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-959">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-960">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-960">Extension</span></span>

* <span data-ttu-id="be8ce-961">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="be8ce-961">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-962">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-962">Interactive</span></span>

* <span data-ttu-id="be8ce-963">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="be8ce-963">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="be8ce-964">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="be8ce-964">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-965">KeyVault</span><span class="sxs-lookup"><span data-stu-id="be8ce-965">KeyVault</span></span>

* <span data-ttu-id="be8ce-966">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="be8ce-966">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-967">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-967">Network</span></span>

* <span data-ttu-id="be8ce-968">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="be8ce-968">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="be8ce-969">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="be8ce-969">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-970">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-970">SQL</span></span>

* <span data-ttu-id="be8ce-971">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="be8ce-971">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="be8ce-972">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="be8ce-972">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="be8ce-973">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="be8ce-973">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="be8ce-974">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="be8ce-974">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="be8ce-975">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="be8ce-975">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="be8ce-976">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-976">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="be8ce-977">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="be8ce-977">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="be8ce-978">`edition`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-978">`edition`.</span></span> <span data-ttu-id="be8ce-979">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="be8ce-979">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="be8ce-980">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-980">`elasticPoolName`.</span></span> <span data-ttu-id="be8ce-981">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="be8ce-981">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="be8ce-982">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="be8ce-982">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="be8ce-983">`edition`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-983">`edition`.</span></span> <span data-ttu-id="be8ce-984">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="be8ce-984">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="be8ce-985">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-985">`dtu`.</span></span> <span data-ttu-id="be8ce-986">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="be8ce-986">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="be8ce-987">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-987">`databaseDtuMin`.</span></span> <span data-ttu-id="be8ce-988">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="be8ce-988">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="be8ce-989">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-989">`databaseDtuMax`.</span></span> <span data-ttu-id="be8ce-990">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="be8ce-990">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="be8ce-991">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-991">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="be8ce-992">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-992">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-993">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-993">Storage</span></span>

* <span data-ttu-id="be8ce-994">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="be8ce-994">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="be8ce-995">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="be8ce-995">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-996">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-996">VM</span></span>

* <span data-ttu-id="be8ce-997">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-997">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="be8ce-998">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="be8ce-998">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="be8ce-999">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="be8ce-999">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="be8ce-1000">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="be8ce-1000">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="be8ce-1001">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1001">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="be8ce-1002">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1002">May 7, 2018</span></span>

<span data-ttu-id="be8ce-1003">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="be8ce-1003">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1004">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1004">Core</span></span>

* <span data-ttu-id="be8ce-1005">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="be8ce-1005">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="be8ce-1006">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="be8ce-1006">Added limited support for positional arguments</span></span>
* <span data-ttu-id="be8ce-1007">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1007">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="be8ce-1008">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="be8ce-1008">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="be8ce-1009">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1009">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="be8ce-1010">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="be8ce-1010">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="be8ce-1011">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1011">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="be8ce-1012">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1012">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="be8ce-1013">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1013">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-1014">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-1014">ACR</span></span>

* <span data-ttu-id="be8ce-1015">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="be8ce-1015">Added ACR Build commands</span></span>
* <span data-ttu-id="be8ce-1016">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="be8ce-1016">Improved resource not found error messages</span></span>
* <span data-ttu-id="be8ce-1017">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="be8ce-1017">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="be8ce-1018">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1018">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="be8ce-1019">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-1019">Improved repository commands error messages</span></span>
* <span data-ttu-id="be8ce-1020">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="be8ce-1020">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1021">ACS</span></span>

* <span data-ttu-id="be8ce-1022">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1022">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="be8ce-1023">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1023">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="be8ce-1024">AMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1024">AMS</span></span>

* <span data-ttu-id="be8ce-1025">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="be8ce-1025">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1026">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1026">Appservice</span></span>

* <span data-ttu-id="be8ce-1027">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1027">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="be8ce-1028">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1028">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="be8ce-1029">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="be8ce-1029">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="be8ce-1030">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-1030">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="be8ce-1031">Batch AI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1031">Batch AI</span></span>

* <span data-ttu-id="be8ce-1032">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="be8ce-1032">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="be8ce-1033">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="be8ce-1033">Cognitive Services</span></span>

* <span data-ttu-id="be8ce-1034">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1034">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="be8ce-1035">Consumo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1035">Consumption</span></span>

* <span data-ttu-id="be8ce-1036">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1036">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1037">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1037">Container</span></span>

* <span data-ttu-id="be8ce-1038">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="be8ce-1038">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="be8ce-1039">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="be8ce-1039">Cosmos DB</span></span>

* <span data-ttu-id="be8ce-1040">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="be8ce-1040">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="be8ce-1041">DMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1041">DMS</span></span>

* <span data-ttu-id="be8ce-1042">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1042">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-1043">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1043">Extension</span></span>

* <span data-ttu-id="be8ce-1044">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="be8ce-1044">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1045">Interactive</span></span>

* <span data-ttu-id="be8ce-1046">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="be8ce-1046">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="be8ce-1047">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="be8ce-1047">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="be8ce-1048">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="be8ce-1048">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="be8ce-1049">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1049">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="be8ce-1050">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-1050">Lab</span></span>

* <span data-ttu-id="be8ce-1051">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="be8ce-1051">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1052">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1052">Network</span></span>

* <span data-ttu-id="be8ce-1053">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1053">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="be8ce-1054">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1054">Profile</span></span>

* <span data-ttu-id="be8ce-1055">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1055">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="be8ce-1056">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="be8ce-1056">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="be8ce-1057">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1057">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="be8ce-1058">Redis</span><span class="sxs-lookup"><span data-stu-id="be8ce-1058">Redis</span></span>

* <span data-ttu-id="be8ce-1059">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1059">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="be8ce-1060">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1060">Deprecated `redis list-all`.</span></span> <span data-ttu-id="be8ce-1061">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1061">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="be8ce-1062">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1062">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="be8ce-1063">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1063">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-1064">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-1064">Role</span></span>

* <span data-ttu-id="be8ce-1065">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1065">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1066">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1066">Storage</span></span>

* <span data-ttu-id="be8ce-1067">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="be8ce-1067">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="be8ce-1068">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="be8ce-1068">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="be8ce-1069">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1069">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="be8ce-1070">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="be8ce-1070">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="be8ce-1071">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="be8ce-1071">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1072">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1072">VM</span></span>

* <span data-ttu-id="be8ce-1073">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="be8ce-1073">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="be8ce-1074">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="be8ce-1074">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="be8ce-1075">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1075">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="be8ce-1076">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1076">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="be8ce-1077">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1077">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="be8ce-1078">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="be8ce-1078">Added write accelerator support</span></span>
* <span data-ttu-id="be8ce-1079">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1079">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="be8ce-1080">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="be8ce-1080">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="be8ce-1081">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="be8ce-1081">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="be8ce-1082">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1082">April 10, 2018</span></span>

<span data-ttu-id="be8ce-1083">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="be8ce-1083">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-1084">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-1084">ACR</span></span>

* <span data-ttu-id="be8ce-1085">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="be8ce-1085">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1086">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1086">ACS</span></span>

* <span data-ttu-id="be8ce-1087">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="be8ce-1087">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1088">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1088">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="be8ce-1090">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="be8ce-1090">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="be8ce-1091">BatchAI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1091">BatchAI</span></span>

* <span data-ttu-id="be8ce-1092">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="be8ce-1092">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="be8ce-1093">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1093">Job level mounting</span></span>
  - <span data-ttu-id="be8ce-1094">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="be8ce-1094">Environment variables with secret values</span></span>
  - <span data-ttu-id="be8ce-1095">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1095">Performance counters settings</span></span>
  - <span data-ttu-id="be8ce-1096">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1096">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="be8ce-1097">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1097">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="be8ce-1098">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="be8ce-1098">Usage and limits reporting</span></span>
  - <span data-ttu-id="be8ce-1099">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1099">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="be8ce-1100">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1100">Support for custom images</span></span>
  - <span data-ttu-id="be8ce-1101">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1101">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="be8ce-1102">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1102">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="be8ce-1103">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="be8ce-1103">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="be8ce-1104">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="be8ce-1104">National clouds are supported</span></span>
* <span data-ttu-id="be8ce-1105">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="be8ce-1105">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="be8ce-1106">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="be8ce-1106">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="be8ce-1107">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1107">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="be8ce-1108">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1108">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="be8ce-1109">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1109">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="be8ce-1110">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1110">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="be8ce-1111">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1111">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="be8ce-1112">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1112">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="be8ce-1113">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="be8ce-1113">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="be8ce-1114">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1114">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="be8ce-1115">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1115">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="be8ce-1116">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1116">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="be8ce-1117">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1117">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="be8ce-1118">Facturación</span><span class="sxs-lookup"><span data-stu-id="be8ce-1118">Billing</span></span>

* <span data-ttu-id="be8ce-1119">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="be8ce-1119">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="be8ce-1120">Consumo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1120">Consumption</span></span>

* <span data-ttu-id="be8ce-1121">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1121">Added `marketplace` commands</span></span>
* <span data-ttu-id="be8ce-1122">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1122">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="be8ce-1123">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1123">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="be8ce-1124">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1124">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="be8ce-1125">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1125">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="be8ce-1126">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1126">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1127">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1127">Container</span></span>

* <span data-ttu-id="be8ce-1128">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1128">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="be8ce-1129">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="be8ce-1129">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-1130">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1130">Extension</span></span>

* <span data-ttu-id="be8ce-1131">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="be8ce-1131">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1132">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1132">Interactive</span></span>

* <span data-ttu-id="be8ce-1133">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1133">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="be8ce-1134">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1134">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="be8ce-1135">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1135">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1136">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1136">Network</span></span>

* <span data-ttu-id="be8ce-1137">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1137">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="be8ce-1138">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1138">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="be8ce-1139">4910</span><span class="sxs-lookup"><span data-stu-id="be8ce-1139">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="be8ce-1140">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="be8ce-1140">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="be8ce-1141">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="be8ce-1141">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="be8ce-1142">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1142">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="be8ce-1143">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1143">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="be8ce-1144">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1144">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1145">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1145">Profile</span></span>

* <span data-ttu-id="be8ce-1146">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1146">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="be8ce-1147">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1147">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-1148">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1148">RDBMS</span></span>

* <span data-ttu-id="be8ce-1149">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1149">Added `georestore` command</span></span>
* <span data-ttu-id="be8ce-1150">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1150">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1151">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1151">Resource</span></span>

* <span data-ttu-id="be8ce-1152">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1152">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="be8ce-1153">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1153">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1154">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1154">SQL</span></span>

* <span data-ttu-id="be8ce-1155">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1155">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1156">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1156">Storage</span></span>

* <span data-ttu-id="be8ce-1157">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="be8ce-1157">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1158">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1158">VM</span></span>

* <span data-ttu-id="be8ce-1159">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1159">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="be8ce-1160">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="be8ce-1160">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="be8ce-1162">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1162">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="be8ce-1163">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1163">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="be8ce-1164">5718</span><span class="sxs-lookup"><span data-stu-id="be8ce-1164">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="be8ce-1165">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1165">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="be8ce-1166">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1166">March 27, 2018</span></span>

<span data-ttu-id="be8ce-1167">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="be8ce-1167">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1168">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1168">Core</span></span>

* <span data-ttu-id="be8ce-1169">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="be8ce-1169">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1170">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1170">ACS</span></span>

* <span data-ttu-id="be8ce-1171">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="be8ce-1171">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1172">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1172">Appservice</span></span>

* <span data-ttu-id="be8ce-1173">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1173">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="be8ce-1174">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1174">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="be8ce-1175">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="be8ce-1175">Backup</span></span>

* <span data-ttu-id="be8ce-1176">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1176">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="be8ce-1177">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1177">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="be8ce-1178">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1178">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="be8ce-1179">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1179">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1180">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1180">Container</span></span>

* <span data-ttu-id="be8ce-1181">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1181">Added `container exec` command.</span></span> <span data-ttu-id="be8ce-1182">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="be8ce-1182">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="be8ce-1183">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-1183">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-1184">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1184">Extension</span></span>

* <span data-ttu-id="be8ce-1185">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1185">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="be8ce-1186">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1186">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="be8ce-1187">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="be8ce-1187">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1188">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1188">Interactive</span></span>

* <span data-ttu-id="be8ce-1189">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1189">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="be8ce-1190">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1190">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="be8ce-1191">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1191">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="be8ce-1192">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="be8ce-1192">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="be8ce-1193">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-1193">Lab</span></span>

* <span data-ttu-id="be8ce-1194">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1194">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1195">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1195">Monitor</span></span>

* <span data-ttu-id="be8ce-1196">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1196">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="be8ce-1197">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1197">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="be8ce-1198">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1198">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1199">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1199">Network</span></span>

* <span data-ttu-id="be8ce-1200">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1200">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1201">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1201">Profile</span></span>

* <span data-ttu-id="be8ce-1202">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1202">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-1203">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1203">RDBMS</span></span>

* <span data-ttu-id="be8ce-1204">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="be8ce-1204">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1205">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1205">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="be8ce-1207">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-1207">Role</span></span>

* <span data-ttu-id="be8ce-1208">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1208">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="be8ce-1209">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="be8ce-1209">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="be8ce-1210">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1210">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="be8ce-1211">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1211">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="be8ce-1212">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1212">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1213">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1213">Storage</span></span>

* <span data-ttu-id="be8ce-1214">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="be8ce-1214">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="be8ce-1215">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="be8ce-1215">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1216">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1216">VM</span></span>

* <span data-ttu-id="be8ce-1217">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="be8ce-1217">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="be8ce-1218">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1218">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="be8ce-1219">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="be8ce-1219">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="be8ce-1220">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="be8ce-1220">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="be8ce-1221">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1221">March 13, 2018</span></span>

<span data-ttu-id="be8ce-1222">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="be8ce-1222">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-1223">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-1223">ACR</span></span>

* <span data-ttu-id="be8ce-1224">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1224">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="be8ce-1225">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1225">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="be8ce-1226">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1226">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1227">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1227">ACS</span></span>

* <span data-ttu-id="be8ce-1228">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1228">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="be8ce-1229">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1229">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="be8ce-1230">Advisor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1230">Advisor</span></span>

* <span data-ttu-id="be8ce-1231">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1231">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="be8ce-1232">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1232">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="be8ce-1233">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1233">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="be8ce-1234">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1234">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="be8ce-1235">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1235">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1236">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1236">Appservice</span></span>

* <span data-ttu-id="be8ce-1237">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1237">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="be8ce-1238">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1238">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="be8ce-1239">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="be8ce-1239">Eventhubs</span></span>

* <span data-ttu-id="be8ce-1240">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1240">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-1241">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1241">Extension</span></span>

* <span data-ttu-id="be8ce-1242">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1242">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1243">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1243">Interactive</span></span>

* <span data-ttu-id="be8ce-1244">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1244">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="be8ce-1245">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1245">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="be8ce-1246">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1246">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="be8ce-1247">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1247">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1248">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1248">Monitor</span></span>

* <span data-ttu-id="be8ce-1249">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1249">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="be8ce-1250">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1250">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="be8ce-1251">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1251">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="be8ce-1252">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1252">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1253">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1253">Network</span></span>

* <span data-ttu-id="be8ce-1254">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1254">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="be8ce-1255">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1255">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="be8ce-1256">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1256">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="be8ce-1257">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1257">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1258">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1258">Profile</span></span>

* <span data-ttu-id="be8ce-1259">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1259">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="be8ce-1260">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1260">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-1261">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1261">RDBMS</span></span>

* <span data-ttu-id="be8ce-1262">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="be8ce-1262">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="be8ce-1263">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="be8ce-1263">Service Bus</span></span>

* <span data-ttu-id="be8ce-1264">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1264">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1265">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1265">Storage</span></span>

* <span data-ttu-id="be8ce-1266">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1266">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="be8ce-1267">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1267">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1268">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1268">VM</span></span>

* <span data-ttu-id="be8ce-1269">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1269">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="be8ce-1270">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1270">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="be8ce-1271">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1271">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="be8ce-1272">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1272">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="be8ce-1273">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1273">February 27, 2018</span></span>

<span data-ttu-id="be8ce-1274">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="be8ce-1274">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1275">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1275">Core</span></span>

* <span data-ttu-id="be8ce-1276">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="be8ce-1276">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="be8ce-1277">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1277">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="be8ce-1278">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1278">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1279">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1279">ACS</span></span>

* <span data-ttu-id="be8ce-1280">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="be8ce-1280">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="be8ce-1281">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1281">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="be8ce-1282">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1282">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="be8ce-1283">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1283">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1284">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1284">Appservice</span></span>

* <span data-ttu-id="be8ce-1285">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1285">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="be8ce-1286">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="be8ce-1286">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="be8ce-1287">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="be8ce-1287">Cognitive Services</span></span>

* <span data-ttu-id="be8ce-1288">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="be8ce-1288">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="be8ce-1289">Consumo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1289">Consumption</span></span>

* <span data-ttu-id="be8ce-1290">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="be8ce-1290">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="be8ce-1291">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="be8ce-1291">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1292">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1292">Container</span></span>

* <span data-ttu-id="be8ce-1293">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1293">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1294">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1294">Network</span></span>

* <span data-ttu-id="be8ce-1295">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1295">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1296">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1296">Resource</span></span>

* <span data-ttu-id="be8ce-1297">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="be8ce-1297">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-1298">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-1298">Role</span></span>

* <span data-ttu-id="be8ce-1299">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="be8ce-1299">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1300">SQL</span></span>

* <span data-ttu-id="be8ce-1301">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="be8ce-1301">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1302">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1302">Storage</span></span>

* <span data-ttu-id="be8ce-1303">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1303">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1304">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1304">VM</span></span>

* <span data-ttu-id="be8ce-1305">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1305">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="be8ce-1306">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1306">February 13, 2018</span></span>

<span data-ttu-id="be8ce-1307">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="be8ce-1307">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1308">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1308">Core</span></span>

* <span data-ttu-id="be8ce-1309">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="be8ce-1309">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1310">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1310">ACS</span></span>

* <span data-ttu-id="be8ce-1311">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1311">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="be8ce-1312">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1312">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="be8ce-1313">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="be8ce-1313">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="be8ce-1314">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1314">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="be8ce-1315">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="be8ce-1315">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="be8ce-1316">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1316">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="be8ce-1317">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="be8ce-1317">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="be8ce-1318">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1318">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1319">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1319">Appservice</span></span>

* <span data-ttu-id="be8ce-1320">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="be8ce-1320">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="be8ce-1321">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1321">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="be8ce-1322">CDN</span><span class="sxs-lookup"><span data-stu-id="be8ce-1322">CDN</span></span>

* <span data-ttu-id="be8ce-1323">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1323">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1324">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1324">Container</span></span>

* <span data-ttu-id="be8ce-1325">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="be8ce-1325">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="be8ce-1326">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-1326">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be8ce-1327">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-1327">CosmosDB</span></span>

* <span data-ttu-id="be8ce-1328">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="be8ce-1328">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-1329">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1329">Extension</span></span>

* <span data-ttu-id="be8ce-1330">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1330">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="be8ce-1331">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1331">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="be8ce-1332">Comentarios</span><span class="sxs-lookup"><span data-stu-id="be8ce-1332">Feedback</span></span>

* <span data-ttu-id="be8ce-1333">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="be8ce-1333">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1334">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1334">Interactive</span></span>

* <span data-ttu-id="be8ce-1335">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="be8ce-1335">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="be8ce-1336">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="be8ce-1336">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-1337">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-1337">IoT</span></span>

* <span data-ttu-id="be8ce-1338">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1338">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="be8ce-1339">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1339">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="be8ce-1340">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1340">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="be8ce-1341">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="be8ce-1341">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1342">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1342">Monitor</span></span>

* <span data-ttu-id="be8ce-1343">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1343">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1344">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1344">Network</span></span>

* <span data-ttu-id="be8ce-1345">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1345">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="be8ce-1346">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1346">Profile</span></span>

* <span data-ttu-id="be8ce-1347">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1347">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1348">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1348">Resource</span></span>

* <span data-ttu-id="be8ce-1349">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1349">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-1350">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-1350">Role</span></span>

* <span data-ttu-id="be8ce-1351">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1351">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1352">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1352">SQL</span></span>

* <span data-ttu-id="be8ce-1353">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1353">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="be8ce-1354">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1354">Added `sql db rename`</span></span>
* <span data-ttu-id="be8ce-1355">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="be8ce-1355">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1356">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1356">Storage</span></span>

* <span data-ttu-id="be8ce-1357">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="be8ce-1357">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1358">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1358">VM</span></span>

* <span data-ttu-id="be8ce-1359">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="be8ce-1359">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="be8ce-1360">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1360">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="be8ce-1361">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="be8ce-1361">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="be8ce-1362">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1362">January 31, 2018</span></span>

<span data-ttu-id="be8ce-1363">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="be8ce-1363">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1364">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1364">Core</span></span>

* <span data-ttu-id="be8ce-1365">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1365">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="be8ce-1366">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="be8ce-1366">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="be8ce-1367">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1367">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="be8ce-1368">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1368">Use `--verbose` to see</span></span>
* <span data-ttu-id="be8ce-1369">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="be8ce-1369">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1370">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1370">ACS</span></span>

* <span data-ttu-id="be8ce-1371">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1371">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="be8ce-1372">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1372">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1373">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1373">Appservice</span></span>

* <span data-ttu-id="be8ce-1374">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="be8ce-1374">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="be8ce-1375">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="be8ce-1375">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="be8ce-1376">CDN</span><span class="sxs-lookup"><span data-stu-id="be8ce-1376">CDN</span></span>

* <span data-ttu-id="be8ce-1377">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1377">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be8ce-1378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-1378">CosmosDB</span></span>

* <span data-ttu-id="be8ce-1379">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="be8ce-1379">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1380">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1380">Interactive</span></span>

* <span data-ttu-id="be8ce-1381">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="be8ce-1381">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1382">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1382">Network</span></span>

* <span data-ttu-id="be8ce-1383">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1383">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="be8ce-1384">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="be8ce-1384">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="be8ce-1385">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1385">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="be8ce-1386">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1386">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="be8ce-1387">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1387">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="be8ce-1388">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1388">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="be8ce-1389">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1389">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="be8ce-1390">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="be8ce-1390">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="be8ce-1391">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1391">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="be8ce-1392">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1392">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1393">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1393">Profile</span></span>

* <span data-ttu-id="be8ce-1394">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="be8ce-1394">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1395">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1395">Resource</span></span>

* <span data-ttu-id="be8ce-1396">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1396">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1397">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1397">Storage</span></span>

* <span data-ttu-id="be8ce-1398">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="be8ce-1398">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="be8ce-1399">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="be8ce-1399">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="be8ce-1400">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1400">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="be8ce-1401">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1401">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="be8ce-1402">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="be8ce-1402">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1403">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1403">VM</span></span>

* <span data-ttu-id="be8ce-1404">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="be8ce-1404">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="be8ce-1405">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1405">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="be8ce-1406">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="be8ce-1406">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="be8ce-1407">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1407">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="be8ce-1408">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="be8ce-1408">January 17, 2018</span></span>

<span data-ttu-id="be8ce-1409">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="be8ce-1409">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-1410">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-1410">ACR</span></span>

* <span data-ttu-id="be8ce-1411">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="be8ce-1411">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="be8ce-1412">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="be8ce-1412">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1413">ACS</span></span>

* <span data-ttu-id="be8ce-1414">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1414">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="be8ce-1415">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="be8ce-1415">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1416">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1416">Appservice</span></span>

* <span data-ttu-id="be8ce-1417">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1417">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="be8ce-1418">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1418">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="be8ce-1419">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1419">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="be8ce-1420">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="be8ce-1420">Backup</span></span>

* <span data-ttu-id="be8ce-1421">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="be8ce-1421">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="be8ce-1422">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1422">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="be8ce-1423">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1423">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="be8ce-1424">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="be8ce-1424">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="be8ce-1425">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="be8ce-1425">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-1426">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1426">Batch</span></span>

* <span data-ttu-id="be8ce-1427">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="be8ce-1427">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="be8ce-1428">Nube</span><span class="sxs-lookup"><span data-stu-id="be8ce-1428">Cloud</span></span>

* <span data-ttu-id="be8ce-1429">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="be8ce-1429">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="be8ce-1430">Consumo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1430">Consumption</span></span>

* <span data-ttu-id="be8ce-1431">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1431">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="be8ce-1432">Event Grid</span><span class="sxs-lookup"><span data-stu-id="be8ce-1432">Event Grid</span></span>

* <span data-ttu-id="be8ce-1433">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1433">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="be8ce-1434">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1434">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="be8ce-1435">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1435">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="be8ce-1436">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1436">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="be8ce-1437">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1437">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="be8ce-1438">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1438">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="be8ce-1439">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1439">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="be8ce-1440">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="be8ce-1440">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1441">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1441">Interactive</span></span>

* <span data-ttu-id="be8ce-1442">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="be8ce-1442">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="be8ce-1443">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="be8ce-1443">Fixed errors on startup</span></span>
* <span data-ttu-id="be8ce-1444">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1444">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-1445">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-1445">IoT</span></span>

* <span data-ttu-id="be8ce-1446">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1446">Added support for device provisioning service</span></span>
* <span data-ttu-id="be8ce-1447">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1447">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="be8ce-1448">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-1448">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1449">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1449">Monitor</span></span>

* <span data-ttu-id="be8ce-1450">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1450">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="be8ce-1451">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1451">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="be8ce-1452">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1452">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1453">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1453">Network</span></span>

* <span data-ttu-id="be8ce-1454">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1454">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="be8ce-1455">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1455">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1456">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1456">Profile</span></span>

* <span data-ttu-id="be8ce-1457">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="be8ce-1457">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-1458">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-1458">Role</span></span>

* <span data-ttu-id="be8ce-1459">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="be8ce-1459">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="be8ce-1460">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="be8ce-1460">Service Fabric</span></span>

* <span data-ttu-id="be8ce-1461">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="be8ce-1461">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="be8ce-1462">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1462">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1463">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1463">VM</span></span>

* <span data-ttu-id="be8ce-1464">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1464">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="be8ce-1465">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="be8ce-1465">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="be8ce-1466">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1466">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="be8ce-1467">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1467">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="be8ce-1468">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="be8ce-1468">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="be8ce-1469">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1469">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="be8ce-1470">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1470">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="be8ce-1471">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1471">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="be8ce-1472">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1472">December 19, 2017</span></span>

<span data-ttu-id="be8ce-1473">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="be8ce-1473">Version 2.0.23</span></span>

* <span data-ttu-id="be8ce-1474">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="be8ce-1474">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1475">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1475">Container</span></span>

* <span data-ttu-id="be8ce-1476">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1476">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1477">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1477">Network</span></span>

* <span data-ttu-id="be8ce-1478">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1478">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="be8ce-1479">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1479">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1480">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1480">Storage</span></span>

* <span data-ttu-id="be8ce-1481">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="be8ce-1481">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1482">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1482">VM</span></span>

* <span data-ttu-id="be8ce-1483">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="be8ce-1483">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="be8ce-1484">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1484">December 5, 2017</span></span>

<span data-ttu-id="be8ce-1485">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="be8ce-1485">Version 2.0.22</span></span>

* <span data-ttu-id="be8ce-1486">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1486">Removed `az component` commands.</span></span> <span data-ttu-id="be8ce-1487">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1487">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1488">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1488">Core</span></span>
* <span data-ttu-id="be8ce-1489">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="be8ce-1489">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="be8ce-1490">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="be8ce-1490">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1491">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1491">ACS</span></span>

* <span data-ttu-id="be8ce-1492">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1492">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="be8ce-1493">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1493">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="be8ce-1494">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="be8ce-1494">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="be8ce-1495">Advisor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1495">Advisor</span></span>

* <span data-ttu-id="be8ce-1496">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1496">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1497">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1497">Appservice</span></span>

* <span data-ttu-id="be8ce-1498">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1498">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="be8ce-1499">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1499">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="be8ce-1500">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1500">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="be8ce-1501">Consumo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1501">Consumption</span></span>

* <span data-ttu-id="be8ce-1502">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="be8ce-1502">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1503">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1503">Container</span></span>

* <span data-ttu-id="be8ce-1504">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="be8ce-1504">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1505">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1505">Monitor</span></span>

* <span data-ttu-id="be8ce-1506">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="be8ce-1506">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1507">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1507">Resource</span></span>

* <span data-ttu-id="be8ce-1508">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1508">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-1509">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-1509">Role</span></span>

* <span data-ttu-id="be8ce-1510">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1510">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="be8ce-1511">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="be8ce-1511">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="be8ce-1512">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1512">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1513">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1513">SQL</span></span>

* <span data-ttu-id="be8ce-1514">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1514">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="be8ce-1515">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1515">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1516">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1516">VM</span></span>

* <span data-ttu-id="be8ce-1517">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1517">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="be8ce-1518">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1518">November 14, 2017</span></span>

<span data-ttu-id="be8ce-1519">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="be8ce-1519">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-1520">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-1520">ACR</span></span>

* <span data-ttu-id="be8ce-1521">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="be8ce-1521">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="be8ce-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1522">ACS</span></span>

* <span data-ttu-id="be8ce-1523">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1523">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="be8ce-1524">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1524">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="be8ce-1525">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1525">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="be8ce-1526">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="be8ce-1526">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="be8ce-1527">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="be8ce-1527">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1528">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1528">Appservice</span></span>

* <span data-ttu-id="be8ce-1529">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="be8ce-1529">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="be8ce-1530">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1530">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="be8ce-1531">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1531">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="be8ce-1532">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1532">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="be8ce-1533">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="be8ce-1533">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="be8ce-1534">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="be8ce-1534">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-1535">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1535">Batch</span></span>

* <span data-ttu-id="be8ce-1536">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1536">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="be8ce-1537">Batchai</span><span class="sxs-lookup"><span data-stu-id="be8ce-1537">Batchai</span></span>

* <span data-ttu-id="be8ce-1538">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1538">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="be8ce-1539">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1539">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="be8ce-1540">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1540">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="be8ce-1541">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1541">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="be8ce-1542">Nube</span><span class="sxs-lookup"><span data-stu-id="be8ce-1542">Cloud</span></span>

* <span data-ttu-id="be8ce-1543">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="be8ce-1543">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1544">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1544">Container</span></span>

* <span data-ttu-id="be8ce-1545">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1545">Added support to open multiple ports</span></span>
* <span data-ttu-id="be8ce-1546">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="be8ce-1546">Added container group restart policy</span></span>
* <span data-ttu-id="be8ce-1547">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="be8ce-1547">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="be8ce-1548">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="be8ce-1548">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="be8ce-1549">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="be8ce-1549">Data Lake Analytics</span></span>

* <span data-ttu-id="be8ce-1550">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="be8ce-1550">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="be8ce-1551">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="be8ce-1551">Data Lake Store</span></span>

* <span data-ttu-id="be8ce-1552">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="be8ce-1552">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-1553">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1553">Extension</span></span>

* <span data-ttu-id="be8ce-1554">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="be8ce-1554">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="be8ce-1555">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="be8ce-1555">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-1556">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-1556">IoT</span></span>

* <span data-ttu-id="be8ce-1557">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="be8ce-1557">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1558">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1558">Monitor</span></span>

* <span data-ttu-id="be8ce-1559">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1559">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1560">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1560">Network</span></span>

* <span data-ttu-id="be8ce-1561">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="be8ce-1561">Added support for CAA DNS records</span></span>
* <span data-ttu-id="be8ce-1562">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1562">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="be8ce-1563">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1563">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="be8ce-1564">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1564">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="be8ce-1565">Reservations</span><span class="sxs-lookup"><span data-stu-id="be8ce-1565">Reservations</span></span>

* <span data-ttu-id="be8ce-1566">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="be8ce-1566">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1567">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1567">Resource</span></span>

* <span data-ttu-id="be8ce-1568">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1568">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1569">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1569">SQL</span></span>

* <span data-ttu-id="be8ce-1570">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1570">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1571">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1571">Storage</span></span>

* <span data-ttu-id="be8ce-1572">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="be8ce-1572">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="be8ce-1573">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="be8ce-1573">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="be8ce-1574">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1574">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="be8ce-1575">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1575">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="be8ce-1576">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1576">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="be8ce-1577">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1577">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="be8ce-1578">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1578">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1579">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1579">VM</span></span>

* <span data-ttu-id="be8ce-1580">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1580">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="be8ce-1581">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="be8ce-1581">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="be8ce-1582">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="be8ce-1582">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="be8ce-1583">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1583">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="be8ce-1584">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1584">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="be8ce-1585">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1585">October 24, 2017</span></span>

<span data-ttu-id="be8ce-1586">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="be8ce-1586">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1587">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1587">Core</span></span>

* <span data-ttu-id="be8ce-1588">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1588">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-1589">ACR</span></span>

* <span data-ttu-id="be8ce-1590">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="be8ce-1590">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="be8ce-1591">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="be8ce-1591">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="be8ce-1592">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="be8ce-1592">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1593">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1593">ACS</span></span>

* <span data-ttu-id="be8ce-1594">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1594">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="be8ce-1595">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="be8ce-1595">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1596">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1596">Appservice</span></span>

* <span data-ttu-id="be8ce-1597">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1597">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="be8ce-1598">Componente</span><span class="sxs-lookup"><span data-stu-id="be8ce-1598">Component</span></span>

* <span data-ttu-id="be8ce-1599">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="be8ce-1599">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1600">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1600">Monitor</span></span>

* <span data-ttu-id="be8ce-1601">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1601">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1602">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1602">Resource</span></span>

* <span data-ttu-id="be8ce-1603">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1603">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="be8ce-1604">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1604">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1605">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1605">VM</span></span>

* <span data-ttu-id="be8ce-1606">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1606">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="be8ce-1607">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1607">October 9, 2017</span></span>

<span data-ttu-id="be8ce-1608">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="be8ce-1608">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1609">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1609">Core</span></span>

* <span data-ttu-id="be8ce-1610">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="be8ce-1610">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1611">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1611">Appservice</span></span>

* <span data-ttu-id="be8ce-1612">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1612">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-1613">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1613">Batch</span></span>

* <span data-ttu-id="be8ce-1614">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="be8ce-1614">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="be8ce-1615">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="be8ce-1615">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="be8ce-1616">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1616">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="be8ce-1617">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="be8ce-1617">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="be8ce-1618">Batchai</span><span class="sxs-lookup"><span data-stu-id="be8ce-1618">Batchai</span></span>

* <span data-ttu-id="be8ce-1619">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1619">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-1620">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be8ce-1620">Keyvault</span></span>

* <span data-ttu-id="be8ce-1621">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1621">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="be8ce-1622">(#4448)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1622">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="be8ce-1623">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1623">Network</span></span>

* <span data-ttu-id="be8ce-1624">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1624">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="be8ce-1625">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="be8ce-1625">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1626">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1626">Resource</span></span>

* <span data-ttu-id="be8ce-1627">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1627">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="be8ce-1628">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="be8ce-1628">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="be8ce-1629">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1629">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="be8ce-1630">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1630">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1631">Sql</span><span class="sxs-lookup"><span data-stu-id="be8ce-1631">Sql</span></span>

* <span data-ttu-id="be8ce-1632">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="be8ce-1632">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="be8ce-1633">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1633">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="be8ce-1634">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1634">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1635">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1635">Storage</span></span>

* <span data-ttu-id="be8ce-1636">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="be8ce-1636">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1637">Vm</span><span class="sxs-lookup"><span data-stu-id="be8ce-1637">Vm</span></span>

* <span data-ttu-id="be8ce-1638">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="be8ce-1638">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="be8ce-1639">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1639">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="be8ce-1640">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1640">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="be8ce-1641">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1641">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="be8ce-1642">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1642">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="be8ce-1643">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1643">September 22, 2017</span></span>

<span data-ttu-id="be8ce-1644">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="be8ce-1644">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1645">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1645">Resource</span></span>

* <span data-ttu-id="be8ce-1646">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="be8ce-1646">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="be8ce-1647">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="be8ce-1647">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="be8ce-1648">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1648">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="be8ce-1649">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1649">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1650">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1650">Network</span></span>

* <span data-ttu-id="be8ce-1651">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1651">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="be8ce-1652">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1652">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="be8ce-1653">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1653">Added `asg` application security group commands</span></span>
* <span data-ttu-id="be8ce-1654">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1654">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="be8ce-1655">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1655">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="be8ce-1656">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1656">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="be8ce-1657">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1657">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1658">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1658">Storage</span></span>

* <span data-ttu-id="be8ce-1659">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="be8ce-1659">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="be8ce-1660">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="be8ce-1660">Eventgrid</span></span>

* <span data-ttu-id="be8ce-1661">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="be8ce-1661">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1662">SQL</span></span>

* <span data-ttu-id="be8ce-1663">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1663">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="be8ce-1664">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="be8ce-1664">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="be8ce-1665">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1665">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-1666">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be8ce-1666">Keyvault</span></span>

* <span data-ttu-id="be8ce-1667">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="be8ce-1667">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1668">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1668">VM</span></span>

* <span data-ttu-id="be8ce-1669">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1669">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="be8ce-1670">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="be8ce-1670">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="be8ce-1671">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1671">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="be8ce-1672">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1672">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="be8ce-1673">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1673">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="be8ce-1674">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1674">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1675">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1675">ACS</span></span>

* <span data-ttu-id="be8ce-1676">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1676">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1677">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1677">Appservice</span></span>

* <span data-ttu-id="be8ce-1678">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1678">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="be8ce-1679">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="be8ce-1679">Backup</span></span>

* <span data-ttu-id="be8ce-1680">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1680">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="be8ce-1681">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1681">September 11, 2017</span></span>

<span data-ttu-id="be8ce-1682">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="be8ce-1682">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="be8ce-1683">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1683">Core</span></span>

* <span data-ttu-id="be8ce-1684">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1684">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="be8ce-1685">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1685">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1686">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1686">Acs</span></span>

* <span data-ttu-id="be8ce-1687">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1687">Added `acs list-locations` command</span></span>
* <span data-ttu-id="be8ce-1688">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1688">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1689">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1689">Appservice</span></span>

* <span data-ttu-id="be8ce-1690">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1690">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="be8ce-1691">CDN</span><span class="sxs-lookup"><span data-stu-id="be8ce-1691">CDN</span></span>

* <span data-ttu-id="be8ce-1692">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1692">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="be8ce-1693">Extensión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1693">Extension</span></span>

* <span data-ttu-id="be8ce-1694">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="be8ce-1694">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-1695">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be8ce-1695">Keyvault</span></span>

* <span data-ttu-id="be8ce-1696">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1696">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1697">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1697">Network</span></span>

* <span data-ttu-id="be8ce-1698">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1698">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="be8ce-1699">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1699">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="be8ce-1700">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1700">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="be8ce-1701">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1701">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="be8ce-1702">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1702">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1703">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1703">Resource</span></span>

* <span data-ttu-id="be8ce-1704">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1704">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="be8ce-1705">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1705">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="be8ce-1706">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1706">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="be8ce-1707">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="be8ce-1707">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1708">SQL</span></span>

* <span data-ttu-id="be8ce-1709">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1709">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1710">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1710">VM</span></span>

* <span data-ttu-id="be8ce-1711">Problema corregido: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1711">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="be8ce-1712">Problema corregido: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1712">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="be8ce-1713">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1713">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="be8ce-1714">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1714">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="be8ce-1715">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1715">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="be8ce-1716">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1716">August 31, 2017</span></span>

<span data-ttu-id="be8ce-1717">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="be8ce-1717">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-1718">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be8ce-1718">Keyvault</span></span>

* <span data-ttu-id="be8ce-1719">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1719">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="be8ce-1720">Sf</span><span class="sxs-lookup"><span data-stu-id="be8ce-1720">Sf</span></span>

* <span data-ttu-id="be8ce-1721">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1721">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1722">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1722">Storage</span></span>

* <span data-ttu-id="be8ce-1723">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1723">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="be8ce-1724">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1724">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="be8ce-1725">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1725">August 28, 2017</span></span>

<span data-ttu-id="be8ce-1726">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="be8ce-1726">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="be8ce-1727">CLI</span><span class="sxs-lookup"><span data-stu-id="be8ce-1727">CLI</span></span>

* <span data-ttu-id="be8ce-1728">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1728">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1729">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1729">ACS</span></span>

* <span data-ttu-id="be8ce-1730">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1730">Corrected preview regions</span></span>
* <span data-ttu-id="be8ce-1731">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1731">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="be8ce-1732">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="be8ce-1732">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1733">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1733">Appservice</span></span>

* <span data-ttu-id="be8ce-1734">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1734">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="be8ce-1735">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1735">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="be8ce-1736">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1736">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="be8ce-1737">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1737">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="be8ce-1738">Problema corregido: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1738">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-1739">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-1739">IoT</span></span>

* <span data-ttu-id="be8ce-1740">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1740">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1741">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1741">Network</span></span>

* <span data-ttu-id="be8ce-1742">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1742">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="be8ce-1743">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1743">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="be8ce-1744">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1744">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="be8ce-1745">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1745">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="be8ce-1746">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1746">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1747">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1747">Profile</span></span>

* <span data-ttu-id="be8ce-1748">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1748">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="be8ce-1749">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="be8ce-1749">Service Fabric</span></span>

* <span data-ttu-id="be8ce-1750">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1750">Preview release</span></span>
* <span data-ttu-id="be8ce-1751">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1751">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="be8ce-1752">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1752">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="be8ce-1753">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1753">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1754">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1754">Storage</span></span>

* <span data-ttu-id="be8ce-1755">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1755">Enabled setting blob tier</span></span>
* <span data-ttu-id="be8ce-1756">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1756">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="be8ce-1757">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1757">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="be8ce-1758">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1758">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="be8ce-1759">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1759">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="be8ce-1760">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="be8ce-1760">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1761">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1761">VM</span></span>

* <span data-ttu-id="be8ce-1762">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1762">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="be8ce-1763">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1763">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="be8ce-1764">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1764">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="be8ce-1765">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1765">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="be8ce-1766">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1766">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="be8ce-1767">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1767">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="be8ce-1768">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1768">August 15, 2017</span></span>

<span data-ttu-id="be8ce-1769">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="be8ce-1769">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1770">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1770">ACS</span></span>

* <span data-ttu-id="be8ce-1771">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="be8ce-1771">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1772">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1772">Appservice</span></span>

* <span data-ttu-id="be8ce-1773">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1773">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="be8ce-1774">Event Grid</span><span class="sxs-lookup"><span data-stu-id="be8ce-1774">Event Grid</span></span>

* <span data-ttu-id="be8ce-1775">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1775">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="be8ce-1776">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1776">August 11, 2017</span></span>

<span data-ttu-id="be8ce-1777">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="be8ce-1777">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1778">ACS</span></span>

* <span data-ttu-id="be8ce-1779">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-1779">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-1780">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1780">Batch</span></span>

* <span data-ttu-id="be8ce-1781">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1781">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="be8ce-1782">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1782">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="be8ce-1783">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1783">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="be8ce-1784">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1784">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="be8ce-1785">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1785">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="be8ce-1786">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1786">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="be8ce-1787">Componente</span><span class="sxs-lookup"><span data-stu-id="be8ce-1787">Component</span></span>

* <span data-ttu-id="be8ce-1788">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1788">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="be8ce-1789">Contenedor</span><span class="sxs-lookup"><span data-stu-id="be8ce-1789">Container</span></span>

* <span data-ttu-id="be8ce-1790">`create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1790">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="be8ce-1791">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="be8ce-1791">Data Lake Store</span></span>

* <span data-ttu-id="be8ce-1792">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1792">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="be8ce-1793">Event Grid</span><span class="sxs-lookup"><span data-stu-id="be8ce-1793">Event Grid</span></span>

* <span data-ttu-id="be8ce-1794">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1794">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1795">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1795">Network</span></span>

* <span data-ttu-id="be8ce-1796">`lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1796">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="be8ce-1797">`application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1797">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="be8ce-1798">`application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1798">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="be8ce-1799">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1799">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1800">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1800">Profile</span></span>

* <span data-ttu-id="be8ce-1801">`account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1801">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1802">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1802">Storage</span></span>

* <span data-ttu-id="be8ce-1803">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1803">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1804">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1804">VM</span></span>

* <span data-ttu-id="be8ce-1805">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1805">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="be8ce-1806">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1806">Exposed `list-skus` command</span></span>
* <span data-ttu-id="be8ce-1807">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1807">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="be8ce-1808">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1808">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="be8ce-1809">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1809">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="be8ce-1810">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1810">July 28, 2017</span></span>

<span data-ttu-id="be8ce-1811">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="be8ce-1811">Version 2.0.12</span></span>

* <span data-ttu-id="be8ce-1812">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1812">Added container commands</span></span>
* <span data-ttu-id="be8ce-1813">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1813">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="be8ce-1814">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-1814">Core</span></span>

* <span data-ttu-id="be8ce-1815">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1815">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="be8ce-1816">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1816">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="be8ce-1817">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1817">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="be8ce-1818">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1818">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="be8ce-1819">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1819">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="be8ce-1820">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1820">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="be8ce-1821">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1821">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="be8ce-1822">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1822">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="be8ce-1823">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1823">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="be8ce-1824">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1824">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="be8ce-1825">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1825">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="be8ce-1826">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1826">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="be8ce-1827">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1827">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="be8ce-1828">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1828">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="be8ce-1829">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1829">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="be8ce-1830">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1830">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="be8ce-1831">ACR</span><span class="sxs-lookup"><span data-stu-id="be8ce-1831">ACR</span></span>

* <span data-ttu-id="be8ce-1832">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1832">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="be8ce-1833">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1833">Support SKU update for managed registries</span></span>
* <span data-ttu-id="be8ce-1834">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1834">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="be8ce-1835">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1835">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="be8ce-1836">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1836">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="be8ce-1837">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1837">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-1838">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1838">ACS</span></span>

* <span data-ttu-id="be8ce-1839">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1839">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-1840">Appservice</span><span class="sxs-lookup"><span data-stu-id="be8ce-1840">Appservice</span></span>

* <span data-ttu-id="be8ce-1841">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1841">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="be8ce-1842">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1842">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="be8ce-1843">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1843">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="be8ce-1844">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1844">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="be8ce-1845">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1845">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="be8ce-1846">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1846">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="be8ce-1847">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1847">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="be8ce-1848">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1848">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="be8ce-1849">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1849">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="be8ce-1850">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1850">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="be8ce-1851">Batch</span><span class="sxs-lookup"><span data-stu-id="be8ce-1851">Batch</span></span>

* <span data-ttu-id="be8ce-1852">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1852">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="be8ce-1853">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1853">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="be8ce-1854">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1854">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="be8ce-1855">CDN</span><span class="sxs-lookup"><span data-stu-id="be8ce-1855">CDN</span></span>

* <span data-ttu-id="be8ce-1856">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="be8ce-1856">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="be8ce-1857">Nube</span><span class="sxs-lookup"><span data-stu-id="be8ce-1857">Cloud</span></span>

* <span data-ttu-id="be8ce-1858">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1858">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="be8ce-1859">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1859">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="be8ce-1860">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1860">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="be8ce-1861">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1861">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="be8ce-1862">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1862">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be8ce-1863">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-1863">CosmosDB</span></span>

* <span data-ttu-id="be8ce-1864">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1864">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="be8ce-1865">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="be8ce-1865">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="be8ce-1866">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="be8ce-1866">Data Lake Analytics</span></span>

* <span data-ttu-id="be8ce-1867">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1867">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="be8ce-1868">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1868">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="be8ce-1869">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1869">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="be8ce-1870">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="be8ce-1870">Data Lake Store</span></span>

* <span data-ttu-id="be8ce-1871">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1871">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="be8ce-1872">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1872">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="be8ce-1873">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1873">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="be8ce-1874">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1874">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="be8ce-1875">Interactive</span><span class="sxs-lookup"><span data-stu-id="be8ce-1875">Interactive</span></span>

* <span data-ttu-id="be8ce-1876">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1876">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="be8ce-1877">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1877">Increased test coverage</span></span>
* <span data-ttu-id="be8ce-1878">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1878">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="be8ce-1879">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1879">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="be8ce-1880">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1880">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="be8ce-1881">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1881">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="be8ce-1882">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1882">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="be8ce-1883">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1883">Added `--progress` flag</span></span>
* <span data-ttu-id="be8ce-1884">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1884">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="be8ce-1885">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1885">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="be8ce-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="be8ce-1886">IoT</span></span>

* <span data-ttu-id="be8ce-1887">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1887">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="be8ce-1888">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="be8ce-1888">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="be8ce-1889">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="be8ce-1889">Key vault</span></span>

* <span data-ttu-id="be8ce-1890">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1890">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="be8ce-1891">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1891">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="be8ce-1892">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1892">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="be8ce-1893">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1893">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="be8ce-1894">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1894">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="be8ce-1895">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1895">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="be8ce-1896">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="be8ce-1896">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="be8ce-1897">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1897">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="be8ce-1898">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-1898">Lab</span></span>

* <span data-ttu-id="be8ce-1899">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1899">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="be8ce-1900">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1900">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-1901">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-1901">Monitor</span></span>

* <span data-ttu-id="be8ce-1902">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1902">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="be8ce-1903">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1903">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="be8ce-1904">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1904">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="be8ce-1905">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1905">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="be8ce-1906">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1906">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="be8ce-1907">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="be8ce-1907">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="be8ce-1908">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1908">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="be8ce-1909">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1909">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="be8ce-1910">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1910">`location` no longer required</span></span>
  * <span data-ttu-id="be8ce-1911">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1911">Add name and ID support for target</span></span>
  * <span data-ttu-id="be8ce-1912">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1912">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="be8ce-1913">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1913">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="be8ce-1914">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1914">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="be8ce-1915">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1915">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="be8ce-1916">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1916">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="be8ce-1917">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1917">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-1918">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-1918">Network</span></span>

* <span data-ttu-id="be8ce-1919">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1919">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="be8ce-1920">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1920">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="be8ce-1921">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1921">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="be8ce-1922">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1922">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="be8ce-1923">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1923">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="be8ce-1924">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1924">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="be8ce-1925">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1925">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="be8ce-1926">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1926">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="be8ce-1927">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1927">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="be8ce-1928">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1928">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="be8ce-1929">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1929">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="be8ce-1930">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1930">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="be8ce-1931">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1931">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="be8ce-1932">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1932">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="be8ce-1933">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1933">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="be8ce-1934">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1934">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="be8ce-1935">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1935">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="be8ce-1936">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1936">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="be8ce-1937">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1937">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="be8ce-1938">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1938">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="be8ce-1939">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1939">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="be8ce-1940">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1940">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="be8ce-1941">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1941">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="be8ce-1942">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1942">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="be8ce-1943">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1943">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="be8ce-1944">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1944">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="be8ce-1945">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1945">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-1946">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-1946">Profile</span></span>

* <span data-ttu-id="be8ce-1947">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1947">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="be8ce-1948">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1948">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="be8ce-1949">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="be8ce-1949">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="be8ce-1950">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1950">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="be8ce-1951">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1951">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="be8ce-1952">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be8ce-1952">RDBMS</span></span>

* <span data-ttu-id="be8ce-1953">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1953">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="be8ce-1954">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1954">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="be8ce-1955">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1955">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="be8ce-1956">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1956">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-1957">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-1957">Resource</span></span>

* <span data-ttu-id="be8ce-1958">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1958">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="be8ce-1959">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1959">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="be8ce-1960">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1960">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="be8ce-1961">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1961">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="be8ce-1962">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1962">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="be8ce-1963">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1963">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="be8ce-1964">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1964">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="be8ce-1965">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1965">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-1966">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-1966">Role</span></span>

* <span data-ttu-id="be8ce-1967">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1967">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="be8ce-1968">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1968">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="be8ce-1969">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1969">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="be8ce-1970">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1970">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="be8ce-1971">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1971">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="be8ce-1972">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="be8ce-1972">Service Fabric</span></span>
* <span data-ttu-id="be8ce-1973">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1973">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="be8ce-1974">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1974">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="be8ce-1975">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1975">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-1976">SQL</span></span>

* <span data-ttu-id="be8ce-1977">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1977">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="be8ce-1978">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1978">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="be8ce-1979">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1979">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-1980">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-1980">Storage</span></span>

* <span data-ttu-id="be8ce-1981">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1981">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="be8ce-1982">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1982">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="be8ce-1983">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1983">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="be8ce-1984">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1984">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="be8ce-1985">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1985">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="be8ce-1986">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1986">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-1987">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-1987">VM</span></span>

* <span data-ttu-id="be8ce-1988">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="be8ce-1988">Support configuring nsg</span></span>
* <span data-ttu-id="be8ce-1989">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1989">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="be8ce-1990">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1990">Support managed service identities</span></span>
* <span data-ttu-id="be8ce-1991">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="be8ce-1991">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="be8ce-1992">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="be8ce-1992">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="be8ce-1993">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-1993">May 10, 2017</span></span>

<span data-ttu-id="be8ce-1994">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="be8ce-1994">Version 2.0.6</span></span>

* <span data-ttu-id="be8ce-1995">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="be8ce-1995">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="be8ce-1996">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="be8ce-1996">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="be8ce-1997">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="be8ce-1997">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="be8ce-1998">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="be8ce-1998">Include Cognitive Services module</span></span>
* <span data-ttu-id="be8ce-1999">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="be8ce-1999">Include Service Fabric module</span></span>
* <span data-ttu-id="be8ce-2000">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="be8ce-2000">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="be8ce-2001">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="be8ce-2001">Add support for CDN commands</span></span>
* <span data-ttu-id="be8ce-2002">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="be8ce-2002">Remove Container module</span></span>
* <span data-ttu-id="be8ce-2003">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="be8ce-2003">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="be8ce-2004">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="be8ce-2004">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="be8ce-2005">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-2005">Core</span></span>

* <span data-ttu-id="be8ce-2006">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="be8ce-2006">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="be8ce-2007">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2007">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="be8ce-2008">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2008">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="be8ce-2009">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2009">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="be8ce-2010">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2010">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="be8ce-2011">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2011">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="be8ce-2012">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2012">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="be8ce-2013">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2013">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="be8ce-2014">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2014">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="be8ce-2015">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2015">core: Improved performance</span></span>
* <span data-ttu-id="be8ce-2016">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="be8ce-2016">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="be8ce-2017">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="be8ce-2017">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-2018">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-2018">ACS</span></span>

* <span data-ttu-id="be8ce-2019">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="be8ce-2019">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="be8ce-2020">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="be8ce-2020">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="be8ce-2021">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="be8ce-2021">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="be8ce-2022">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2022">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-2023">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-2023">AppService</span></span>

* <span data-ttu-id="be8ce-2024">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2024">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="be8ce-2025">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="be8ce-2025">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="be8ce-2026">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="be8ce-2026">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="be8ce-2027">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="be8ce-2027">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="be8ce-2028">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="be8ce-2028">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="be8ce-2029">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2029">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="be8ce-2030">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="be8ce-2030">support slot swap with preview</span></span>
* <span data-ttu-id="be8ce-2031">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2031">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="be8ce-2032">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2032">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be8ce-2033">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-2033">CosmosDB</span></span>

* <span data-ttu-id="be8ce-2034">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-2034">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="be8ce-2035">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="be8ce-2035">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="be8ce-2036">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="be8ce-2036">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="be8ce-2037">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="be8ce-2037">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="be8ce-2038">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="be8ce-2038">Data Lake Analytics</span></span>

* <span data-ttu-id="be8ce-2039">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="be8ce-2039">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="be8ce-2040">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="be8ce-2040">Add support for new catalog item type: package.</span></span> <span data-ttu-id="be8ce-2041">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2041">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="be8ce-2042">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="be8ce-2042">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="be8ce-2043">Tabla</span><span class="sxs-lookup"><span data-stu-id="be8ce-2043">Table</span></span>
  * <span data-ttu-id="be8ce-2044">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="be8ce-2044">Table valued function</span></span>
  * <span data-ttu-id="be8ce-2045">Ver</span><span class="sxs-lookup"><span data-stu-id="be8ce-2045">View</span></span>
  * <span data-ttu-id="be8ce-2046">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2046">Table Statistics.</span></span> <span data-ttu-id="be8ce-2047">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="be8ce-2047">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="be8ce-2048">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="be8ce-2048">Data Lake Store</span></span>

* <span data-ttu-id="be8ce-2049">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="be8ce-2049">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="be8ce-2050">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="be8ce-2050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="be8ce-2051">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2051">missed help for access show.</span></span> <span data-ttu-id="be8ce-2052">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2052">adding it.</span></span> <span data-ttu-id="be8ce-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="be8ce-2054">Buscar</span><span class="sxs-lookup"><span data-stu-id="be8ce-2054">Find</span></span>

* <span data-ttu-id="be8ce-2055">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="be8ce-2055">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="be8ce-2056">KeyVault</span><span class="sxs-lookup"><span data-stu-id="be8ce-2056">KeyVault</span></span>

* <span data-ttu-id="be8ce-2057">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="be8ce-2057">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="be8ce-2058">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="be8ce-2058">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="be8ce-2059">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="be8ce-2059">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="be8ce-2060">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="be8ce-2060">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="be8ce-2061">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2061">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="be8ce-2062">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-2062">Lab</span></span>

* <span data-ttu-id="be8ce-2063">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-2063">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="be8ce-2064">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-2064">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="be8ce-2065">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-2065">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="be8ce-2066">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-2066">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="be8ce-2067">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="be8ce-2067">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="be8ce-2068">Supervisión</span><span class="sxs-lookup"><span data-stu-id="be8ce-2068">Monitor</span></span>

* <span data-ttu-id="be8ce-2069">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2069">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="be8ce-2070">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2070">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="be8ce-2071">Red</span><span class="sxs-lookup"><span data-stu-id="be8ce-2071">Network</span></span>

* <span data-ttu-id="be8ce-2072">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2072">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="be8ce-2073">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2073">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="be8ce-2074">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="be8ce-2074">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="be8ce-2075">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="be8ce-2075">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="be8ce-2076">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="be8ce-2076">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="be8ce-2077">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="be8ce-2077">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="be8ce-2078">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="be8ce-2078">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="be8ce-2079">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="be8ce-2079">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="be8ce-2080">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2080">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="be8ce-2081">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="be8ce-2081">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="be8ce-2082">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2082">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="be8ce-2083">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2083">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="be8ce-2084">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="be8ce-2084">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="be8ce-2085">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="be8ce-2085">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="be8ce-2086">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="be8ce-2086">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="be8ce-2087">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="be8ce-2087">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="be8ce-2088">Perfil</span><span class="sxs-lookup"><span data-stu-id="be8ce-2088">Profile</span></span>

* <span data-ttu-id="be8ce-2089">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2089">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="be8ce-2090">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2090">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="be8ce-2091">Redis</span><span class="sxs-lookup"><span data-stu-id="be8ce-2091">Redis</span></span>

* <span data-ttu-id="be8ce-2092">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="be8ce-2092">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="be8ce-2093">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="be8ce-2093">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="be8ce-2094">Recurso</span><span class="sxs-lookup"><span data-stu-id="be8ce-2094">Resource</span></span>

* <span data-ttu-id="be8ce-2095">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2095">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="be8ce-2096">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2096">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="be8ce-2097">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2097">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="be8ce-2098">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="be8ce-2098">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="be8ce-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="be8ce-2100">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="be8ce-2100">Add docs for az lock update.</span></span> <span data-ttu-id="be8ce-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="be8ce-2102">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="be8ce-2102">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="be8ce-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="be8ce-2104">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="be8ce-2104">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="be8ce-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="be8ce-2106">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2106">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="be8ce-2107">Rol</span><span class="sxs-lookup"><span data-stu-id="be8ce-2107">Role</span></span>

* <span data-ttu-id="be8ce-2108">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2108">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="be8ce-2109">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2109">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="be8ce-2110">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2110">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="be8ce-2111">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="be8ce-2111">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="be8ce-2112">SQL</span><span class="sxs-lookup"><span data-stu-id="be8ce-2112">SQL</span></span>

* <span data-ttu-id="be8ce-2113">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="be8ce-2113">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="be8ce-2114">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2114">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="be8ce-2115">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-2115">Storage</span></span>

* <span data-ttu-id="be8ce-2116">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2116">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="be8ce-2117">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="be8ce-2117">Add support for incremental blob copy</span></span>
* <span data-ttu-id="be8ce-2118">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="be8ce-2118">Add support for large block blob upload</span></span>
* <span data-ttu-id="be8ce-2119">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="be8ce-2119">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-2120">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-2120">VM</span></span>

* <span data-ttu-id="be8ce-2121">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="be8ce-2121">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="be8ce-2122">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="be8ce-2122">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="be8ce-2123">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="be8ce-2123">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="be8ce-2124">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="be8ce-2124">az vm/vmss disk</span></span>
  3. <span data-ttu-id="be8ce-2125">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="be8ce-2125">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="be8ce-2126">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="be8ce-2126">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="be8ce-2127">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2127">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="be8ce-2128">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-2128">April 3, 2017</span></span>

<span data-ttu-id="be8ce-2129">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="be8ce-2129">Version 2.0.2</span></span>

<span data-ttu-id="be8ce-2130">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="be8ce-2130">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="be8ce-2131">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be8ce-2131">Core</span></span>

* <span data-ttu-id="be8ce-2132">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="be8ce-2132">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="be8ce-2133">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2133">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="be8ce-2134">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2134">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="be8ce-2135">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2135">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="be8ce-2136">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2136">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="be8ce-2137">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2137">Add prompting for missing template parameters.</span></span> <span data-ttu-id="be8ce-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="be8ce-2139">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="be8ce-2139">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="be8ce-2140">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="be8ce-2140">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="be8ce-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="be8ce-2141">ACS</span></span>

* <span data-ttu-id="be8ce-2142">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2142">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="be8ce-2143">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2143">Add support for ssh key password prompting.</span></span> <span data-ttu-id="be8ce-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="be8ce-2145">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2145">Add support for windows clusters.</span></span> <span data-ttu-id="be8ce-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="be8ce-2147">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="be8ce-2147">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="be8ce-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="be8ce-2149">AppService</span><span class="sxs-lookup"><span data-stu-id="be8ce-2149">AppService</span></span>

* <span data-ttu-id="be8ce-2150">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2150">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="be8ce-2151">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2151">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="be8ce-2152">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2152">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="be8ce-2153">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2153">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="be8ce-2154">DataLake</span><span class="sxs-lookup"><span data-stu-id="be8ce-2154">DataLake</span></span>

* <span data-ttu-id="be8ce-2155">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="be8ce-2155">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="be8ce-2156">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="be8ce-2156">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="be8ce-2157">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="be8ce-2157">DocuemntDB</span></span>

* <span data-ttu-id="be8ce-2158">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2158">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="be8ce-2159">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be8ce-2159">VM</span></span>

* <span data-ttu-id="be8ce-2160">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2160">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="be8ce-2161">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2161">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="be8ce-2162">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2162">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="be8ce-2163">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2163">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="be8ce-2164">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2164">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="be8ce-2165">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2165">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="be8ce-2166">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="be8ce-2166">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="be8ce-2167">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="be8ce-2167">February 27, 2017</span></span>

<span data-ttu-id="be8ce-2168">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="be8ce-2168">Version 2.0.0</span></span>

<span data-ttu-id="be8ce-2169">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="be8ce-2169">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="be8ce-2170">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="be8ce-2170">Container Service (acs)</span></span>
- <span data-ttu-id="be8ce-2171">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="be8ce-2171">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="be8ce-2172">Redes</span><span class="sxs-lookup"><span data-stu-id="be8ce-2172">Networking</span></span>
- <span data-ttu-id="be8ce-2173">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="be8ce-2173">Storage</span></span>

<span data-ttu-id="be8ce-2174">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2174">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="be8ce-2175">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="be8ce-2175">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="be8ce-2176">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="be8ce-2176">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="be8ce-2177">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="be8ce-2177">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="be8ce-2178">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="be8ce-2178">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="be8ce-2179">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="be8ce-2179">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="be8ce-2180">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="be8ce-2180">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="be8ce-2181">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="be8ce-2181">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="be8ce-2182">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="be8ce-2182">Provide feedback from the command line with the `az feedback` command</span></span>

