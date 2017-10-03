---
title: "Notas de la versión de la CLI de Azure 2.0"
description: "Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0"
keywords: "CLI de Azure 2.0, notas de la versión"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 72630c52b5e6afd69809ff19145717c0d65e0252
ms.sourcegitcommit: 3a490ae3a2a1b2e63a062806f9b720fa4c6be01e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="020dc-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="020dc-104">Azure CLI 2.0 release notes</span></span>

## <a name="september-22-2017"></a><span data-ttu-id="020dc-105">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-105">September 22, 2017</span></span>

<span data-ttu-id="020dc-106">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="020dc-106">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="020dc-107">Recurso</span><span class="sxs-lookup"><span data-stu-id="020dc-107">Resource</span></span>

* <span data-ttu-id="020dc-108">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="020dc-108">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="020dc-109">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="020dc-109">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="020dc-110">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="020dc-110">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="020dc-111">[NUEVO CAMBIO] Se cambió el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="020dc-111">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="020dc-112">Red</span><span class="sxs-lookup"><span data-stu-id="020dc-112">Network</span></span>

* <span data-ttu-id="020dc-113">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="020dc-113">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="020dc-114">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="020dc-114">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="020dc-115">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="020dc-115">Added `asg` application security group commands</span></span>
* <span data-ttu-id="020dc-116">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="020dc-116">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="020dc-117">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="020dc-117">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="020dc-118">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="020dc-118">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="020dc-119">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="020dc-119">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="020dc-120">Storage</span><span class="sxs-lookup"><span data-stu-id="020dc-120">Storage</span></span>

* <span data-ttu-id="020dc-121">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="020dc-121">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="020dc-122">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="020dc-122">Eventgrid</span></span>

* <span data-ttu-id="020dc-123">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="020dc-123">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="020dc-124">SQL</span><span class="sxs-lookup"><span data-stu-id="020dc-124">SQL</span></span>

* <span data-ttu-id="020dc-125">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="020dc-125">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="020dc-126">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="020dc-126">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="020dc-127">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="020dc-127">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="020dc-128">Keyvault</span><span class="sxs-lookup"><span data-stu-id="020dc-128">Keyvault</span></span>

* <span data-ttu-id="020dc-129">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="020dc-129">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="020dc-130">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="020dc-130">VM</span></span>

* <span data-ttu-id="020dc-131">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="020dc-131">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="020dc-132">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="020dc-132">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="020dc-133">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="020dc-133">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="020dc-134">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="020dc-134">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="020dc-135">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="020dc-135">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="020dc-136">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="020dc-136">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="020dc-137">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-137">ACS</span></span>

* <span data-ttu-id="020dc-138">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-138">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="020dc-139">Appservice</span><span class="sxs-lookup"><span data-stu-id="020dc-139">Appservice</span></span>

* <span data-ttu-id="020dc-140">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="020dc-140">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="020dc-141">Backup</span><span class="sxs-lookup"><span data-stu-id="020dc-141">Backup</span></span>

* <span data-ttu-id="020dc-142">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="020dc-142">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="020dc-143">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-143">September 11, 2017</span></span>

<span data-ttu-id="020dc-144">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="020dc-144">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="020dc-145">Núcleo</span><span class="sxs-lookup"><span data-stu-id="020dc-145">Core</span></span>

* <span data-ttu-id="020dc-146">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="020dc-146">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="020dc-147">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="020dc-147">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="020dc-148">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-148">Acs</span></span>

* <span data-ttu-id="020dc-149">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="020dc-149">Added `acs list-locations` command</span></span>
* <span data-ttu-id="020dc-150">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="020dc-150">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="020dc-151">Appservice</span><span class="sxs-lookup"><span data-stu-id="020dc-151">Appservice</span></span>

* <span data-ttu-id="020dc-152">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="020dc-152">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="020dc-153">CDN</span><span class="sxs-lookup"><span data-stu-id="020dc-153">CDN</span></span>

* <span data-ttu-id="020dc-154">Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-154">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="020dc-155">Extensión</span><span class="sxs-lookup"><span data-stu-id="020dc-155">Extension</span></span>

* <span data-ttu-id="020dc-156">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="020dc-156">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="020dc-157">Keyvault</span><span class="sxs-lookup"><span data-stu-id="020dc-157">Keyvault</span></span>

* <span data-ttu-id="020dc-158">Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="020dc-158">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="020dc-159">Red</span><span class="sxs-lookup"><span data-stu-id="020dc-159">Network</span></span>

* <span data-ttu-id="020dc-160">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="020dc-160">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="020dc-161">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-161">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="020dc-162">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-162">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="020dc-163">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-163">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="020dc-164">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-164">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="020dc-165">Recurso</span><span class="sxs-lookup"><span data-stu-id="020dc-165">Resource</span></span>

* <span data-ttu-id="020dc-166">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-166">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="020dc-167">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-167">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="020dc-168">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="020dc-168">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="020dc-169">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="020dc-169">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="020dc-170">SQL</span><span class="sxs-lookup"><span data-stu-id="020dc-170">SQL</span></span>

* <span data-ttu-id="020dc-171">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="020dc-171">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="020dc-172">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="020dc-172">VM</span></span>

* <span data-ttu-id="020dc-173">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="020dc-173">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="020dc-174">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="020dc-174">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="020dc-175">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-175">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="020dc-176">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="020dc-176">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="020dc-177">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="020dc-177">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="020dc-178">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-178">August 31, 2017</span></span>

<span data-ttu-id="020dc-179">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="020dc-179">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="020dc-180">Keyvault</span><span class="sxs-lookup"><span data-stu-id="020dc-180">Keyvault</span></span>

* <span data-ttu-id="020dc-181">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="020dc-181">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="020dc-182">Sf</span><span class="sxs-lookup"><span data-stu-id="020dc-182">Sf</span></span>

* <span data-ttu-id="020dc-183">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="020dc-183">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="020dc-184">Storage</span><span class="sxs-lookup"><span data-stu-id="020dc-184">Storage</span></span>

* <span data-ttu-id="020dc-185">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="020dc-185">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="020dc-186">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="020dc-186">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="020dc-187">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-187">August 28, 2017</span></span>

<span data-ttu-id="020dc-188">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="020dc-188">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="020dc-189">CLI</span><span class="sxs-lookup"><span data-stu-id="020dc-189">CLI</span></span>

* <span data-ttu-id="020dc-190">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="020dc-190">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="020dc-191">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-191">ACS</span></span>

* <span data-ttu-id="020dc-192">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="020dc-192">Corrected preview regions.</span></span>
* <span data-ttu-id="020dc-193">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="020dc-193">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="020dc-194">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="020dc-194">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="020dc-195">Appservice</span><span class="sxs-lookup"><span data-stu-id="020dc-195">Appservice</span></span>

* <span data-ttu-id="020dc-196">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="020dc-196">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="020dc-197">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="020dc-197">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="020dc-198">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="020dc-198">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="020dc-199">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="020dc-199">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="020dc-200">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="020dc-200">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="020dc-201">IoT</span><span class="sxs-lookup"><span data-stu-id="020dc-201">IoT</span></span>

* <span data-ttu-id="020dc-202">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="020dc-202">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="020dc-203">Red</span><span class="sxs-lookup"><span data-stu-id="020dc-203">Network</span></span>

* <span data-ttu-id="020dc-204">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="020dc-204">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="020dc-205">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="020dc-205">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="020dc-206">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="020dc-206">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="020dc-207">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-207">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="020dc-208">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-208">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="020dc-209">Perfil</span><span class="sxs-lookup"><span data-stu-id="020dc-209">Profile</span></span>

* <span data-ttu-id="020dc-210">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="020dc-210">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="020dc-211">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="020dc-211">Service Fabric</span></span>

* <span data-ttu-id="020dc-212">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="020dc-212">Preview release</span></span>
* <span data-ttu-id="020dc-213">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="020dc-213">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="020dc-214">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="020dc-214">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="020dc-215">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="020dc-215">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="020dc-216">Storage</span><span class="sxs-lookup"><span data-stu-id="020dc-216">Storage</span></span>

* <span data-ttu-id="020dc-217">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="020dc-217">Enabled setting blob tier</span></span>
* <span data-ttu-id="020dc-218">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="020dc-218">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="020dc-219">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="020dc-219">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="020dc-220">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="020dc-220">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="020dc-221">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-221">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="020dc-222">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="020dc-222">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="020dc-223">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="020dc-223">VM</span></span>

* <span data-ttu-id="020dc-224">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="020dc-224">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="020dc-225">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-225">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="020dc-226">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-226">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="020dc-227">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="020dc-227">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="020dc-228">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="020dc-228">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="020dc-229">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-229">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="020dc-230">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-230">August 15, 2017</span></span>

<span data-ttu-id="020dc-231">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="020dc-231">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="020dc-232">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-232">ACS</span></span>

* <span data-ttu-id="020dc-233">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="020dc-233">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="020dc-234">Appservice</span><span class="sxs-lookup"><span data-stu-id="020dc-234">Appservice</span></span>

* <span data-ttu-id="020dc-235">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="020dc-235">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="020dc-236">Event Grid</span><span class="sxs-lookup"><span data-stu-id="020dc-236">Event Grid</span></span>

* <span data-ttu-id="020dc-237">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="020dc-237">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="020dc-238">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-238">August 11, 2017</span></span>

<span data-ttu-id="020dc-239">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="020dc-239">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="020dc-240">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-240">ACS</span></span>

* <span data-ttu-id="020dc-241">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="020dc-241">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="020dc-242">Batch</span><span class="sxs-lookup"><span data-stu-id="020dc-242">Batch</span></span>

* <span data-ttu-id="020dc-243">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="020dc-243">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="020dc-244">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="020dc-244">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="020dc-245">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="020dc-245">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="020dc-246">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="020dc-246">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="020dc-247">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="020dc-247">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="020dc-248">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="020dc-248">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="020dc-249">Componente</span><span class="sxs-lookup"><span data-stu-id="020dc-249">Component</span></span>

* <span data-ttu-id="020dc-250">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="020dc-250">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="020dc-251">Contenedor</span><span class="sxs-lookup"><span data-stu-id="020dc-251">Container</span></span>

* <span data-ttu-id="020dc-252">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="020dc-252">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="020dc-253">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="020dc-253">Data Lake Store</span></span>

* <span data-ttu-id="020dc-254">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="020dc-254">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="020dc-255">Event Grid</span><span class="sxs-lookup"><span data-stu-id="020dc-255">Event Grid</span></span>

* <span data-ttu-id="020dc-256">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="020dc-256">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="020dc-257">Red</span><span class="sxs-lookup"><span data-stu-id="020dc-257">Network</span></span>

* <span data-ttu-id="020dc-258">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="020dc-258">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="020dc-259">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="020dc-259">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="020dc-260">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="020dc-260">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="020dc-261">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="020dc-261">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="020dc-262">Perfil</span><span class="sxs-lookup"><span data-stu-id="020dc-262">Profile</span></span>

* <span data-ttu-id="020dc-263">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="020dc-263">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="020dc-264">Storage</span><span class="sxs-lookup"><span data-stu-id="020dc-264">Storage</span></span>

* <span data-ttu-id="020dc-265">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="020dc-265">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="020dc-266">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="020dc-266">VM</span></span>

* <span data-ttu-id="020dc-267">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="020dc-267">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="020dc-268">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="020dc-268">Exposed `list-skus` command</span></span>
* <span data-ttu-id="020dc-269">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="020dc-269">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="020dc-270">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="020dc-270">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="020dc-271">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="020dc-271">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="020dc-272">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-272">July 28, 2017</span></span>

<span data-ttu-id="020dc-273">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="020dc-273">Version 2.0.12</span></span>

* <span data-ttu-id="020dc-274">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="020dc-274">Added container commands</span></span>
* <span data-ttu-id="020dc-275">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="020dc-275">Added billing and consumption modules</span></span>

```
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

### <a name="core"></a><span data-ttu-id="020dc-276">Núcleo</span><span class="sxs-lookup"><span data-stu-id="020dc-276">Core</span></span>

* <span data-ttu-id="020dc-277">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="020dc-277">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="020dc-278">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="020dc-278">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="020dc-279">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="020dc-279">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="020dc-280">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="020dc-280">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="020dc-281">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="020dc-281">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="020dc-282">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="020dc-282">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="020dc-283">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="020dc-283">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="020dc-284">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="020dc-284">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="020dc-285">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="020dc-285">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="020dc-286">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="020dc-286">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="020dc-287">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="020dc-287">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="020dc-288">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="020dc-288">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="020dc-289">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="020dc-289">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="020dc-290">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="020dc-290">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="020dc-291">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="020dc-291">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="020dc-292">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="020dc-292">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="020dc-293">ACR</span><span class="sxs-lookup"><span data-stu-id="020dc-293">ACR</span></span>

* <span data-ttu-id="020dc-294">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="020dc-294">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="020dc-295">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="020dc-295">Support SKU update for managed registries</span></span>
* <span data-ttu-id="020dc-296">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="020dc-296">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="020dc-297">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="020dc-297">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="020dc-298">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="020dc-298">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="020dc-299">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="020dc-299">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="020dc-300">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-300">ACS</span></span>

* <span data-ttu-id="020dc-301">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="020dc-301">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="020dc-302">Appservice</span><span class="sxs-lookup"><span data-stu-id="020dc-302">Appservice</span></span>

* <span data-ttu-id="020dc-303">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="020dc-303">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="020dc-304">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="020dc-304">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="020dc-305">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="020dc-305">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="020dc-306">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="020dc-306">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="020dc-307">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="020dc-307">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="020dc-308">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="020dc-308">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="020dc-309">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="020dc-309">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="020dc-310">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="020dc-310">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="020dc-311">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="020dc-311">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="020dc-312">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="020dc-312">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="020dc-313">Batch</span><span class="sxs-lookup"><span data-stu-id="020dc-313">Batch</span></span>

* <span data-ttu-id="020dc-314">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="020dc-314">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="020dc-315">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="020dc-315">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="020dc-316">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-316">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="020dc-317">CDN</span><span class="sxs-lookup"><span data-stu-id="020dc-317">CDN</span></span>

* <span data-ttu-id="020dc-318">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="020dc-318">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="020dc-319">Nube</span><span class="sxs-lookup"><span data-stu-id="020dc-319">Cloud</span></span>

* <span data-ttu-id="020dc-320">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="020dc-320">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="020dc-321">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="020dc-321">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="020dc-322">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="020dc-322">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="020dc-323">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="020dc-323">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="020dc-324">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="020dc-324">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="020dc-325">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="020dc-325">CosmosDB</span></span>

* <span data-ttu-id="020dc-326">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="020dc-326">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="020dc-327">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="020dc-327">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="020dc-328">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="020dc-328">Data Lake Analytics</span></span>

* <span data-ttu-id="020dc-329">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="020dc-329">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="020dc-330">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="020dc-330">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="020dc-331">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="020dc-331">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="020dc-332">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="020dc-332">Data Lake Store</span></span>

* <span data-ttu-id="020dc-333">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-333">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="020dc-334">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="020dc-334">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="020dc-335">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="020dc-335">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="020dc-336">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="020dc-336">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="020dc-337">Interactive</span><span class="sxs-lookup"><span data-stu-id="020dc-337">Interactive</span></span>

* <span data-ttu-id="020dc-338">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="020dc-338">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="020dc-339">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="020dc-339">Increased test coverage</span></span>
* <span data-ttu-id="020dc-340">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="020dc-340">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="020dc-341">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="020dc-341">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="020dc-342">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="020dc-342">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="020dc-343">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="020dc-343">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="020dc-344">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="020dc-344">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="020dc-345">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="020dc-345">Added `--progress` flag</span></span>
* <span data-ttu-id="020dc-346">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="020dc-346">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="020dc-347">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="020dc-347">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="020dc-348">IoT</span><span class="sxs-lookup"><span data-stu-id="020dc-348">IoT</span></span>

* <span data-ttu-id="020dc-349">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="020dc-349">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="020dc-350">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="020dc-350">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="020dc-351">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="020dc-351">Key vault</span></span>

* <span data-ttu-id="020dc-352">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="020dc-352">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="020dc-353">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="020dc-353">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="020dc-354">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="020dc-354">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="020dc-355">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="020dc-355">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="020dc-356">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="020dc-356">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="020dc-357">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="020dc-357">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="020dc-358">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="020dc-358">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="020dc-359">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="020dc-359">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="020dc-360">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="020dc-360">Lab</span></span>

* <span data-ttu-id="020dc-361">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="020dc-361">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="020dc-362">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="020dc-362">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="020dc-363">Supervisión</span><span class="sxs-lookup"><span data-stu-id="020dc-363">Monitor</span></span>

* <span data-ttu-id="020dc-364">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="020dc-364">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="020dc-365">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="020dc-365">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="020dc-366">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="020dc-366">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="020dc-367">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="020dc-367">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="020dc-368">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="020dc-368">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="020dc-369">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="020dc-369">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="020dc-370">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="020dc-370">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="020dc-371">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="020dc-371">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="020dc-372">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="020dc-372">`location` no longer required</span></span>
  * <span data-ttu-id="020dc-373">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="020dc-373">Add name and ID support for target</span></span>
  * <span data-ttu-id="020dc-374">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="020dc-374">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="020dc-375">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="020dc-375">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="020dc-376">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="020dc-376">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="020dc-377">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="020dc-377">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="020dc-378">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="020dc-378">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="020dc-379">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="020dc-379">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="020dc-380">Red</span><span class="sxs-lookup"><span data-stu-id="020dc-380">Network</span></span>

* <span data-ttu-id="020dc-381">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="020dc-381">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="020dc-382">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-382">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="020dc-383">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="020dc-383">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="020dc-384">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="020dc-384">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="020dc-385">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-385">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="020dc-386">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="020dc-386">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="020dc-387">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="020dc-387">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="020dc-388">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="020dc-388">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="020dc-389">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="020dc-389">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="020dc-390">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="020dc-390">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="020dc-391">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="020dc-391">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="020dc-392">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="020dc-392">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="020dc-393">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="020dc-393">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="020dc-394">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-394">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="020dc-395">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-395">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="020dc-396">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-396">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="020dc-397">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="020dc-397">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="020dc-398">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="020dc-398">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="020dc-399">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-399">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="020dc-400">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-400">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="020dc-401">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-401">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="020dc-402">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="020dc-402">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="020dc-403">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="020dc-403">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="020dc-404">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="020dc-404">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="020dc-405">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="020dc-405">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="020dc-406">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="020dc-406">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="020dc-407">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="020dc-407">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="020dc-408">Perfil</span><span class="sxs-lookup"><span data-stu-id="020dc-408">Profile</span></span>

* <span data-ttu-id="020dc-409">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="020dc-409">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="020dc-410">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="020dc-410">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="020dc-411">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="020dc-411">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="020dc-412">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="020dc-412">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="020dc-413">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="020dc-413">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="020dc-414">RDBMS</span><span class="sxs-lookup"><span data-stu-id="020dc-414">RDBMS</span></span>

* <span data-ttu-id="020dc-415">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="020dc-415">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="020dc-416">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="020dc-416">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="020dc-417">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="020dc-417">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="020dc-418">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="020dc-418">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="020dc-419">Recurso</span><span class="sxs-lookup"><span data-stu-id="020dc-419">Resource</span></span>

* <span data-ttu-id="020dc-420">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-420">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="020dc-421">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="020dc-421">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="020dc-422">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="020dc-422">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="020dc-423">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="020dc-423">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="020dc-424">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="020dc-424">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="020dc-425">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="020dc-425">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="020dc-426">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="020dc-426">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="020dc-427">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="020dc-427">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="020dc-428">Rol</span><span class="sxs-lookup"><span data-stu-id="020dc-428">Role</span></span>

* <span data-ttu-id="020dc-429">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="020dc-429">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="020dc-430">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="020dc-430">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="020dc-431">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="020dc-431">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="020dc-432">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="020dc-432">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="020dc-433">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="020dc-433">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="020dc-434">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="020dc-434">Service Fabric</span></span>
* <span data-ttu-id="020dc-435">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="020dc-435">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="020dc-436">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="020dc-436">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="020dc-437">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="020dc-437">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="020dc-438">SQL</span><span class="sxs-lookup"><span data-stu-id="020dc-438">SQL</span></span>

* <span data-ttu-id="020dc-439">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="020dc-439">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="020dc-440">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="020dc-440">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="020dc-441">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="020dc-441">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="020dc-442">Storage</span><span class="sxs-lookup"><span data-stu-id="020dc-442">Storage</span></span>

* <span data-ttu-id="020dc-443">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="020dc-443">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="020dc-444">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="020dc-444">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="020dc-445">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="020dc-445">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="020dc-446">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="020dc-446">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="020dc-447">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="020dc-447">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="020dc-448">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="020dc-448">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="020dc-449">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="020dc-449">VM</span></span>

* <span data-ttu-id="020dc-450">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="020dc-450">Support configuring nsg</span></span>
* <span data-ttu-id="020dc-451">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="020dc-451">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="020dc-452">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="020dc-452">Support managed service identities</span></span>
* <span data-ttu-id="020dc-453">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="020dc-453">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="020dc-454">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="020dc-454">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="020dc-455">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-455">May 10, 2017</span></span>

<span data-ttu-id="020dc-456">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="020dc-456">Version 2.0.6</span></span>

* <span data-ttu-id="020dc-457">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="020dc-457">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="020dc-458">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="020dc-458">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="020dc-459">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="020dc-459">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="020dc-460">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="020dc-460">Include Cognitive Services module.</span></span>
* <span data-ttu-id="020dc-461">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="020dc-461">Include Service Fabric module.</span></span>
* <span data-ttu-id="020dc-462">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="020dc-462">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="020dc-463">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="020dc-463">Add support for CDN commands.</span></span>
* <span data-ttu-id="020dc-464">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="020dc-464">Remove Container module.</span></span>
* <span data-ttu-id="020dc-465">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="020dc-465">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="020dc-466">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="020dc-466">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```
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

### <a name="core"></a><span data-ttu-id="020dc-467">Núcleo</span><span class="sxs-lookup"><span data-stu-id="020dc-467">Core</span></span>

* <span data-ttu-id="020dc-468">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="020dc-468">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="020dc-469">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="020dc-469">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="020dc-470">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="020dc-470">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="020dc-471">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="020dc-471">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="020dc-472">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="020dc-472">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="020dc-473">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="020dc-473">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="020dc-474">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="020dc-474">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="020dc-475">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="020dc-475">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="020dc-476">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="020dc-476">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="020dc-477">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="020dc-477">core: Improved performance</span></span>
* <span data-ttu-id="020dc-478">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="020dc-478">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="020dc-479">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="020dc-479">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="020dc-480">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-480">ACS</span></span>

* <span data-ttu-id="020dc-481">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="020dc-481">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="020dc-482">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="020dc-482">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="020dc-483">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="020dc-483">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="020dc-484">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="020dc-484">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="020dc-485">AppService</span><span class="sxs-lookup"><span data-stu-id="020dc-485">AppService</span></span>

* <span data-ttu-id="020dc-486">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="020dc-486">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="020dc-487">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="020dc-487">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="020dc-488">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="020dc-488">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="020dc-489">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="020dc-489">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="020dc-490">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="020dc-490">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="020dc-491">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="020dc-491">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="020dc-492">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="020dc-492">support slot swap with preview</span></span>
* <span data-ttu-id="020dc-493">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="020dc-493">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="020dc-494">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="020dc-494">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="020dc-495">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="020dc-495">CosmosDB</span></span>

* <span data-ttu-id="020dc-496">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="020dc-496">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="020dc-497">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="020dc-497">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="020dc-498">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="020dc-498">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="020dc-499">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="020dc-499">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="020dc-500">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="020dc-500">Data Lake Analytics</span></span>

* <span data-ttu-id="020dc-501">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="020dc-501">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="020dc-502">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="020dc-502">Add support for new catalog item type: package.</span></span> <span data-ttu-id="020dc-503">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="020dc-503">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="020dc-504">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="020dc-504">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="020dc-505">Tabla</span><span class="sxs-lookup"><span data-stu-id="020dc-505">Table</span></span>
  * <span data-ttu-id="020dc-506">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="020dc-506">Table valued function</span></span>
  * <span data-ttu-id="020dc-507">Ver</span><span class="sxs-lookup"><span data-stu-id="020dc-507">View</span></span>
  * <span data-ttu-id="020dc-508">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="020dc-508">Table Statistics.</span></span> <span data-ttu-id="020dc-509">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="020dc-509">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="020dc-510">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="020dc-510">Data Lake Store</span></span>

* <span data-ttu-id="020dc-511">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="020dc-511">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="020dc-512">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="020dc-512">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="020dc-513">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="020dc-513">missed help for access show.</span></span> <span data-ttu-id="020dc-514">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="020dc-514">adding it.</span></span> <span data-ttu-id="020dc-515">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="020dc-515">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="020dc-516">Buscar</span><span class="sxs-lookup"><span data-stu-id="020dc-516">Find</span></span>

* <span data-ttu-id="020dc-517">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="020dc-517">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="020dc-518">KeyVault</span><span class="sxs-lookup"><span data-stu-id="020dc-518">KeyVault</span></span>

* <span data-ttu-id="020dc-519">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="020dc-519">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="020dc-520">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="020dc-520">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="020dc-521">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="020dc-521">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="020dc-522">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="020dc-522">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="020dc-523">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="020dc-523">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="020dc-524">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="020dc-524">Lab</span></span>

* <span data-ttu-id="020dc-525">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="020dc-525">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="020dc-526">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="020dc-526">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="020dc-527">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="020dc-527">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="020dc-528">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="020dc-528">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="020dc-529">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="020dc-529">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="020dc-530">Supervisión</span><span class="sxs-lookup"><span data-stu-id="020dc-530">Monitor</span></span>

* <span data-ttu-id="020dc-531">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="020dc-531">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="020dc-532">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="020dc-532">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="020dc-533">Red</span><span class="sxs-lookup"><span data-stu-id="020dc-533">Network</span></span>

* <span data-ttu-id="020dc-534">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="020dc-534">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="020dc-535">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="020dc-535">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="020dc-536">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="020dc-536">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="020dc-537">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="020dc-537">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="020dc-538">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="020dc-538">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="020dc-539">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="020dc-539">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="020dc-540">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="020dc-540">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="020dc-541">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="020dc-541">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="020dc-542">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="020dc-542">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="020dc-543">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="020dc-543">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="020dc-544">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="020dc-544">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="020dc-545">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="020dc-545">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="020dc-546">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="020dc-546">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="020dc-547">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="020dc-547">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="020dc-548">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="020dc-548">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="020dc-549">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="020dc-549">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="020dc-550">Perfil</span><span class="sxs-lookup"><span data-stu-id="020dc-550">Profile</span></span>

* <span data-ttu-id="020dc-551">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="020dc-551">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="020dc-552">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="020dc-552">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="020dc-553">Redis</span><span class="sxs-lookup"><span data-stu-id="020dc-553">Redis</span></span>

* <span data-ttu-id="020dc-554">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="020dc-554">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="020dc-555">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="020dc-555">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="020dc-556">Recurso</span><span class="sxs-lookup"><span data-stu-id="020dc-556">Resource</span></span>

* <span data-ttu-id="020dc-557">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="020dc-557">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="020dc-558">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="020dc-558">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="020dc-559">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="020dc-559">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="020dc-560">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="020dc-560">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="020dc-561">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="020dc-561">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="020dc-562">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="020dc-562">Add docs for az lock update.</span></span> <span data-ttu-id="020dc-563">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="020dc-563">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="020dc-564">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="020dc-564">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="020dc-565">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="020dc-565">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="020dc-566">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="020dc-566">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="020dc-567">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="020dc-567">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="020dc-568">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="020dc-568">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="020dc-569">Rol</span><span class="sxs-lookup"><span data-stu-id="020dc-569">Role</span></span>

* <span data-ttu-id="020dc-570">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="020dc-570">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="020dc-571">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="020dc-571">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="020dc-572">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="020dc-572">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="020dc-573">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="020dc-573">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="020dc-574">SQL</span><span class="sxs-lookup"><span data-stu-id="020dc-574">SQL</span></span>

* <span data-ttu-id="020dc-575">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="020dc-575">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="020dc-576">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="020dc-576">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="020dc-577">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="020dc-577">Storage</span></span>

* <span data-ttu-id="020dc-578">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="020dc-578">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="020dc-579">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="020dc-579">Add support for incremental blob copy</span></span>
* <span data-ttu-id="020dc-580">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="020dc-580">Add support for large block blob upload</span></span>
* <span data-ttu-id="020dc-581">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="020dc-581">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="020dc-582">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="020dc-582">VM</span></span>

* <span data-ttu-id="020dc-583">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="020dc-583">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="020dc-584">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="020dc-584">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="020dc-585">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="020dc-585">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="020dc-586">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="020dc-586">az vm/vmss disk</span></span>
  3. <span data-ttu-id="020dc-587">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="020dc-587">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="020dc-588">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="020dc-588">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="020dc-589">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="020dc-589">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="020dc-590">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-590">April 3, 2017</span></span>

<span data-ttu-id="020dc-591">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="020dc-591">Version 2.0.2</span></span>

<span data-ttu-id="020dc-592">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="020dc-592">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

```
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

### <a name="core"></a><span data-ttu-id="020dc-593">Núcleo</span><span class="sxs-lookup"><span data-stu-id="020dc-593">Core</span></span>

* <span data-ttu-id="020dc-594">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="020dc-594">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="020dc-595">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="020dc-595">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="020dc-596">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="020dc-596">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="020dc-597">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="020dc-597">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="020dc-598">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="020dc-598">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="020dc-599">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="020dc-599">Add prompting for missing template parameters.</span></span> <span data-ttu-id="020dc-600">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="020dc-600">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="020dc-601">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="020dc-601">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="020dc-602">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="020dc-602">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="020dc-603">ACS</span><span class="sxs-lookup"><span data-stu-id="020dc-603">ACS</span></span>

* <span data-ttu-id="020dc-604">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="020dc-604">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="020dc-605">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="020dc-605">Add support for ssh key password prompting.</span></span> <span data-ttu-id="020dc-606">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="020dc-606">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="020dc-607">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="020dc-607">Add support for windows clusters.</span></span> <span data-ttu-id="020dc-608">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="020dc-608">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="020dc-609">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="020dc-609">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="020dc-610">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="020dc-610">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="020dc-611">AppService</span><span class="sxs-lookup"><span data-stu-id="020dc-611">AppService</span></span>

* <span data-ttu-id="020dc-612">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="020dc-612">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="020dc-613">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="020dc-613">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="020dc-614">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="020dc-614">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="020dc-615">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="020dc-615">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="020dc-616">DataLake</span><span class="sxs-lookup"><span data-stu-id="020dc-616">DataLake</span></span>

* <span data-ttu-id="020dc-617">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="020dc-617">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="020dc-618">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="020dc-618">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="020dc-619">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="020dc-619">DocuemntDB</span></span>

* <span data-ttu-id="020dc-620">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="020dc-620">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="020dc-621">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="020dc-621">VM</span></span>

* <span data-ttu-id="020dc-622">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="020dc-622">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="020dc-623">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="020dc-623">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="020dc-624">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="020dc-624">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="020dc-625">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="020dc-625">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="020dc-626">Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="020dc-626">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="020dc-627">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="020dc-627">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="020dc-628">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="020dc-628">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="020dc-629">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="020dc-629">February 27, 2017</span></span>

<span data-ttu-id="020dc-630">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="020dc-630">Version 2.0.0</span></span>

<span data-ttu-id="020dc-631">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="020dc-631">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="020dc-632">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="020dc-632">General availability applies to these command modules:</span></span>
- <span data-ttu-id="020dc-633">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="020dc-633">Container Service (acs)</span></span>
- <span data-ttu-id="020dc-634">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="020dc-634">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="020dc-635">Redes</span><span class="sxs-lookup"><span data-stu-id="020dc-635">Networking</span></span>
- <span data-ttu-id="020dc-636">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="020dc-636">Storage</span></span>

<span data-ttu-id="020dc-637">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="020dc-637">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="020dc-638">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="020dc-638">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="020dc-639">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="020dc-639">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="020dc-640">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="020dc-640">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="020dc-641">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="020dc-641">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="020dc-642">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="020dc-642">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

```
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
> <span data-ttu-id="020dc-643">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="020dc-643">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="020dc-644">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="020dc-644">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="020dc-645">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="020dc-645">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="020dc-646">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="020dc-646">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="020dc-647">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="020dc-647">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="020dc-648">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="020dc-648">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="020dc-649">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="020dc-649">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="020dc-650">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="020dc-650">Provide feedback from the command line with the `az feedback` command.</span></span>

