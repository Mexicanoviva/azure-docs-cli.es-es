---
title: Notas de la versión de la CLI de Azure 2.0
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/28/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 62e57d048666f478b670f182bb9348dba90de6a0
ms.sourcegitcommit: 8f060bc009278eafc0ed448bad4b7d08c742ff63
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/29/2018
ms.locfileid: "43145097"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="91ff5-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="91ff5-103">Azure CLI 2.0 release notes</span></span>

## <a name="auguest-28-2018"></a><span data-ttu-id="91ff5-104">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-104">Auguest 28, 2018</span></span>

<span data-ttu-id="91ff5-105">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="91ff5-105">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-106">Core</span></span>

* <span data-ttu-id="91ff5-107">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="91ff5-107">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="91ff5-108">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="91ff5-108">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-109">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-109">ACR</span></span>

* <span data-ttu-id="91ff5-110">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="91ff5-110">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="91ff5-111">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="91ff5-111">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-112">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-112">ACS</span></span>

* <span data-ttu-id="91ff5-113">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="91ff5-113">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="91ff5-114">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="91ff5-114">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-115">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-115">AppService</span></span>

* <span data-ttu-id="91ff5-116">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="91ff5-116">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="91ff5-117">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-117">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="91ff5-118">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-118">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="91ff5-119">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="91ff5-119">Backup</span></span>

* <span data-ttu-id="91ff5-120">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-120">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="91ff5-121">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="91ff5-121">Bot Service</span></span>

* <span data-ttu-id="91ff5-122">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="91ff5-122">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="91ff5-123">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="91ff5-123">Cognitive Services</span></span>

* <span data-ttu-id="91ff5-124">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="91ff5-124">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="91ff5-125">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-125">IoT</span></span>

* <span data-ttu-id="91ff5-126">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="91ff5-126">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-127">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-127">Monitor</span></span>

* <span data-ttu-id="91ff5-128">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="91ff5-128">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="91ff5-129">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="91ff5-129">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-130">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-130">Network</span></span>

* <span data-ttu-id="91ff5-131">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-131">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-132">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-132">Resource</span></span>

* <span data-ttu-id="91ff5-133">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-133">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-134">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-134">Storage</span></span>

* <span data-ttu-id="91ff5-135">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-135">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-136">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-136">VM</span></span>

* <span data-ttu-id="91ff5-137">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-137">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="91ff5-138">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-138">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="91ff5-139">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-139">Auguest 14, 2018</span></span>

<span data-ttu-id="91ff5-140">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="91ff5-140">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-141">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-141">Core</span></span>

* <span data-ttu-id="91ff5-142">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="91ff5-142">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="91ff5-143">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="91ff5-143">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="91ff5-144">Telemetría</span><span class="sxs-lookup"><span data-stu-id="91ff5-144">Telemetry</span></span>

* <span data-ttu-id="91ff5-145">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="91ff5-145">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-146">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-146">ACR</span></span>

* <span data-ttu-id="91ff5-147">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-147">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="91ff5-148">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="91ff5-148">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-149">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-149">ACS</span></span>

* <span data-ttu-id="91ff5-150">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="91ff5-150">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="91ff5-151">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="91ff5-151">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="91ff5-152">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="91ff5-152">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="91ff5-153">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="91ff5-153">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="91ff5-154">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="91ff5-154">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="91ff5-155">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-155">AppService</span></span>

* <span data-ttu-id="91ff5-156">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="91ff5-156">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="91ff5-157">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="91ff5-157">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="91ff5-158">BatchAI</span><span class="sxs-lookup"><span data-stu-id="91ff5-158">BatchAI</span></span>

* <span data-ttu-id="91ff5-159">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="91ff5-159">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="91ff5-160">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-160">Container</span></span>

* <span data-ttu-id="91ff5-161">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-161">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="91ff5-162">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-162">IoT</span></span>

* <span data-ttu-id="91ff5-163">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="91ff5-163">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="91ff5-164">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="91ff5-164">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="91ff5-165">Iot Central</span><span class="sxs-lookup"><span data-stu-id="91ff5-165">Iot Central</span></span>

* <span data-ttu-id="91ff5-166">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="91ff5-166">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="91ff5-167">KeyVault</span><span class="sxs-lookup"><span data-stu-id="91ff5-167">KeyVault</span></span>


* <span data-ttu-id="91ff5-168">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="91ff5-168">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="91ff5-169">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="91ff5-169">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="91ff5-170">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="91ff5-170">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="91ff5-171">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="91ff5-171">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="91ff5-172">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="91ff5-172">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="91ff5-173">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-173">Relay</span></span>

* <span data-ttu-id="91ff5-174">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="91ff5-174">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-175">Sql</span><span class="sxs-lookup"><span data-stu-id="91ff5-175">Sql</span></span>

* <span data-ttu-id="91ff5-176">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-176">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-177">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-177">Storage</span></span>

* <span data-ttu-id="91ff5-178">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="91ff5-178">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="91ff5-179">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="91ff5-179">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="91ff5-180">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="91ff5-180">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="91ff5-181">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="91ff5-181">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="91ff5-182">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-182">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-183">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-183">VM</span></span>

* <span data-ttu-id="91ff5-184">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="91ff5-184">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="91ff5-185">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-185">July 31, 2018</span></span>

<span data-ttu-id="91ff5-186">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="91ff5-186">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-187">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-187">ACR</span></span>

* <span data-ttu-id="91ff5-188">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-188">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="91ff5-189">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-189">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-190">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-190">ACS</span></span>

* <span data-ttu-id="91ff5-191">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="91ff5-191">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-192">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-192">Batch</span></span>

* <span data-ttu-id="91ff5-193">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="91ff5-193">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-194">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-194">Container</span></span>

* <span data-ttu-id="91ff5-195">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="91ff5-195">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-196">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-196">Network</span></span>

* <span data-ttu-id="91ff5-197">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="91ff5-197">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="91ff5-198">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-198">Resource</span></span>

* <span data-ttu-id="91ff5-199">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="91ff5-199">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="91ff5-200">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="91ff5-200">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-201">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-201">Role</span></span>

* <span data-ttu-id="91ff5-202">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="91ff5-202">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="91ff5-203">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="91ff5-203">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="91ff5-204">Search</span><span class="sxs-lookup"><span data-stu-id="91ff5-204">Search</span></span>

* <span data-ttu-id="91ff5-205">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="91ff5-205">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="91ff5-206">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="91ff5-206">Service Bus</span></span>

* <span data-ttu-id="91ff5-207">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="91ff5-207">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="91ff5-208">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="91ff5-208">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="91ff5-209">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="91ff5-209">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="91ff5-210">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="91ff5-210">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-211">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-211">Storage</span></span>

* <span data-ttu-id="91ff5-212">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="91ff5-212">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="91ff5-213">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-213">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-214">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-214">VM</span></span>

* <span data-ttu-id="91ff5-215">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="91ff5-215">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="91ff5-216">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="91ff5-216">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="91ff5-217">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="91ff5-217">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="91ff5-218">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="91ff5-218">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="91ff5-219">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-219">July 18, 2018</span></span>

<span data-ttu-id="91ff5-220">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="91ff5-220">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-221">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-221">Core</span></span>

* <span data-ttu-id="91ff5-222">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="91ff5-222">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="91ff5-223">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="91ff5-223">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="91ff5-224">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-224">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-225">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-225">ACR</span></span>

* <span data-ttu-id="91ff5-226">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="91ff5-226">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="91ff5-227">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="91ff5-227">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="91ff5-228">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="91ff5-228">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="91ff5-229">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="91ff5-229">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-230">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-230">ACS</span></span>

* <span data-ttu-id="91ff5-231">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="91ff5-231">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-232">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-232">AppService</span></span>

* <span data-ttu-id="91ff5-233">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="91ff5-233">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-234">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-234">Batch</span></span>

* <span data-ttu-id="91ff5-235">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="91ff5-235">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="91ff5-236">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="91ff5-236">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="91ff5-237">Batch AI</span><span class="sxs-lookup"><span data-stu-id="91ff5-237">Batch AI</span></span>

* <span data-ttu-id="91ff5-238">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="91ff5-238">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-239">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-239">Container</span></span>

* <span data-ttu-id="91ff5-240">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="91ff5-240">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="91ff5-241">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="91ff5-241">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-242">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-242">Network</span></span>

* <span data-ttu-id="91ff5-243">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-243">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="91ff5-244">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-244">Added `network nic wait`</span></span>
* <span data-ttu-id="91ff5-245">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="91ff5-245">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="91ff5-246">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="91ff5-246">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="91ff5-247">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-247">Resource</span></span>

* <span data-ttu-id="91ff5-248">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="91ff5-248">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="91ff5-249">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="91ff5-249">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="91ff5-250">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-250">Added `deployment wait` command</span></span>
* <span data-ttu-id="91ff5-251">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="91ff5-251">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-252">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-252">SQL</span></span>

* <span data-ttu-id="91ff5-253">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-253">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="91ff5-254">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="91ff5-254">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="91ff5-255">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="91ff5-255">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-256">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-256">Storage</span></span>

* <span data-ttu-id="91ff5-257">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="91ff5-257">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-258">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-258">VM</span></span>

* <span data-ttu-id="91ff5-259">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="91ff5-259">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="91ff5-260">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-260">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="91ff5-261">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-261">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="91ff5-262">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-262">July 3, 2018</span></span>

<span data-ttu-id="91ff5-263">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="91ff5-263">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="91ff5-264">AKS</span><span class="sxs-lookup"><span data-stu-id="91ff5-264">AKS</span></span>

* <span data-ttu-id="91ff5-265">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="91ff5-265">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="91ff5-266">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-266">July 3, 2018</span></span>

<span data-ttu-id="91ff5-267">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="91ff5-267">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-268">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-268">Core</span></span>

* <span data-ttu-id="91ff5-269">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="91ff5-269">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-270">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-270">ACR</span></span>

* <span data-ttu-id="91ff5-271">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="91ff5-271">Added polling build status</span></span>
* <span data-ttu-id="91ff5-272">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="91ff5-272">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="91ff5-273">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="91ff5-273">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-274">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-274">ACS</span></span>

* <span data-ttu-id="91ff5-275">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="91ff5-275">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="91ff5-276">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="91ff5-276">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="91ff5-277">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-277">Updated options for `aks browse` command.</span></span> <span data-ttu-id="91ff5-278">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="91ff5-278">Added `--listen-port` support</span></span>
* <span data-ttu-id="91ff5-279">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-279">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="91ff5-280">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="91ff5-280">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="91ff5-281">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="91ff5-281">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-282">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-282">AppService</span></span>

* <span data-ttu-id="91ff5-283">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="91ff5-283">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="91ff5-284">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="91ff5-284">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="91ff5-285">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="91ff5-285">Backup</span></span>

* <span data-ttu-id="91ff5-286">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="91ff5-286">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="91ff5-287">BatchAI</span><span class="sxs-lookup"><span data-stu-id="91ff5-287">BatchAI</span></span>

* <span data-ttu-id="91ff5-288">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="91ff5-288">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="91ff5-289">Nube</span><span class="sxs-lookup"><span data-stu-id="91ff5-289">Cloud</span></span>

* <span data-ttu-id="91ff5-290">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="91ff5-290">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-291">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-291">Container</span></span>

* <span data-ttu-id="91ff5-292">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="91ff5-292">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="91ff5-293">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="91ff5-293">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="91ff5-294">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="91ff5-294">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-295">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-295">Extension</span></span>

* <span data-ttu-id="91ff5-296">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="91ff5-296">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-297">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-297">Network</span></span>

* <span data-ttu-id="91ff5-298">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="91ff5-298">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="91ff5-299">Rdbms</span><span class="sxs-lookup"><span data-stu-id="91ff5-299">Rdbms</span></span>

* <span data-ttu-id="91ff5-300">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-300">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-301">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-301">Resource</span></span>

* <span data-ttu-id="91ff5-302">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="91ff5-302">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-303">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-303">VM</span></span>

* <span data-ttu-id="91ff5-304">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="91ff5-304">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="91ff5-305">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-305">June 25, 2018</span></span>

<span data-ttu-id="91ff5-306">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="91ff5-306">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="91ff5-307">CLI</span><span class="sxs-lookup"><span data-stu-id="91ff5-307">CLI</span></span>

* <span data-ttu-id="91ff5-308">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-308">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="91ff5-309">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-309">June 19, 2018</span></span>

<span data-ttu-id="91ff5-310">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="91ff5-310">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-311">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-311">Core</span></span>

* <span data-ttu-id="91ff5-312">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-312">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-313">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-313">ACR</span></span>

* <span data-ttu-id="91ff5-314">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="91ff5-314">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="91ff5-315">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="91ff5-315">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-316">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-316">ACS</span></span>

* <span data-ttu-id="91ff5-317">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-317">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="91ff5-318">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-318">Added `--update` support</span></span>
* <span data-ttu-id="91ff5-319">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="91ff5-319">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="91ff5-320">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="91ff5-320">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="91ff5-321">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="91ff5-321">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="91ff5-322">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="91ff5-322">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="91ff5-323">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="91ff5-323">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="91ff5-324">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="91ff5-324">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-325">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-325">AppService</span></span>

* <span data-ttu-id="91ff5-326">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="91ff5-326">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="91ff5-327">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="91ff5-327">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-328">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-328">Batch</span></span>

* <span data-ttu-id="91ff5-329">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="91ff5-329">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="91ff5-330">Batch AI</span><span class="sxs-lookup"><span data-stu-id="91ff5-330">Batch AI</span></span>

* <span data-ttu-id="91ff5-331">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="91ff5-331">Added support for workspaces.</span></span> <span data-ttu-id="91ff5-332">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="91ff5-332">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="91ff5-333">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-333">Added support for experiments.</span></span> <span data-ttu-id="91ff5-334">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="91ff5-334">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="91ff5-335">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="91ff5-335">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="91ff5-336">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-336">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="91ff5-337">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-337">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="91ff5-338">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-338">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="91ff5-339">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="91ff5-339">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="91ff5-340">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-340">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="91ff5-341">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-341">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="91ff5-342">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-342">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="91ff5-343">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-343">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="91ff5-344">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-344">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="91ff5-345">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-345">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="91ff5-346">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="91ff5-346">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="91ff5-347">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-347">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="91ff5-348">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="91ff5-348">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="91ff5-349">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="91ff5-349">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="91ff5-350">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="91ff5-350">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="91ff5-351">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="91ff5-351">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="91ff5-352">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="91ff5-352">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="91ff5-353">Mapas</span><span class="sxs-lookup"><span data-stu-id="91ff5-353">Maps</span></span>

* <span data-ttu-id="91ff5-354">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-354">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-355">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-355">Network</span></span>

* <span data-ttu-id="91ff5-356">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="91ff5-356">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="91ff5-357">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-357">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="91ff5-358">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="91ff5-358">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="91ff5-359">Reservations</span><span class="sxs-lookup"><span data-stu-id="91ff5-359">Reservations</span></span>

* <span data-ttu-id="91ff5-360">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-360">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="91ff5-361">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-361">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="91ff5-362">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-362">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="91ff5-363">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-363">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="91ff5-364">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-364">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="91ff5-365">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-365">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-366">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-366">Role</span></span>

* <span data-ttu-id="91ff5-367">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="91ff5-367">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-368">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-368">SQL</span></span>

* <span data-ttu-id="91ff5-369">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="91ff5-369">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-370">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-370">Storage</span></span>

* <span data-ttu-id="91ff5-371">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="91ff5-371">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-372">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-372">VM</span></span>

* <span data-ttu-id="91ff5-373">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-373">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="91ff5-374">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="91ff5-374">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="91ff5-375">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="91ff5-375">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="91ff5-376">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-376">June 13, 2018</span></span>

<span data-ttu-id="91ff5-377">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="91ff5-377">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-378">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-378">Core</span></span>

* <span data-ttu-id="91ff5-379">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="91ff5-379">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="91ff5-380">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-380">June 13, 2018</span></span>

<span data-ttu-id="91ff5-381">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="91ff5-381">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="91ff5-382">AKS</span><span class="sxs-lookup"><span data-stu-id="91ff5-382">AKS</span></span>

* <span data-ttu-id="91ff5-383">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-383">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="91ff5-384">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="91ff5-384">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="91ff5-385">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-385">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="91ff5-386">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-386">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="91ff5-387">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-387">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-388">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-388">AppService</span></span>

* <span data-ttu-id="91ff5-389">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="91ff5-389">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="91ff5-390">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-390">June 5, 2018</span></span>

<span data-ttu-id="91ff5-391">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="91ff5-391">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-392">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-392">Interactive</span></span>

* <span data-ttu-id="91ff5-393">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="91ff5-393">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="91ff5-394">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-394">June 5, 2018</span></span>

<span data-ttu-id="91ff5-395">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="91ff5-395">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-396">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-396">Core</span></span>

* <span data-ttu-id="91ff5-397">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="91ff5-397">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="91ff5-398">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="91ff5-398">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-399">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-399">ACR</span></span>

* <span data-ttu-id="91ff5-400">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="91ff5-400">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="91ff5-401">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-401">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="91ff5-402">AKS</span><span class="sxs-lookup"><span data-stu-id="91ff5-402">AKS</span></span>

* <span data-ttu-id="91ff5-403">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="91ff5-403">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-404">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-404">Batch</span></span>

* <span data-ttu-id="91ff5-405">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="91ff5-405">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="91ff5-406">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-406">IOT</span></span>

* <span data-ttu-id="91ff5-407">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="91ff5-407">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-408">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-408">Network</span></span>

* <span data-ttu-id="91ff5-409">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="91ff5-409">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="91ff5-410">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="91ff5-410">Policy Insights</span></span>

* <span data-ttu-id="91ff5-411">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="91ff5-411">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="91ff5-412">ARM</span><span class="sxs-lookup"><span data-stu-id="91ff5-412">ARM</span></span>

* <span data-ttu-id="91ff5-413">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-413">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-414">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-414">SQL</span></span>

* <span data-ttu-id="91ff5-415">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="91ff5-415">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="91ff5-416">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="91ff5-416">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="91ff5-417">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-417">Storage</span></span>

* <span data-ttu-id="91ff5-418">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="91ff5-418">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-419">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-419">VM</span></span>

* <span data-ttu-id="91ff5-420">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="91ff5-420">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="91ff5-421">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-421">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="91ff5-422">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-422">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="91ff5-423">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-423">May 22, 2018</span></span>

<span data-ttu-id="91ff5-424">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="91ff5-424">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-425">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-425">Core</span></span>

* <span data-ttu-id="91ff5-426">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="91ff5-426">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-427">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-427">ACS</span></span>

* <span data-ttu-id="91ff5-428">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="91ff5-428">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="91ff5-429">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="91ff5-429">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-430">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-430">AppService</span></span>

* <span data-ttu-id="91ff5-431">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="91ff5-431">Improved generic update commands</span></span>
* <span data-ttu-id="91ff5-432">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="91ff5-432">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-433">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-433">Container</span></span>

* <span data-ttu-id="91ff5-434">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="91ff5-434">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="91ff5-435">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="91ff5-435">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-436">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-436">Extension</span></span>

* <span data-ttu-id="91ff5-437">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="91ff5-437">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-438">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-438">Interactive</span></span>

* <span data-ttu-id="91ff5-439">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="91ff5-439">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="91ff5-440">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="91ff5-440">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="91ff5-441">KeyVault</span><span class="sxs-lookup"><span data-stu-id="91ff5-441">KeyVault</span></span>

* <span data-ttu-id="91ff5-442">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="91ff5-442">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-443">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-443">Network</span></span>

* <span data-ttu-id="91ff5-444">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="91ff5-444">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="91ff5-445">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="91ff5-445">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-446">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-446">SQL</span></span>

* <span data-ttu-id="91ff5-447">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="91ff5-447">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="91ff5-448">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="91ff5-448">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="91ff5-449">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="91ff5-449">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="91ff5-450">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="91ff5-450">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="91ff5-451">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="91ff5-451">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="91ff5-452">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-452">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="91ff5-453">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="91ff5-453">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="91ff5-454">`edition`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-454">`edition`.</span></span> <span data-ttu-id="91ff5-455">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="91ff5-455">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="91ff5-456">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-456">`elasticPoolName`.</span></span> <span data-ttu-id="91ff5-457">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="91ff5-457">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="91ff5-458">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="91ff5-458">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="91ff5-459">`edition`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-459">`edition`.</span></span> <span data-ttu-id="91ff5-460">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="91ff5-460">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="91ff5-461">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-461">`dtu`.</span></span> <span data-ttu-id="91ff5-462">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="91ff5-462">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="91ff5-463">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-463">`databaseDtuMin`.</span></span> <span data-ttu-id="91ff5-464">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="91ff5-464">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="91ff5-465">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-465">`databaseDtuMax`.</span></span> <span data-ttu-id="91ff5-466">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="91ff5-466">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="91ff5-467">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-467">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="91ff5-468">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-468">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-469">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-469">Storage</span></span>

* <span data-ttu-id="91ff5-470">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="91ff5-470">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="91ff5-471">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="91ff5-471">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-472">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-472">VM</span></span>

* <span data-ttu-id="91ff5-473">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-473">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="91ff5-474">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="91ff5-474">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="91ff5-475">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="91ff5-475">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="91ff5-476">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="91ff5-476">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="91ff5-477">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-477">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="91ff5-478">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-478">May 7, 2018</span></span>

<span data-ttu-id="91ff5-479">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="91ff5-479">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-480">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-480">Core</span></span>

* <span data-ttu-id="91ff5-481">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="91ff5-481">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="91ff5-482">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="91ff5-482">Added limited support for positional arguments</span></span>
* <span data-ttu-id="91ff5-483">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-483">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="91ff5-484">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="91ff5-484">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="91ff5-485">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-485">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="91ff5-486">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="91ff5-486">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="91ff5-487">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-487">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="91ff5-488">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="91ff5-488">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="91ff5-489">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-489">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-490">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-490">ACR</span></span>

* <span data-ttu-id="91ff5-491">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="91ff5-491">Added ACR Build commands</span></span>
* <span data-ttu-id="91ff5-492">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="91ff5-492">Improved resource not found error messages</span></span>
* <span data-ttu-id="91ff5-493">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="91ff5-493">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="91ff5-494">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="91ff5-494">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="91ff5-495">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-495">Improved repository commands error messages</span></span>
* <span data-ttu-id="91ff5-496">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="91ff5-496">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-497">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-497">ACS</span></span>

* <span data-ttu-id="91ff5-498">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="91ff5-498">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="91ff5-499">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="91ff5-499">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="91ff5-500">AMS</span><span class="sxs-lookup"><span data-stu-id="91ff5-500">AMS</span></span>

* <span data-ttu-id="91ff5-501">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="91ff5-501">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-502">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-502">Appservice</span></span>

* <span data-ttu-id="91ff5-503">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="91ff5-503">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="91ff5-504">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-504">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="91ff5-505">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="91ff5-505">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="91ff5-506">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="91ff5-506">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="91ff5-507">Batch AI</span><span class="sxs-lookup"><span data-stu-id="91ff5-507">Batch AI</span></span>

* <span data-ttu-id="91ff5-508">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="91ff5-508">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="91ff5-509">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="91ff5-509">Cognitive Services</span></span>

* <span data-ttu-id="91ff5-510">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="91ff5-510">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="91ff5-511">Consumo</span><span class="sxs-lookup"><span data-stu-id="91ff5-511">Consumption</span></span>

* <span data-ttu-id="91ff5-512">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="91ff5-512">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-513">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-513">Container</span></span>

* <span data-ttu-id="91ff5-514">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="91ff5-514">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="91ff5-515">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="91ff5-515">Cosmos DB</span></span>

* <span data-ttu-id="91ff5-516">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="91ff5-516">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="91ff5-517">DMS</span><span class="sxs-lookup"><span data-stu-id="91ff5-517">DMS</span></span>

* <span data-ttu-id="91ff5-518">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-518">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-519">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-519">Extension</span></span>

* <span data-ttu-id="91ff5-520">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="91ff5-520">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-521">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-521">Interactive</span></span>

* <span data-ttu-id="91ff5-522">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="91ff5-522">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="91ff5-523">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="91ff5-523">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="91ff5-524">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="91ff5-524">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="91ff5-525">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-525">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="91ff5-526">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-526">Lab</span></span>

* <span data-ttu-id="91ff5-527">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="91ff5-527">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-528">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-528">Network</span></span>

* <span data-ttu-id="91ff5-529">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="91ff5-529">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="91ff5-530">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-530">Profile</span></span>

* <span data-ttu-id="91ff5-531">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-531">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="91ff5-532">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="91ff5-532">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="91ff5-533">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="91ff5-533">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="91ff5-534">Redis</span><span class="sxs-lookup"><span data-stu-id="91ff5-534">Redis</span></span>

* <span data-ttu-id="91ff5-535">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="91ff5-535">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="91ff5-536">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-536">Deprecated `redis list-all`.</span></span> <span data-ttu-id="91ff5-537">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="91ff5-537">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="91ff5-538">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="91ff5-538">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="91ff5-539">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-539">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-540">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-540">Role</span></span>

* <span data-ttu-id="91ff5-541">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="91ff5-541">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-542">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-542">Storage</span></span>

* <span data-ttu-id="91ff5-543">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="91ff5-543">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="91ff5-544">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="91ff5-544">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="91ff5-545">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="91ff5-545">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="91ff5-546">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="91ff5-546">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="91ff5-547">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="91ff5-547">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-548">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-548">VM</span></span>

* <span data-ttu-id="91ff5-549">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="91ff5-549">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="91ff5-550">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="91ff5-550">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="91ff5-551">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="91ff5-551">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="91ff5-552">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="91ff5-552">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="91ff5-553">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="91ff5-553">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="91ff5-554">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="91ff5-554">Added write accelerator support</span></span>
* <span data-ttu-id="91ff5-555">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-555">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="91ff5-556">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="91ff5-556">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="91ff5-557">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="91ff5-557">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="91ff5-558">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-558">April 10, 2018</span></span>

<span data-ttu-id="91ff5-559">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="91ff5-559">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-560">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-560">ACR</span></span>

* <span data-ttu-id="91ff5-561">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="91ff5-561">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-562">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-562">ACS</span></span>

* <span data-ttu-id="91ff5-563">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="91ff5-563">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-564">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-564">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="91ff5-566">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="91ff5-566">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="91ff5-567">BatchAI</span><span class="sxs-lookup"><span data-stu-id="91ff5-567">BatchAI</span></span>

* <span data-ttu-id="91ff5-568">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="91ff5-568">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="91ff5-569">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="91ff5-569">Job level mounting</span></span>
 - <span data-ttu-id="91ff5-570">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="91ff5-570">Environment variables with secret values</span></span>
 - <span data-ttu-id="91ff5-571">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="91ff5-571">Performance counters settings</span></span>
 - <span data-ttu-id="91ff5-572">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="91ff5-572">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="91ff5-573">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="91ff5-573">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="91ff5-574">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="91ff5-574">Usage and limits reporting</span></span>
 - <span data-ttu-id="91ff5-575">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="91ff5-575">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="91ff5-576">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="91ff5-576">Support for custom images</span></span>
 - <span data-ttu-id="91ff5-577">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="91ff5-577">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="91ff5-578">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="91ff5-578">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="91ff5-579">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="91ff5-579">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="91ff5-580">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="91ff5-580">National clouds are supported</span></span>
* <span data-ttu-id="91ff5-581">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="91ff5-581">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="91ff5-582">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="91ff5-582">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="91ff5-583">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="91ff5-583">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="91ff5-584">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="91ff5-584">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="91ff5-585">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="91ff5-585">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="91ff5-586">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="91ff5-586">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="91ff5-587">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-587">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="91ff5-588">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="91ff5-588">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="91ff5-589">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="91ff5-589">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="91ff5-590">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-590">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="91ff5-591">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-591">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="91ff5-592">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="91ff5-592">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="91ff5-593">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-593">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="91ff5-594">Facturación</span><span class="sxs-lookup"><span data-stu-id="91ff5-594">Billing</span></span>

* <span data-ttu-id="91ff5-595">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="91ff5-595">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="91ff5-596">Consumo</span><span class="sxs-lookup"><span data-stu-id="91ff5-596">Consumption</span></span>

* <span data-ttu-id="91ff5-597">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-597">Added `marketplace` commands</span></span>
* <span data-ttu-id="91ff5-598">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="91ff5-598">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="91ff5-599">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="91ff5-599">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="91ff5-600">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="91ff5-600">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="91ff5-601">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="91ff5-601">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="91ff5-602">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="91ff5-602">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-603">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-603">Container</span></span>

* <span data-ttu-id="91ff5-604">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="91ff5-604">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="91ff5-605">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="91ff5-605">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-606">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-606">Extension</span></span>

* <span data-ttu-id="91ff5-607">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="91ff5-607">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-608">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-608">Interactive</span></span>

* <span data-ttu-id="91ff5-609">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="91ff5-609">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="91ff5-610">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-610">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="91ff5-611">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="91ff5-611">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-612">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-612">Network</span></span>

* <span data-ttu-id="91ff5-613">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-613">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="91ff5-614">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-614">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="91ff5-615">4910</span><span class="sxs-lookup"><span data-stu-id="91ff5-615">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="91ff5-616">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="91ff5-616">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="91ff5-617">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="91ff5-617">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="91ff5-618">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-618">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="91ff5-619">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-619">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="91ff5-620">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="91ff5-620">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-621">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-621">Profile</span></span>

* <span data-ttu-id="91ff5-622">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="91ff5-622">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="91ff5-623">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="91ff5-623">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="91ff5-624">RDBMS</span><span class="sxs-lookup"><span data-stu-id="91ff5-624">RDBMS</span></span>

* <span data-ttu-id="91ff5-625">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-625">Added `georestore` command</span></span>
* <span data-ttu-id="91ff5-626">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-626">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-627">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-627">Resource</span></span>

* <span data-ttu-id="91ff5-628">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-628">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="91ff5-629">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-629">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-630">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-630">SQL</span></span>

* <span data-ttu-id="91ff5-631">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="91ff5-631">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-632">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-632">Storage</span></span>

* <span data-ttu-id="91ff5-633">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="91ff5-633">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-634">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-634">VM</span></span>

* <span data-ttu-id="91ff5-635">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-635">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="91ff5-636">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="91ff5-636">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="91ff5-638">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-638">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="91ff5-639">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="91ff5-639">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="91ff5-640">5718</span><span class="sxs-lookup"><span data-stu-id="91ff5-640">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="91ff5-641">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="91ff5-641">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="91ff5-642">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-642">March 27, 2018</span></span>

<span data-ttu-id="91ff5-643">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="91ff5-643">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-644">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-644">Core</span></span>

* <span data-ttu-id="91ff5-645">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="91ff5-645">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-646">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-646">ACS</span></span>

* <span data-ttu-id="91ff5-647">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="91ff5-647">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-648">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-648">Appservice</span></span>

* <span data-ttu-id="91ff5-649">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-649">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="91ff5-650">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-650">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="91ff5-651">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="91ff5-651">Backup</span></span>

* <span data-ttu-id="91ff5-652">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-652">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="91ff5-653">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-653">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="91ff5-654">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="91ff5-654">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="91ff5-655">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="91ff5-655">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-656">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-656">Container</span></span>

* <span data-ttu-id="91ff5-657">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-657">Added `container exec` command.</span></span> <span data-ttu-id="91ff5-658">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="91ff5-658">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="91ff5-659">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="91ff5-659">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-660">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-660">Extension</span></span>

* <span data-ttu-id="91ff5-661">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="91ff5-661">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="91ff5-662">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="91ff5-662">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="91ff5-663">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="91ff5-663">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-664">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-664">Interactive</span></span>

* <span data-ttu-id="91ff5-665">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-665">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="91ff5-666">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="91ff5-666">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="91ff5-667">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-667">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="91ff5-668">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="91ff5-668">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="91ff5-669">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-669">Lab</span></span>

* <span data-ttu-id="91ff5-670">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="91ff5-670">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-671">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-671">Monitor</span></span>

* <span data-ttu-id="91ff5-672">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="91ff5-672">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="91ff5-673">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="91ff5-673">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="91ff5-674">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="91ff5-674">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-675">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-675">Network</span></span>

* <span data-ttu-id="91ff5-676">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="91ff5-676">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-677">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-677">Profile</span></span>

* <span data-ttu-id="91ff5-678">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="91ff5-678">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="91ff5-679">RDBMS</span><span class="sxs-lookup"><span data-stu-id="91ff5-679">RDBMS</span></span>

* <span data-ttu-id="91ff5-680">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="91ff5-680">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-681">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-681">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="91ff5-683">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-683">Role</span></span>

* <span data-ttu-id="91ff5-684">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-684">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="91ff5-685">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="91ff5-685">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="91ff5-686">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-686">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="91ff5-687">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-687">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="91ff5-688">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="91ff5-688">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-689">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-689">Storage</span></span>

* <span data-ttu-id="91ff5-690">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="91ff5-690">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="91ff5-691">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="91ff5-691">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-692">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-692">VM</span></span>

* <span data-ttu-id="91ff5-693">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="91ff5-693">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="91ff5-694">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-694">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="91ff5-695">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="91ff5-695">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="91ff5-696">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="91ff5-696">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="91ff5-697">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-697">March 13, 2018</span></span>

<span data-ttu-id="91ff5-698">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="91ff5-698">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-699">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-699">ACR</span></span>

* <span data-ttu-id="91ff5-700">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-700">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="91ff5-701">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-701">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="91ff5-702">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-702">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-703">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-703">ACS</span></span>

* <span data-ttu-id="91ff5-704">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="91ff5-704">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="91ff5-705">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="91ff5-705">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="91ff5-706">Advisor</span><span class="sxs-lookup"><span data-stu-id="91ff5-706">Advisor</span></span>

* <span data-ttu-id="91ff5-707">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="91ff5-707">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="91ff5-708">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-708">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="91ff5-709">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="91ff5-709">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="91ff5-710">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="91ff5-710">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="91ff5-711">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-711">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-712">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-712">Appservice</span></span>

* <span data-ttu-id="91ff5-713">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-713">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="91ff5-714">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-714">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="91ff5-715">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="91ff5-715">Eventhubs</span></span>

* <span data-ttu-id="91ff5-716">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="91ff5-716">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-717">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-717">Extension</span></span>

* <span data-ttu-id="91ff5-718">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="91ff5-718">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-719">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-719">Interactive</span></span>

* <span data-ttu-id="91ff5-720">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="91ff5-720">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="91ff5-721">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="91ff5-721">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="91ff5-722">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="91ff5-722">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="91ff5-723">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="91ff5-723">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-724">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-724">Monitor</span></span>

* <span data-ttu-id="91ff5-725">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-725">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="91ff5-726">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-726">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="91ff5-727">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-727">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="91ff5-728">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-728">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-729">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-729">Network</span></span>

* <span data-ttu-id="91ff5-730">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-730">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="91ff5-731">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="91ff5-731">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="91ff5-732">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-732">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="91ff5-733">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-733">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-734">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-734">Profile</span></span>

* <span data-ttu-id="91ff5-735">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-735">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="91ff5-736">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-736">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="91ff5-737">RDBMS</span><span class="sxs-lookup"><span data-stu-id="91ff5-737">RDBMS</span></span>

* <span data-ttu-id="91ff5-738">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="91ff5-738">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="91ff5-739">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="91ff5-739">Service Bus</span></span>

* <span data-ttu-id="91ff5-740">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="91ff5-740">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-741">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-741">Storage</span></span>

* <span data-ttu-id="91ff5-742">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="91ff5-742">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="91ff5-743">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="91ff5-743">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-744">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-744">VM</span></span>

* <span data-ttu-id="91ff5-745">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="91ff5-745">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="91ff5-746">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-746">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="91ff5-747">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-747">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="91ff5-748">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="91ff5-748">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="91ff5-749">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-749">February 27, 2018</span></span>

<span data-ttu-id="91ff5-750">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="91ff5-750">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-751">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-751">Core</span></span>

* <span data-ttu-id="91ff5-752">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="91ff5-752">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="91ff5-753">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="91ff5-753">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="91ff5-754">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="91ff5-754">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-755">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-755">ACS</span></span>

* <span data-ttu-id="91ff5-756">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="91ff5-756">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="91ff5-757">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="91ff5-757">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="91ff5-758">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="91ff5-758">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="91ff5-759">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="91ff5-759">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-760">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-760">Appservice</span></span>

* <span data-ttu-id="91ff5-761">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="91ff5-761">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="91ff5-762">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="91ff5-762">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="91ff5-763">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="91ff5-763">Cognitive Services</span></span>

* <span data-ttu-id="91ff5-764">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="91ff5-764">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="91ff5-765">Consumo</span><span class="sxs-lookup"><span data-stu-id="91ff5-765">Consumption</span></span>

* <span data-ttu-id="91ff5-766">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="91ff5-766">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="91ff5-767">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="91ff5-767">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-768">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-768">Container</span></span>

* <span data-ttu-id="91ff5-769">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="91ff5-769">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-770">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-770">Network</span></span>

* <span data-ttu-id="91ff5-771">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="91ff5-771">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-772">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-772">Resource</span></span>

* <span data-ttu-id="91ff5-773">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="91ff5-773">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-774">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-774">Role</span></span>

* <span data-ttu-id="91ff5-775">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="91ff5-775">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-776">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-776">SQL</span></span>

* <span data-ttu-id="91ff5-777">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="91ff5-777">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-778">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-778">Storage</span></span>

* <span data-ttu-id="91ff5-779">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-779">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-780">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-780">VM</span></span>

* <span data-ttu-id="91ff5-781">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="91ff5-781">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="91ff5-782">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-782">February 13, 2018</span></span>

<span data-ttu-id="91ff5-783">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="91ff5-783">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-784">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-784">Core</span></span>

* <span data-ttu-id="91ff5-785">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="91ff5-785">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-786">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-786">ACS</span></span>

* <span data-ttu-id="91ff5-787">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-787">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="91ff5-788">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-788">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="91ff5-789">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="91ff5-789">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="91ff5-790">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="91ff5-790">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="91ff5-791">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="91ff5-791">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="91ff5-792">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="91ff5-792">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="91ff5-793">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="91ff5-793">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="91ff5-794">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="91ff5-794">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-795">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-795">Appservice</span></span>

* <span data-ttu-id="91ff5-796">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="91ff5-796">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="91ff5-797">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="91ff5-797">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="91ff5-798">CDN</span><span class="sxs-lookup"><span data-stu-id="91ff5-798">CDN</span></span>

* <span data-ttu-id="91ff5-799">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-799">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-800">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-800">Container</span></span>

* <span data-ttu-id="91ff5-801">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="91ff5-801">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="91ff5-802">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="91ff5-802">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="91ff5-803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="91ff5-803">CosmosDB</span></span>

* <span data-ttu-id="91ff5-804">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="91ff5-804">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-805">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-805">Extension</span></span>

* <span data-ttu-id="91ff5-806">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-806">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="91ff5-807">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-807">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="91ff5-808">Comentarios</span><span class="sxs-lookup"><span data-stu-id="91ff5-808">Feedback</span></span>

* <span data-ttu-id="91ff5-809">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="91ff5-809">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-810">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-810">Interactive</span></span>

* <span data-ttu-id="91ff5-811">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="91ff5-811">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="91ff5-812">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="91ff5-812">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="91ff5-813">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-813">IoT</span></span>

* <span data-ttu-id="91ff5-814">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-814">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="91ff5-815">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-815">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="91ff5-816">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-816">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="91ff5-817">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="91ff5-817">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-818">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-818">Monitor</span></span>

* <span data-ttu-id="91ff5-819">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-819">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-820">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-820">Network</span></span>

* <span data-ttu-id="91ff5-821">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="91ff5-821">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="91ff5-822">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-822">Profile</span></span>

* <span data-ttu-id="91ff5-823">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="91ff5-823">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-824">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-824">Resource</span></span>

* <span data-ttu-id="91ff5-825">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="91ff5-825">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-826">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-826">Role</span></span>

* <span data-ttu-id="91ff5-827">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-827">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-828">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-828">SQL</span></span>

* <span data-ttu-id="91ff5-829">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-829">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="91ff5-830">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-830">Added `sql db rename`</span></span>
* <span data-ttu-id="91ff5-831">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="91ff5-831">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-832">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-832">Storage</span></span>

* <span data-ttu-id="91ff5-833">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="91ff5-833">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-834">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-834">VM</span></span>

* <span data-ttu-id="91ff5-835">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="91ff5-835">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="91ff5-836">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="91ff5-836">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="91ff5-837">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="91ff5-837">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="91ff5-838">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-838">January 31, 2018</span></span>

<span data-ttu-id="91ff5-839">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="91ff5-839">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-840">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-840">Core</span></span>

* <span data-ttu-id="91ff5-841">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="91ff5-841">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="91ff5-842">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="91ff5-842">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="91ff5-843">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="91ff5-843">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="91ff5-844">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="91ff5-844">Use `--verbose` to see</span></span>
* <span data-ttu-id="91ff5-845">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="91ff5-845">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-846">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-846">ACS</span></span>

* <span data-ttu-id="91ff5-847">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="91ff5-847">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="91ff5-848">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="91ff5-848">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-849">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-849">Appservice</span></span>

* <span data-ttu-id="91ff5-850">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="91ff5-850">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="91ff5-851">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="91ff5-851">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="91ff5-852">CDN</span><span class="sxs-lookup"><span data-stu-id="91ff5-852">CDN</span></span>

* <span data-ttu-id="91ff5-853">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-853">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="91ff5-854">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="91ff5-854">CosmosDB</span></span>

* <span data-ttu-id="91ff5-855">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="91ff5-855">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-856">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-856">Interactive</span></span>

* <span data-ttu-id="91ff5-857">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="91ff5-857">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-858">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-858">Network</span></span>

* <span data-ttu-id="91ff5-859">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-859">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="91ff5-860">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="91ff5-860">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="91ff5-861">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-861">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="91ff5-862">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-862">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="91ff5-863">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="91ff5-863">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="91ff5-864">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="91ff5-864">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="91ff5-865">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="91ff5-865">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="91ff5-866">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="91ff5-866">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="91ff5-867">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="91ff5-867">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="91ff5-868">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="91ff5-868">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-869">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-869">Profile</span></span>

* <span data-ttu-id="91ff5-870">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="91ff5-870">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-871">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-871">Resource</span></span>

* <span data-ttu-id="91ff5-872">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="91ff5-872">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-873">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-873">Storage</span></span>

* <span data-ttu-id="91ff5-874">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="91ff5-874">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="91ff5-875">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="91ff5-875">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="91ff5-876">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="91ff5-876">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="91ff5-877">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-877">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="91ff5-878">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="91ff5-878">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-879">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-879">VM</span></span>

* <span data-ttu-id="91ff5-880">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="91ff5-880">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="91ff5-881">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="91ff5-881">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="91ff5-882">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="91ff5-882">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="91ff5-883">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-883">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="91ff5-884">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="91ff5-884">January 17, 2018</span></span>

<span data-ttu-id="91ff5-885">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="91ff5-885">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-886">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-886">ACR</span></span>

* <span data-ttu-id="91ff5-887">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="91ff5-887">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="91ff5-888">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="91ff5-888">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-889">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-889">ACS</span></span>

* <span data-ttu-id="91ff5-890">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="91ff5-890">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="91ff5-891">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="91ff5-891">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-892">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-892">Appservice</span></span>

* <span data-ttu-id="91ff5-893">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="91ff5-893">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="91ff5-894">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="91ff5-894">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="91ff5-895">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="91ff5-895">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="91ff5-896">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="91ff5-896">Backup</span></span>

* <span data-ttu-id="91ff5-897">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="91ff5-897">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="91ff5-898">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="91ff5-898">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="91ff5-899">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="91ff5-899">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="91ff5-900">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="91ff5-900">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="91ff5-901">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="91ff5-901">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-902">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-902">Batch</span></span>

* <span data-ttu-id="91ff5-903">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="91ff5-903">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="91ff5-904">Nube</span><span class="sxs-lookup"><span data-stu-id="91ff5-904">Cloud</span></span>

* <span data-ttu-id="91ff5-905">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="91ff5-905">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="91ff5-906">Consumo</span><span class="sxs-lookup"><span data-stu-id="91ff5-906">Consumption</span></span>

* <span data-ttu-id="91ff5-907">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="91ff5-907">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="91ff5-908">Event Grid</span><span class="sxs-lookup"><span data-stu-id="91ff5-908">Event Grid</span></span>

* <span data-ttu-id="91ff5-909">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="91ff5-909">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="91ff5-910">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="91ff5-910">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="91ff5-911">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-911">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="91ff5-912">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="91ff5-912">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="91ff5-913">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-913">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="91ff5-914">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-914">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="91ff5-915">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="91ff5-915">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="91ff5-916">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="91ff5-916">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-917">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-917">Interactive</span></span>

* <span data-ttu-id="91ff5-918">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="91ff5-918">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="91ff5-919">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="91ff5-919">Fixed errors on startup</span></span>
* <span data-ttu-id="91ff5-920">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="91ff5-920">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="91ff5-921">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-921">IoT</span></span>

* <span data-ttu-id="91ff5-922">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="91ff5-922">Added support for device provisioning service</span></span>
* <span data-ttu-id="91ff5-923">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-923">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="91ff5-924">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-924">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-925">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-925">Monitor</span></span>

* <span data-ttu-id="91ff5-926">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-926">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="91ff5-927">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-927">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="91ff5-928">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="91ff5-928">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-929">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-929">Network</span></span>

* <span data-ttu-id="91ff5-930">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-930">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="91ff5-931">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-931">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-932">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-932">Profile</span></span>

* <span data-ttu-id="91ff5-933">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="91ff5-933">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-934">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-934">Role</span></span>

* <span data-ttu-id="91ff5-935">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="91ff5-935">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="91ff5-936">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="91ff5-936">Service Fabric</span></span>

* <span data-ttu-id="91ff5-937">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="91ff5-937">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="91ff5-938">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="91ff5-938">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-939">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-939">VM</span></span>

* <span data-ttu-id="91ff5-940">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="91ff5-940">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="91ff5-941">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="91ff5-941">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="91ff5-942">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="91ff5-942">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="91ff5-943">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="91ff5-943">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="91ff5-944">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="91ff5-944">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="91ff5-945">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-945">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="91ff5-946">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-946">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="91ff5-947">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="91ff5-947">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="91ff5-948">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-948">December 19, 2017</span></span>

<span data-ttu-id="91ff5-949">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="91ff5-949">Version 2.0.23</span></span>

* <span data-ttu-id="91ff5-950">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="91ff5-950">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-951">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-951">Container</span></span>

* <span data-ttu-id="91ff5-952">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-952">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-953">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-953">Network</span></span>

* <span data-ttu-id="91ff5-954">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-954">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="91ff5-955">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-955">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-956">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-956">Storage</span></span>

* <span data-ttu-id="91ff5-957">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="91ff5-957">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-958">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-958">VM</span></span>

* <span data-ttu-id="91ff5-959">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="91ff5-959">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="91ff5-960">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-960">December 5, 2017</span></span>

<span data-ttu-id="91ff5-961">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="91ff5-961">Version 2.0.22</span></span>

* <span data-ttu-id="91ff5-962">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-962">Removed `az component` commands.</span></span> <span data-ttu-id="91ff5-963">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="91ff5-963">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-964">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-964">Core</span></span>
* <span data-ttu-id="91ff5-965">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="91ff5-965">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="91ff5-966">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="91ff5-966">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-967">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-967">ACS</span></span>

* <span data-ttu-id="91ff5-968">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="91ff5-968">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="91ff5-969">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-969">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="91ff5-970">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="91ff5-970">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="91ff5-971">Advisor</span><span class="sxs-lookup"><span data-stu-id="91ff5-971">Advisor</span></span>

* <span data-ttu-id="91ff5-972">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="91ff5-972">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-973">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-973">Appservice</span></span>

* <span data-ttu-id="91ff5-974">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="91ff5-974">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="91ff5-975">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="91ff5-975">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="91ff5-976">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="91ff5-976">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="91ff5-977">Consumo</span><span class="sxs-lookup"><span data-stu-id="91ff5-977">Consumption</span></span>

* <span data-ttu-id="91ff5-978">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="91ff5-978">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-979">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-979">Container</span></span>

* <span data-ttu-id="91ff5-980">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="91ff5-980">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-981">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-981">Monitor</span></span>

* <span data-ttu-id="91ff5-982">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="91ff5-982">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-983">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-983">Resource</span></span>

* <span data-ttu-id="91ff5-984">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="91ff5-984">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-985">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-985">Role</span></span>

* <span data-ttu-id="91ff5-986">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="91ff5-986">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="91ff5-987">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="91ff5-987">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="91ff5-988">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="91ff5-988">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-989">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-989">SQL</span></span>

* <span data-ttu-id="91ff5-990">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="91ff5-990">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="91ff5-991">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-991">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-992">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-992">VM</span></span>

* <span data-ttu-id="91ff5-993">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="91ff5-993">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="91ff5-994">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-994">November 14, 2017</span></span>

<span data-ttu-id="91ff5-995">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="91ff5-995">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-996">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-996">ACR</span></span>

* <span data-ttu-id="91ff5-997">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="91ff5-997">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="91ff5-998">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-998">ACS</span></span>

* <span data-ttu-id="91ff5-999">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="91ff5-999">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="91ff5-1000">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1000">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="91ff5-1001">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1001">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="91ff5-1002">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="91ff5-1002">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="91ff5-1003">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="91ff5-1003">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1004">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1004">Appservice</span></span>

* <span data-ttu-id="91ff5-1005">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="91ff5-1005">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="91ff5-1006">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1006">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="91ff5-1007">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1007">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="91ff5-1008">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1008">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="91ff5-1009">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="91ff5-1009">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="91ff5-1010">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="91ff5-1010">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-1011">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-1011">Batch</span></span>

* <span data-ttu-id="91ff5-1012">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1012">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="91ff5-1013">Batchai</span><span class="sxs-lookup"><span data-stu-id="91ff5-1013">Batchai</span></span>

* <span data-ttu-id="91ff5-1014">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1014">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="91ff5-1015">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1015">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="91ff5-1016">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1016">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="91ff5-1017">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1017">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="91ff5-1018">Nube</span><span class="sxs-lookup"><span data-stu-id="91ff5-1018">Cloud</span></span>

* <span data-ttu-id="91ff5-1019">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="91ff5-1019">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-1020">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-1020">Container</span></span>

* <span data-ttu-id="91ff5-1021">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1021">Added support to open multiple ports</span></span>
* <span data-ttu-id="91ff5-1022">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="91ff5-1022">Added container group restart policy</span></span>
* <span data-ttu-id="91ff5-1023">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="91ff5-1023">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="91ff5-1024">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="91ff5-1024">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="91ff5-1025">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="91ff5-1025">Data Lake Analytics</span></span>

* <span data-ttu-id="91ff5-1026">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="91ff5-1026">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="91ff5-1027">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="91ff5-1027">Data Lake Store</span></span>

* <span data-ttu-id="91ff5-1028">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="91ff5-1028">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-1029">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-1029">Extension</span></span>

* <span data-ttu-id="91ff5-1030">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="91ff5-1030">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="91ff5-1031">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="91ff5-1031">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="91ff5-1032">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-1032">IoT</span></span>

* <span data-ttu-id="91ff5-1033">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="91ff5-1033">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-1034">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-1034">Monitor</span></span>

* <span data-ttu-id="91ff5-1035">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1035">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-1036">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1036">Network</span></span>

* <span data-ttu-id="91ff5-1037">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="91ff5-1037">Added support for CAA DNS records</span></span>
* <span data-ttu-id="91ff5-1038">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1038">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="91ff5-1039">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1039">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="91ff5-1040">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1040">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="91ff5-1041">Reservations</span><span class="sxs-lookup"><span data-stu-id="91ff5-1041">Reservations</span></span>

* <span data-ttu-id="91ff5-1042">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="91ff5-1042">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-1043">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1043">Resource</span></span>

* <span data-ttu-id="91ff5-1044">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1044">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-1045">SQL</span></span>

* <span data-ttu-id="91ff5-1046">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1046">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1047">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1047">Storage</span></span>

* <span data-ttu-id="91ff5-1048">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="91ff5-1048">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="91ff5-1049">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="91ff5-1049">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="91ff5-1050">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1050">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="91ff5-1051">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1051">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="91ff5-1052">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1052">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="91ff5-1053">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1053">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="91ff5-1054">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1054">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1055">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1055">VM</span></span>

* <span data-ttu-id="91ff5-1056">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1056">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="91ff5-1057">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="91ff5-1057">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="91ff5-1058">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="91ff5-1058">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="91ff5-1059">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1059">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="91ff5-1060">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1060">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="91ff5-1061">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1061">October 24, 2017</span></span>

<span data-ttu-id="91ff5-1062">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="91ff5-1062">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-1063">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-1063">Core</span></span>

* <span data-ttu-id="91ff5-1064">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1064">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-1065">ACR</span></span>

* <span data-ttu-id="91ff5-1066">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="91ff5-1066">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="91ff5-1067">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="91ff5-1067">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="91ff5-1068">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="91ff5-1068">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1069">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1069">ACS</span></span>

* <span data-ttu-id="91ff5-1070">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1070">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="91ff5-1071">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="91ff5-1071">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1072">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1072">Appservice</span></span>

* <span data-ttu-id="91ff5-1073">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1073">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="91ff5-1074">Componente</span><span class="sxs-lookup"><span data-stu-id="91ff5-1074">Component</span></span>

* <span data-ttu-id="91ff5-1075">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="91ff5-1075">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-1076">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-1076">Monitor</span></span>

* <span data-ttu-id="91ff5-1077">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1077">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-1078">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1078">Resource</span></span>

* <span data-ttu-id="91ff5-1079">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1079">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="91ff5-1080">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="91ff5-1080">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1081">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1081">VM</span></span>

* <span data-ttu-id="91ff5-1082">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1082">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="91ff5-1083">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1083">October 9, 2017</span></span>

<span data-ttu-id="91ff5-1084">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="91ff5-1084">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-1085">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-1085">Core</span></span>

* <span data-ttu-id="91ff5-1086">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="91ff5-1086">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1087">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1087">Appservice</span></span>

* <span data-ttu-id="91ff5-1088">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1088">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-1089">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-1089">Batch</span></span>

* <span data-ttu-id="91ff5-1090">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="91ff5-1090">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="91ff5-1091">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="91ff5-1091">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="91ff5-1092">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-1092">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="91ff5-1093">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="91ff5-1093">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="91ff5-1094">Batchai</span><span class="sxs-lookup"><span data-stu-id="91ff5-1094">Batchai</span></span>

* <span data-ttu-id="91ff5-1095">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-1095">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="91ff5-1096">Keyvault</span><span class="sxs-lookup"><span data-stu-id="91ff5-1096">Keyvault</span></span>

* <span data-ttu-id="91ff5-1097">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1097">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="91ff5-1098">(#4448)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1098">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="91ff5-1099">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1099">Network</span></span>

* <span data-ttu-id="91ff5-1100">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1100">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="91ff5-1101">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="91ff5-1101">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-1102">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1102">Resource</span></span>

* <span data-ttu-id="91ff5-1103">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1103">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="91ff5-1104">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="91ff5-1104">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="91ff5-1105">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="91ff5-1105">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="91ff5-1106">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1106">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-1107">Sql</span><span class="sxs-lookup"><span data-stu-id="91ff5-1107">Sql</span></span>

* <span data-ttu-id="91ff5-1108">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="91ff5-1108">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="91ff5-1109">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="91ff5-1109">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="91ff5-1110">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1110">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1111">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1111">Storage</span></span>

* <span data-ttu-id="91ff5-1112">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1112">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1113">Vm</span><span class="sxs-lookup"><span data-stu-id="91ff5-1113">Vm</span></span>

* <span data-ttu-id="91ff5-1114">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="91ff5-1114">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="91ff5-1115">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1115">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="91ff5-1116">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1116">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="91ff5-1117">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1117">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="91ff5-1118">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1118">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="91ff5-1119">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1119">September 22, 2017</span></span>

<span data-ttu-id="91ff5-1120">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="91ff5-1120">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-1121">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1121">Resource</span></span>

* <span data-ttu-id="91ff5-1122">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="91ff5-1122">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="91ff5-1123">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="91ff5-1123">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="91ff5-1124">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1124">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="91ff5-1125">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1125">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-1126">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1126">Network</span></span>

* <span data-ttu-id="91ff5-1127">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1127">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="91ff5-1128">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1128">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="91ff5-1129">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1129">Added `asg` application security group commands</span></span>
* <span data-ttu-id="91ff5-1130">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1130">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="91ff5-1131">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1131">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="91ff5-1132">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1132">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="91ff5-1133">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1133">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1134">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1134">Storage</span></span>

* <span data-ttu-id="91ff5-1135">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="91ff5-1135">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="91ff5-1136">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="91ff5-1136">Eventgrid</span></span>

* <span data-ttu-id="91ff5-1137">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="91ff5-1137">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-1138">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-1138">SQL</span></span>

* <span data-ttu-id="91ff5-1139">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1139">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="91ff5-1140">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="91ff5-1140">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="91ff5-1141">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1141">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="91ff5-1142">Keyvault</span><span class="sxs-lookup"><span data-stu-id="91ff5-1142">Keyvault</span></span>

* <span data-ttu-id="91ff5-1143">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="91ff5-1143">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1144">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1144">VM</span></span>

* <span data-ttu-id="91ff5-1145">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1145">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="91ff5-1146">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="91ff5-1146">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="91ff5-1147">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1147">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="91ff5-1148">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1148">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="91ff5-1149">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1149">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="91ff5-1150">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1150">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1151">ACS</span></span>

* <span data-ttu-id="91ff5-1152">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1152">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1153">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1153">Appservice</span></span>

* <span data-ttu-id="91ff5-1154">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1154">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="91ff5-1155">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="91ff5-1155">Backup</span></span>

* <span data-ttu-id="91ff5-1156">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="91ff5-1156">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="91ff5-1157">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1157">September 11, 2017</span></span>

<span data-ttu-id="91ff5-1158">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="91ff5-1158">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="91ff5-1159">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-1159">Core</span></span>

* <span data-ttu-id="91ff5-1160">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1160">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="91ff5-1161">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1161">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1162">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1162">Acs</span></span>

* <span data-ttu-id="91ff5-1163">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1163">Added `acs list-locations` command</span></span>
* <span data-ttu-id="91ff5-1164">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1164">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1165">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1165">Appservice</span></span>

* <span data-ttu-id="91ff5-1166">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1166">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="91ff5-1167">CDN</span><span class="sxs-lookup"><span data-stu-id="91ff5-1167">CDN</span></span>

* <span data-ttu-id="91ff5-1168">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1168">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="91ff5-1169">Extensión</span><span class="sxs-lookup"><span data-stu-id="91ff5-1169">Extension</span></span>

* <span data-ttu-id="91ff5-1170">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="91ff5-1170">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="91ff5-1171">Keyvault</span><span class="sxs-lookup"><span data-stu-id="91ff5-1171">Keyvault</span></span>

* <span data-ttu-id="91ff5-1172">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1172">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-1173">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1173">Network</span></span>

* <span data-ttu-id="91ff5-1174">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1174">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="91ff5-1175">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1175">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="91ff5-1176">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1176">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="91ff5-1177">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1177">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="91ff5-1178">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1178">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-1179">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1179">Resource</span></span>

* <span data-ttu-id="91ff5-1180">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1180">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="91ff5-1181">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1181">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="91ff5-1182">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1182">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="91ff5-1183">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="91ff5-1183">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-1184">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-1184">SQL</span></span>

* <span data-ttu-id="91ff5-1185">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1185">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1186">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1186">VM</span></span>

* <span data-ttu-id="91ff5-1187">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1187">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="91ff5-1188">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1188">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="91ff5-1189">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1189">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="91ff5-1190">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1190">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="91ff5-1191">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1191">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="91ff5-1192">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1192">August 31, 2017</span></span>

<span data-ttu-id="91ff5-1193">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="91ff5-1193">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="91ff5-1194">Keyvault</span><span class="sxs-lookup"><span data-stu-id="91ff5-1194">Keyvault</span></span>

* <span data-ttu-id="91ff5-1195">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1195">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="91ff5-1196">Sf</span><span class="sxs-lookup"><span data-stu-id="91ff5-1196">Sf</span></span>

* <span data-ttu-id="91ff5-1197">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1197">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1198">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1198">Storage</span></span>

* <span data-ttu-id="91ff5-1199">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1199">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="91ff5-1200">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1200">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="91ff5-1201">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1201">August 28, 2017</span></span>

<span data-ttu-id="91ff5-1202">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="91ff5-1202">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="91ff5-1203">CLI</span><span class="sxs-lookup"><span data-stu-id="91ff5-1203">CLI</span></span>

* <span data-ttu-id="91ff5-1204">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1204">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1205">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1205">ACS</span></span>

* <span data-ttu-id="91ff5-1206">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="91ff5-1206">Corrected preview regions</span></span>
* <span data-ttu-id="91ff5-1207">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1207">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="91ff5-1208">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="91ff5-1208">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1209">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1209">Appservice</span></span>

* <span data-ttu-id="91ff5-1210">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1210">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="91ff5-1211">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1211">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="91ff5-1212">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1212">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="91ff5-1213">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1213">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="91ff5-1214">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1214">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="91ff5-1215">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-1215">IoT</span></span>

* <span data-ttu-id="91ff5-1216">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1216">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-1217">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1217">Network</span></span>

* <span data-ttu-id="91ff5-1218">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1218">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="91ff5-1219">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1219">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="91ff5-1220">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1220">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="91ff5-1221">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="91ff5-1222">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1222">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-1223">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-1223">Profile</span></span>

* <span data-ttu-id="91ff5-1224">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1224">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="91ff5-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="91ff5-1225">Service Fabric</span></span>

* <span data-ttu-id="91ff5-1226">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="91ff5-1226">Preview release</span></span>
* <span data-ttu-id="91ff5-1227">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1227">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="91ff5-1228">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1228">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="91ff5-1229">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1229">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1230">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1230">Storage</span></span>

* <span data-ttu-id="91ff5-1231">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1231">Enabled setting blob tier</span></span>
* <span data-ttu-id="91ff5-1232">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1232">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="91ff5-1233">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1233">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="91ff5-1234">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1234">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="91ff5-1235">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1235">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="91ff5-1236">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="91ff5-1236">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1237">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1237">VM</span></span>

* <span data-ttu-id="91ff5-1238">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1238">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="91ff5-1239">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1239">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="91ff5-1240">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1240">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="91ff5-1241">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1241">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="91ff5-1242">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1242">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="91ff5-1243">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1243">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="91ff5-1244">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1244">August 15, 2017</span></span>

<span data-ttu-id="91ff5-1245">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="91ff5-1245">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1246">ACS</span></span>

* <span data-ttu-id="91ff5-1247">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="91ff5-1247">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1248">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1248">Appservice</span></span>

* <span data-ttu-id="91ff5-1249">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1249">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="91ff5-1250">Event Grid</span><span class="sxs-lookup"><span data-stu-id="91ff5-1250">Event Grid</span></span>

* <span data-ttu-id="91ff5-1251">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1251">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="91ff5-1252">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1252">August 11, 2017</span></span>

<span data-ttu-id="91ff5-1253">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="91ff5-1253">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1254">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1254">ACS</span></span>

* <span data-ttu-id="91ff5-1255">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="91ff5-1255">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-1256">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-1256">Batch</span></span>

* <span data-ttu-id="91ff5-1257">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1257">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="91ff5-1258">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1258">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="91ff5-1259">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1259">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="91ff5-1260">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1260">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="91ff5-1261">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1261">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="91ff5-1262">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1262">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="91ff5-1263">Componente</span><span class="sxs-lookup"><span data-stu-id="91ff5-1263">Component</span></span>

* <span data-ttu-id="91ff5-1264">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1264">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="91ff5-1265">Contenedor</span><span class="sxs-lookup"><span data-stu-id="91ff5-1265">Container</span></span>

* <span data-ttu-id="91ff5-1266">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1266">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="91ff5-1267">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="91ff5-1267">Data Lake Store</span></span>

* <span data-ttu-id="91ff5-1268">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1268">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="91ff5-1269">Event Grid</span><span class="sxs-lookup"><span data-stu-id="91ff5-1269">Event Grid</span></span>

* <span data-ttu-id="91ff5-1270">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1270">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-1271">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1271">Network</span></span>

* <span data-ttu-id="91ff5-1272">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1272">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="91ff5-1273">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1273">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="91ff5-1274">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1274">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="91ff5-1275">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1275">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-1276">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-1276">Profile</span></span>

* <span data-ttu-id="91ff5-1277">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1277">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1278">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1278">Storage</span></span>

* <span data-ttu-id="91ff5-1279">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1279">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1280">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1280">VM</span></span>

* <span data-ttu-id="91ff5-1281">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1281">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="91ff5-1282">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1282">Exposed `list-skus` command</span></span>
* <span data-ttu-id="91ff5-1283">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1283">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="91ff5-1284">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1284">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="91ff5-1285">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1285">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="91ff5-1286">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1286">July 28, 2017</span></span>

<span data-ttu-id="91ff5-1287">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="91ff5-1287">Version 2.0.12</span></span>

* <span data-ttu-id="91ff5-1288">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1288">Added container commands</span></span>
* <span data-ttu-id="91ff5-1289">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1289">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="91ff5-1290">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-1290">Core</span></span>

* <span data-ttu-id="91ff5-1291">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1291">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="91ff5-1292">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1292">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="91ff5-1293">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1293">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="91ff5-1294">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1294">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="91ff5-1295">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1295">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="91ff5-1296">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1296">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="91ff5-1297">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1297">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="91ff5-1298">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1298">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="91ff5-1299">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1299">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="91ff5-1300">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1300">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="91ff5-1301">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1301">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="91ff5-1302">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1302">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="91ff5-1303">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1303">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="91ff5-1304">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1304">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="91ff5-1305">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1305">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="91ff5-1306">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1306">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="91ff5-1307">ACR</span><span class="sxs-lookup"><span data-stu-id="91ff5-1307">ACR</span></span>

* <span data-ttu-id="91ff5-1308">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1308">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="91ff5-1309">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1309">Support SKU update for managed registries</span></span>
* <span data-ttu-id="91ff5-1310">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1310">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="91ff5-1311">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1311">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="91ff5-1312">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1312">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="91ff5-1313">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1313">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1314">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1314">ACS</span></span>

* <span data-ttu-id="91ff5-1315">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1315">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1316">Appservice</span><span class="sxs-lookup"><span data-stu-id="91ff5-1316">Appservice</span></span>

* <span data-ttu-id="91ff5-1317">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1317">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="91ff5-1318">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1318">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="91ff5-1319">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1319">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="91ff5-1320">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1320">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="91ff5-1321">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1321">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="91ff5-1322">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1322">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="91ff5-1323">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1323">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="91ff5-1324">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1324">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="91ff5-1325">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1325">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="91ff5-1326">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1326">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="91ff5-1327">Batch</span><span class="sxs-lookup"><span data-stu-id="91ff5-1327">Batch</span></span>

* <span data-ttu-id="91ff5-1328">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1328">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="91ff5-1329">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1329">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="91ff5-1330">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1330">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="91ff5-1331">CDN</span><span class="sxs-lookup"><span data-stu-id="91ff5-1331">CDN</span></span>

* <span data-ttu-id="91ff5-1332">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="91ff5-1332">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="91ff5-1333">Nube</span><span class="sxs-lookup"><span data-stu-id="91ff5-1333">Cloud</span></span>

* <span data-ttu-id="91ff5-1334">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1334">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="91ff5-1335">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1335">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="91ff5-1336">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1336">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="91ff5-1337">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1337">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="91ff5-1338">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1338">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="91ff5-1339">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="91ff5-1339">CosmosDB</span></span>

* <span data-ttu-id="91ff5-1340">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1340">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="91ff5-1341">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="91ff5-1341">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="91ff5-1342">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="91ff5-1342">Data Lake Analytics</span></span>

* <span data-ttu-id="91ff5-1343">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1343">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="91ff5-1344">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1344">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="91ff5-1345">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1345">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="91ff5-1346">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="91ff5-1346">Data Lake Store</span></span>

* <span data-ttu-id="91ff5-1347">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1347">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="91ff5-1348">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1348">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="91ff5-1349">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1349">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="91ff5-1350">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1350">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="91ff5-1351">Interactive</span><span class="sxs-lookup"><span data-stu-id="91ff5-1351">Interactive</span></span>

* <span data-ttu-id="91ff5-1352">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1352">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="91ff5-1353">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1353">Increased test coverage</span></span>
* <span data-ttu-id="91ff5-1354">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1354">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="91ff5-1355">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1355">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="91ff5-1356">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1356">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="91ff5-1357">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1357">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="91ff5-1358">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1358">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="91ff5-1359">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1359">Added `--progress` flag</span></span>
* <span data-ttu-id="91ff5-1360">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1360">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="91ff5-1361">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1361">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="91ff5-1362">IoT</span><span class="sxs-lookup"><span data-stu-id="91ff5-1362">IoT</span></span>

* <span data-ttu-id="91ff5-1363">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1363">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="91ff5-1364">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1364">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="91ff5-1365">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="91ff5-1365">Key vault</span></span>

* <span data-ttu-id="91ff5-1366">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="91ff5-1366">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="91ff5-1367">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1367">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="91ff5-1368">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1368">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="91ff5-1369">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1369">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="91ff5-1370">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1370">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="91ff5-1371">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1371">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="91ff5-1372">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="91ff5-1372">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="91ff5-1373">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1373">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="91ff5-1374">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-1374">Lab</span></span>

* <span data-ttu-id="91ff5-1375">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1375">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="91ff5-1376">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1376">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-1377">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-1377">Monitor</span></span>

* <span data-ttu-id="91ff5-1378">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1378">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="91ff5-1379">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1379">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="91ff5-1380">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1380">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="91ff5-1381">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1381">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="91ff5-1382">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1382">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="91ff5-1383">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="91ff5-1383">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="91ff5-1384">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1384">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="91ff5-1385">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1385">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="91ff5-1386">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1386">`location` no longer required</span></span>
  * <span data-ttu-id="91ff5-1387">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1387">Add name and ID support for target</span></span>
  * <span data-ttu-id="91ff5-1388">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1388">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="91ff5-1389">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1389">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="91ff5-1390">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1390">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="91ff5-1391">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1391">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="91ff5-1392">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1392">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="91ff5-1393">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1393">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-1394">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1394">Network</span></span>

* <span data-ttu-id="91ff5-1395">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1395">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="91ff5-1396">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1396">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="91ff5-1397">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1397">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="91ff5-1398">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1398">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="91ff5-1399">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1399">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="91ff5-1400">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1400">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="91ff5-1401">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1401">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="91ff5-1402">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1402">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="91ff5-1403">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1403">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="91ff5-1404">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1404">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="91ff5-1405">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1405">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="91ff5-1406">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1406">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="91ff5-1407">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1407">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="91ff5-1408">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1408">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="91ff5-1409">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1409">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="91ff5-1410">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1410">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="91ff5-1411">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1411">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="91ff5-1412">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1412">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="91ff5-1413">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1413">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="91ff5-1414">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1414">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="91ff5-1415">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1415">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="91ff5-1416">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1416">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="91ff5-1417">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1417">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="91ff5-1418">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1418">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="91ff5-1419">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1419">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="91ff5-1420">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1420">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="91ff5-1421">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1421">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-1422">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-1422">Profile</span></span>

* <span data-ttu-id="91ff5-1423">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1423">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="91ff5-1424">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1424">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="91ff5-1425">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="91ff5-1425">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="91ff5-1426">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1426">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="91ff5-1427">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1427">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="91ff5-1428">RDBMS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1428">RDBMS</span></span>

* <span data-ttu-id="91ff5-1429">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1429">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="91ff5-1430">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1430">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="91ff5-1431">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1431">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="91ff5-1432">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1432">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-1433">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1433">Resource</span></span>

* <span data-ttu-id="91ff5-1434">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1434">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="91ff5-1435">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1435">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="91ff5-1436">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1436">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="91ff5-1437">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1437">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="91ff5-1438">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1438">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="91ff5-1439">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1439">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="91ff5-1440">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1440">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="91ff5-1441">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1441">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-1442">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-1442">Role</span></span>

* <span data-ttu-id="91ff5-1443">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1443">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="91ff5-1444">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1444">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="91ff5-1445">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1445">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="91ff5-1446">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1446">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="91ff5-1447">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1447">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="91ff5-1448">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="91ff5-1448">Service Fabric</span></span>
* <span data-ttu-id="91ff5-1449">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1449">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="91ff5-1450">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1450">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="91ff5-1451">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1451">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-1452">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-1452">SQL</span></span>

* <span data-ttu-id="91ff5-1453">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1453">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="91ff5-1454">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1454">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="91ff5-1455">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1455">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1456">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1456">Storage</span></span>

* <span data-ttu-id="91ff5-1457">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1457">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="91ff5-1458">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1458">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="91ff5-1459">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1459">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="91ff5-1460">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1460">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="91ff5-1461">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1461">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="91ff5-1462">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1462">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1463">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1463">VM</span></span>

* <span data-ttu-id="91ff5-1464">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="91ff5-1464">Support configuring nsg</span></span>
* <span data-ttu-id="91ff5-1465">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1465">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="91ff5-1466">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1466">Support managed service identities</span></span>
* <span data-ttu-id="91ff5-1467">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1467">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="91ff5-1468">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="91ff5-1468">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="91ff5-1469">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1469">May 10, 2017</span></span>

<span data-ttu-id="91ff5-1470">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="91ff5-1470">Version 2.0.6</span></span>

* <span data-ttu-id="91ff5-1471">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1471">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="91ff5-1472">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1472">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="91ff5-1473">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="91ff5-1473">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="91ff5-1474">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="91ff5-1474">Include Cognitive Services module</span></span>
* <span data-ttu-id="91ff5-1475">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="91ff5-1475">Include Service Fabric module</span></span>
* <span data-ttu-id="91ff5-1476">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1476">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="91ff5-1477">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="91ff5-1477">Add support for CDN commands</span></span>
* <span data-ttu-id="91ff5-1478">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="91ff5-1478">Remove Container module</span></span>
* <span data-ttu-id="91ff5-1479">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1479">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="91ff5-1480">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1480">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="91ff5-1481">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-1481">Core</span></span>

* <span data-ttu-id="91ff5-1482">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="91ff5-1482">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="91ff5-1483">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1483">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="91ff5-1484">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1484">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="91ff5-1485">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1485">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="91ff5-1486">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1486">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="91ff5-1487">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1487">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="91ff5-1488">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1488">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="91ff5-1489">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1489">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="91ff5-1490">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1490">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="91ff5-1491">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="91ff5-1491">core: Improved performance</span></span>
* <span data-ttu-id="91ff5-1492">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="91ff5-1492">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="91ff5-1493">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="91ff5-1493">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1494">ACS</span></span>

* <span data-ttu-id="91ff5-1495">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="91ff5-1495">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="91ff5-1496">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="91ff5-1496">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="91ff5-1497">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="91ff5-1497">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="91ff5-1498">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1498">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1499">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-1499">AppService</span></span>

* <span data-ttu-id="91ff5-1500">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1500">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="91ff5-1501">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="91ff5-1501">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="91ff5-1502">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1502">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="91ff5-1503">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="91ff5-1503">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="91ff5-1504">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="91ff5-1504">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="91ff5-1505">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1505">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="91ff5-1506">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="91ff5-1506">support slot swap with preview</span></span>
* <span data-ttu-id="91ff5-1507">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1507">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="91ff5-1508">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1508">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="91ff5-1509">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="91ff5-1509">CosmosDB</span></span>

* <span data-ttu-id="91ff5-1510">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="91ff5-1510">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="91ff5-1511">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1511">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="91ff5-1512">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="91ff5-1512">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="91ff5-1513">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="91ff5-1513">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="91ff5-1514">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="91ff5-1514">Data Lake Analytics</span></span>

* <span data-ttu-id="91ff5-1515">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="91ff5-1515">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="91ff5-1516">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="91ff5-1516">Add support for new catalog item type: package.</span></span> <span data-ttu-id="91ff5-1517">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1517">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="91ff5-1518">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="91ff5-1518">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="91ff5-1519">Tabla</span><span class="sxs-lookup"><span data-stu-id="91ff5-1519">Table</span></span>
  * <span data-ttu-id="91ff5-1520">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="91ff5-1520">Table valued function</span></span>
  * <span data-ttu-id="91ff5-1521">Ver</span><span class="sxs-lookup"><span data-stu-id="91ff5-1521">View</span></span>
  * <span data-ttu-id="91ff5-1522">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1522">Table Statistics.</span></span> <span data-ttu-id="91ff5-1523">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="91ff5-1523">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="91ff5-1524">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="91ff5-1524">Data Lake Store</span></span>

* <span data-ttu-id="91ff5-1525">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="91ff5-1525">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="91ff5-1526">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1526">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="91ff5-1527">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1527">missed help for access show.</span></span> <span data-ttu-id="91ff5-1528">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1528">adding it.</span></span> <span data-ttu-id="91ff5-1529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="91ff5-1530">Buscar</span><span class="sxs-lookup"><span data-stu-id="91ff5-1530">Find</span></span>

* <span data-ttu-id="91ff5-1531">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="91ff5-1531">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="91ff5-1532">KeyVault</span><span class="sxs-lookup"><span data-stu-id="91ff5-1532">KeyVault</span></span>

* <span data-ttu-id="91ff5-1533">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="91ff5-1533">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="91ff5-1534">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="91ff5-1534">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="91ff5-1535">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="91ff5-1535">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="91ff5-1536">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="91ff5-1536">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="91ff5-1537">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1537">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="91ff5-1538">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-1538">Lab</span></span>

* <span data-ttu-id="91ff5-1539">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-1539">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="91ff5-1540">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-1540">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="91ff5-1541">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-1541">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="91ff5-1542">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-1542">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="91ff5-1543">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="91ff5-1543">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="91ff5-1544">Supervisión</span><span class="sxs-lookup"><span data-stu-id="91ff5-1544">Monitor</span></span>

* <span data-ttu-id="91ff5-1545">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1545">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="91ff5-1546">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1546">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="91ff5-1547">Red</span><span class="sxs-lookup"><span data-stu-id="91ff5-1547">Network</span></span>

* <span data-ttu-id="91ff5-1548">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1548">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="91ff5-1549">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1549">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="91ff5-1550">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="91ff5-1550">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="91ff5-1551">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="91ff5-1551">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="91ff5-1552">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="91ff5-1552">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="91ff5-1553">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="91ff5-1553">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="91ff5-1554">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="91ff5-1554">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="91ff5-1555">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="91ff5-1555">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="91ff5-1556">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1556">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="91ff5-1557">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="91ff5-1557">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="91ff5-1558">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1558">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="91ff5-1559">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1559">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="91ff5-1560">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="91ff5-1560">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="91ff5-1561">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="91ff5-1561">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="91ff5-1562">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="91ff5-1562">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="91ff5-1563">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="91ff5-1563">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="91ff5-1564">Perfil</span><span class="sxs-lookup"><span data-stu-id="91ff5-1564">Profile</span></span>

* <span data-ttu-id="91ff5-1565">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1565">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="91ff5-1566">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1566">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="91ff5-1567">Redis</span><span class="sxs-lookup"><span data-stu-id="91ff5-1567">Redis</span></span>

* <span data-ttu-id="91ff5-1568">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="91ff5-1568">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="91ff5-1569">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="91ff5-1569">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="91ff5-1570">Recurso</span><span class="sxs-lookup"><span data-stu-id="91ff5-1570">Resource</span></span>

* <span data-ttu-id="91ff5-1571">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1571">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="91ff5-1572">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1572">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="91ff5-1573">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1573">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="91ff5-1574">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="91ff5-1574">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="91ff5-1575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="91ff5-1576">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="91ff5-1576">Add docs for az lock update.</span></span> <span data-ttu-id="91ff5-1577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="91ff5-1578">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="91ff5-1578">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="91ff5-1579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="91ff5-1580">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="91ff5-1580">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="91ff5-1581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="91ff5-1582">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1582">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="91ff5-1583">Rol</span><span class="sxs-lookup"><span data-stu-id="91ff5-1583">Role</span></span>

* <span data-ttu-id="91ff5-1584">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1584">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="91ff5-1585">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1585">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="91ff5-1586">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1586">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="91ff5-1587">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="91ff5-1587">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="91ff5-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="91ff5-1588">SQL</span></span>

* <span data-ttu-id="91ff5-1589">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="91ff5-1589">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="91ff5-1590">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1590">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="91ff5-1591">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1591">Storage</span></span>

* <span data-ttu-id="91ff5-1592">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1592">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="91ff5-1593">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="91ff5-1593">Add support for incremental blob copy</span></span>
* <span data-ttu-id="91ff5-1594">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="91ff5-1594">Add support for large block blob upload</span></span>
* <span data-ttu-id="91ff5-1595">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="91ff5-1595">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1596">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1596">VM</span></span>

* <span data-ttu-id="91ff5-1597">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="91ff5-1597">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="91ff5-1598">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="91ff5-1598">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="91ff5-1599">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="91ff5-1599">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="91ff5-1600">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="91ff5-1600">az vm/vmss disk</span></span>
  3. <span data-ttu-id="91ff5-1601">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="91ff5-1601">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="91ff5-1602">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="91ff5-1602">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="91ff5-1603">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1603">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="91ff5-1604">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1604">April 3, 2017</span></span>

<span data-ttu-id="91ff5-1605">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="91ff5-1605">Version 2.0.2</span></span>

<span data-ttu-id="91ff5-1606">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="91ff5-1606">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="91ff5-1607">Núcleo</span><span class="sxs-lookup"><span data-stu-id="91ff5-1607">Core</span></span>

* <span data-ttu-id="91ff5-1608">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="91ff5-1608">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="91ff5-1609">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1609">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="91ff5-1610">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1610">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="91ff5-1611">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1611">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="91ff5-1612">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1612">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="91ff5-1613">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1613">Add prompting for missing template parameters.</span></span> <span data-ttu-id="91ff5-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="91ff5-1615">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="91ff5-1615">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="91ff5-1616">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="91ff5-1616">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="91ff5-1617">ACS</span><span class="sxs-lookup"><span data-stu-id="91ff5-1617">ACS</span></span>

* <span data-ttu-id="91ff5-1618">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1618">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="91ff5-1619">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1619">Add support for ssh key password prompting.</span></span> <span data-ttu-id="91ff5-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="91ff5-1621">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1621">Add support for windows clusters.</span></span> <span data-ttu-id="91ff5-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="91ff5-1623">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="91ff5-1623">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="91ff5-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="91ff5-1625">AppService</span><span class="sxs-lookup"><span data-stu-id="91ff5-1625">AppService</span></span>

* <span data-ttu-id="91ff5-1626">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1626">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="91ff5-1627">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1627">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="91ff5-1628">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1628">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="91ff5-1629">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1629">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="91ff5-1630">DataLake</span><span class="sxs-lookup"><span data-stu-id="91ff5-1630">DataLake</span></span>

* <span data-ttu-id="91ff5-1631">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="91ff5-1631">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="91ff5-1632">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="91ff5-1632">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="91ff5-1633">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="91ff5-1633">DocuemntDB</span></span>

* <span data-ttu-id="91ff5-1634">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1634">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="91ff5-1635">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="91ff5-1635">VM</span></span>

* <span data-ttu-id="91ff5-1636">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1636">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="91ff5-1637">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1637">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="91ff5-1638">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1638">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="91ff5-1639">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1639">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="91ff5-1640">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1640">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="91ff5-1641">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1641">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="91ff5-1642">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="91ff5-1642">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="91ff5-1643">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="91ff5-1643">February 27, 2017</span></span>

<span data-ttu-id="91ff5-1644">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="91ff5-1644">Version 2.0.0</span></span>

<span data-ttu-id="91ff5-1645">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="91ff5-1645">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="91ff5-1646">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1646">Container Service (acs)</span></span>
- <span data-ttu-id="91ff5-1647">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1647">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="91ff5-1648">Redes</span><span class="sxs-lookup"><span data-stu-id="91ff5-1648">Networking</span></span>
- <span data-ttu-id="91ff5-1649">Storage</span><span class="sxs-lookup"><span data-stu-id="91ff5-1649">Storage</span></span>

<span data-ttu-id="91ff5-1650">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1650">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="91ff5-1651">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="91ff5-1651">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="91ff5-1652">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="91ff5-1652">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="91ff5-1653">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="91ff5-1653">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="91ff5-1654">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="91ff5-1654">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="91ff5-1655">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="91ff5-1655">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="91ff5-1656">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1656">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="91ff5-1657">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="91ff5-1657">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="91ff5-1658">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="91ff5-1658">Provide feedback from the command line with the `az feedback` command</span></span>

