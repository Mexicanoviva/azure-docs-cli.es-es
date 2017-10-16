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
ms.openlocfilehash: 2ea9daa558200204750f19b5d22685587ff097ef
ms.sourcegitcommit: 376bc0601aba890630dadd55908c1a65ddf40f5a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="20e65-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="20e65-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-9-2017"></a><span data-ttu-id="20e65-105">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-105">October 9, 2017</span></span>

<span data-ttu-id="20e65-106">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="20e65-106">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="20e65-107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="20e65-107">Core</span></span>

* <span data-ttu-id="20e65-108">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="20e65-108">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="20e65-109">Appservice</span><span class="sxs-lookup"><span data-stu-id="20e65-109">Appservice</span></span>

* <span data-ttu-id="20e65-110">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="20e65-110">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="20e65-111">Batch</span><span class="sxs-lookup"><span data-stu-id="20e65-111">Batch</span></span>

* <span data-ttu-id="20e65-112">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="20e65-112">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="20e65-113">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="20e65-113">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="20e65-114">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="20e65-114">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="20e65-115">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="20e65-115">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="20e65-116">Batchai</span><span class="sxs-lookup"><span data-stu-id="20e65-116">Batchai</span></span>

* <span data-ttu-id="20e65-117">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="20e65-117">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="20e65-118">Keyvault</span><span class="sxs-lookup"><span data-stu-id="20e65-118">Keyvault</span></span>

* <span data-ttu-id="20e65-119">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="20e65-119">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="20e65-120">(#4448)</span><span class="sxs-lookup"><span data-stu-id="20e65-120">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="20e65-121">Red</span><span class="sxs-lookup"><span data-stu-id="20e65-121">Network</span></span>

* <span data-ttu-id="20e65-122">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="20e65-122">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="20e65-123">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="20e65-123">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="20e65-124">Recurso</span><span class="sxs-lookup"><span data-stu-id="20e65-124">Resource</span></span>

* <span data-ttu-id="20e65-125">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="20e65-125">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="20e65-126">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="20e65-126">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="20e65-127">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="20e65-127">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="20e65-128">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="20e65-128">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="20e65-129">Sql</span><span class="sxs-lookup"><span data-stu-id="20e65-129">Sql</span></span>

* <span data-ttu-id="20e65-130">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="20e65-130">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="20e65-131">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="20e65-131">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="20e65-132">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="20e65-132">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="20e65-133">Storage</span><span class="sxs-lookup"><span data-stu-id="20e65-133">Storage</span></span>

* <span data-ttu-id="20e65-134">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="20e65-134">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-135">Vm</span><span class="sxs-lookup"><span data-stu-id="20e65-135">Vm</span></span>

* <span data-ttu-id="20e65-136">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="20e65-136">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="20e65-137">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="20e65-137">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="20e65-138">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="20e65-138">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="20e65-139">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="20e65-139">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="20e65-140">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="20e65-140">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="20e65-141">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-141">September 22, 2017</span></span>

<span data-ttu-id="20e65-142">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="20e65-142">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="20e65-143">Recurso</span><span class="sxs-lookup"><span data-stu-id="20e65-143">Resource</span></span>

* <span data-ttu-id="20e65-144">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="20e65-144">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="20e65-145">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="20e65-145">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="20e65-146">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="20e65-146">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="20e65-147">[NUEVO CAMBIO] Se cambió el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="20e65-147">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="20e65-148">Red</span><span class="sxs-lookup"><span data-stu-id="20e65-148">Network</span></span>

* <span data-ttu-id="20e65-149">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="20e65-149">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="20e65-150">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="20e65-150">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="20e65-151">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="20e65-151">Added `asg` application security group commands</span></span>
* <span data-ttu-id="20e65-152">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="20e65-152">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="20e65-153">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="20e65-153">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="20e65-154">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="20e65-154">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="20e65-155">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="20e65-155">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="20e65-156">Storage</span><span class="sxs-lookup"><span data-stu-id="20e65-156">Storage</span></span>

* <span data-ttu-id="20e65-157">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="20e65-157">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="20e65-158">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="20e65-158">Eventgrid</span></span>

* <span data-ttu-id="20e65-159">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="20e65-159">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="20e65-160">SQL</span><span class="sxs-lookup"><span data-stu-id="20e65-160">SQL</span></span>

* <span data-ttu-id="20e65-161">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="20e65-161">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="20e65-162">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="20e65-162">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="20e65-163">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="20e65-163">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="20e65-164">Keyvault</span><span class="sxs-lookup"><span data-stu-id="20e65-164">Keyvault</span></span>

* <span data-ttu-id="20e65-165">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="20e65-165">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-166">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="20e65-166">VM</span></span>

* <span data-ttu-id="20e65-167">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="20e65-167">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="20e65-168">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="20e65-168">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="20e65-169">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="20e65-169">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="20e65-170">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="20e65-170">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="20e65-171">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="20e65-171">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="20e65-172">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="20e65-172">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="20e65-173">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-173">ACS</span></span>

* <span data-ttu-id="20e65-174">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-174">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="20e65-175">Appservice</span><span class="sxs-lookup"><span data-stu-id="20e65-175">Appservice</span></span>

* <span data-ttu-id="20e65-176">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="20e65-176">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="20e65-177">Backup</span><span class="sxs-lookup"><span data-stu-id="20e65-177">Backup</span></span>

* <span data-ttu-id="20e65-178">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="20e65-178">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="20e65-179">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-179">September 11, 2017</span></span>

<span data-ttu-id="20e65-180">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="20e65-180">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="20e65-181">Núcleo</span><span class="sxs-lookup"><span data-stu-id="20e65-181">Core</span></span>

* <span data-ttu-id="20e65-182">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="20e65-182">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="20e65-183">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="20e65-183">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="20e65-184">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-184">Acs</span></span>

* <span data-ttu-id="20e65-185">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="20e65-185">Added `acs list-locations` command</span></span>
* <span data-ttu-id="20e65-186">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="20e65-186">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="20e65-187">Appservice</span><span class="sxs-lookup"><span data-stu-id="20e65-187">Appservice</span></span>

* <span data-ttu-id="20e65-188">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="20e65-188">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="20e65-189">CDN</span><span class="sxs-lookup"><span data-stu-id="20e65-189">CDN</span></span>

* <span data-ttu-id="20e65-190">Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-190">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="20e65-191">Extensión</span><span class="sxs-lookup"><span data-stu-id="20e65-191">Extension</span></span>

* <span data-ttu-id="20e65-192">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="20e65-192">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="20e65-193">Keyvault</span><span class="sxs-lookup"><span data-stu-id="20e65-193">Keyvault</span></span>

* <span data-ttu-id="20e65-194">Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="20e65-194">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="20e65-195">Red</span><span class="sxs-lookup"><span data-stu-id="20e65-195">Network</span></span>

* <span data-ttu-id="20e65-196">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="20e65-196">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="20e65-197">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-197">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="20e65-198">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-198">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="20e65-199">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-199">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="20e65-200">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-200">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="20e65-201">Recurso</span><span class="sxs-lookup"><span data-stu-id="20e65-201">Resource</span></span>

* <span data-ttu-id="20e65-202">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-202">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="20e65-203">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-203">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="20e65-204">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="20e65-204">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="20e65-205">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="20e65-205">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="20e65-206">SQL</span><span class="sxs-lookup"><span data-stu-id="20e65-206">SQL</span></span>

* <span data-ttu-id="20e65-207">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="20e65-207">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-208">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="20e65-208">VM</span></span>

* <span data-ttu-id="20e65-209">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="20e65-209">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="20e65-210">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="20e65-210">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="20e65-211">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-211">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="20e65-212">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="20e65-212">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="20e65-213">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="20e65-213">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="20e65-214">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-214">August 31, 2017</span></span>

<span data-ttu-id="20e65-215">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="20e65-215">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="20e65-216">Keyvault</span><span class="sxs-lookup"><span data-stu-id="20e65-216">Keyvault</span></span>

* <span data-ttu-id="20e65-217">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="20e65-217">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="20e65-218">Sf</span><span class="sxs-lookup"><span data-stu-id="20e65-218">Sf</span></span>

* <span data-ttu-id="20e65-219">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="20e65-219">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="20e65-220">Storage</span><span class="sxs-lookup"><span data-stu-id="20e65-220">Storage</span></span>

* <span data-ttu-id="20e65-221">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="20e65-221">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="20e65-222">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="20e65-222">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="20e65-223">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-223">August 28, 2017</span></span>

<span data-ttu-id="20e65-224">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="20e65-224">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="20e65-225">CLI</span><span class="sxs-lookup"><span data-stu-id="20e65-225">CLI</span></span>

* <span data-ttu-id="20e65-226">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="20e65-226">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="20e65-227">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-227">ACS</span></span>

* <span data-ttu-id="20e65-228">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="20e65-228">Corrected preview regions.</span></span>
* <span data-ttu-id="20e65-229">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="20e65-229">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="20e65-230">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="20e65-230">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="20e65-231">Appservice</span><span class="sxs-lookup"><span data-stu-id="20e65-231">Appservice</span></span>

* <span data-ttu-id="20e65-232">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="20e65-232">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="20e65-233">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="20e65-233">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="20e65-234">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="20e65-234">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="20e65-235">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="20e65-235">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="20e65-236">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="20e65-236">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="20e65-237">IoT</span><span class="sxs-lookup"><span data-stu-id="20e65-237">IoT</span></span>

* <span data-ttu-id="20e65-238">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="20e65-238">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="20e65-239">Red</span><span class="sxs-lookup"><span data-stu-id="20e65-239">Network</span></span>

* <span data-ttu-id="20e65-240">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="20e65-240">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="20e65-241">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="20e65-241">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="20e65-242">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="20e65-242">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="20e65-243">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-243">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="20e65-244">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-244">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="20e65-245">Perfil</span><span class="sxs-lookup"><span data-stu-id="20e65-245">Profile</span></span>

* <span data-ttu-id="20e65-246">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="20e65-246">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="20e65-247">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="20e65-247">Service Fabric</span></span>

* <span data-ttu-id="20e65-248">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="20e65-248">Preview release</span></span>
* <span data-ttu-id="20e65-249">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="20e65-249">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="20e65-250">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="20e65-250">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="20e65-251">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="20e65-251">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="20e65-252">Storage</span><span class="sxs-lookup"><span data-stu-id="20e65-252">Storage</span></span>

* <span data-ttu-id="20e65-253">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="20e65-253">Enabled setting blob tier</span></span>
* <span data-ttu-id="20e65-254">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="20e65-254">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="20e65-255">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="20e65-255">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="20e65-256">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="20e65-256">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="20e65-257">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-257">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="20e65-258">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="20e65-258">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-259">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="20e65-259">VM</span></span>

* <span data-ttu-id="20e65-260">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="20e65-260">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="20e65-261">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-261">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="20e65-262">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-262">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="20e65-263">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="20e65-263">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="20e65-264">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="20e65-264">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="20e65-265">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-265">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="20e65-266">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-266">August 15, 2017</span></span>

<span data-ttu-id="20e65-267">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="20e65-267">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="20e65-268">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-268">ACS</span></span>

* <span data-ttu-id="20e65-269">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="20e65-269">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="20e65-270">Appservice</span><span class="sxs-lookup"><span data-stu-id="20e65-270">Appservice</span></span>

* <span data-ttu-id="20e65-271">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="20e65-271">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="20e65-272">Event Grid</span><span class="sxs-lookup"><span data-stu-id="20e65-272">Event Grid</span></span>

* <span data-ttu-id="20e65-273">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="20e65-273">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="20e65-274">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-274">August 11, 2017</span></span>

<span data-ttu-id="20e65-275">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="20e65-275">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="20e65-276">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-276">ACS</span></span>

* <span data-ttu-id="20e65-277">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="20e65-277">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="20e65-278">Batch</span><span class="sxs-lookup"><span data-stu-id="20e65-278">Batch</span></span>

* <span data-ttu-id="20e65-279">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="20e65-279">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="20e65-280">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="20e65-280">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="20e65-281">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="20e65-281">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="20e65-282">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="20e65-282">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="20e65-283">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="20e65-283">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="20e65-284">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="20e65-284">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="20e65-285">Componente</span><span class="sxs-lookup"><span data-stu-id="20e65-285">Component</span></span>

* <span data-ttu-id="20e65-286">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="20e65-286">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="20e65-287">Contenedor</span><span class="sxs-lookup"><span data-stu-id="20e65-287">Container</span></span>

* <span data-ttu-id="20e65-288">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="20e65-288">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="20e65-289">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="20e65-289">Data Lake Store</span></span>

* <span data-ttu-id="20e65-290">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="20e65-290">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="20e65-291">Event Grid</span><span class="sxs-lookup"><span data-stu-id="20e65-291">Event Grid</span></span>

* <span data-ttu-id="20e65-292">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="20e65-292">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="20e65-293">Red</span><span class="sxs-lookup"><span data-stu-id="20e65-293">Network</span></span>

* <span data-ttu-id="20e65-294">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="20e65-294">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="20e65-295">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="20e65-295">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="20e65-296">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="20e65-296">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="20e65-297">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="20e65-297">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="20e65-298">Perfil</span><span class="sxs-lookup"><span data-stu-id="20e65-298">Profile</span></span>

* <span data-ttu-id="20e65-299">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="20e65-299">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="20e65-300">Storage</span><span class="sxs-lookup"><span data-stu-id="20e65-300">Storage</span></span>

* <span data-ttu-id="20e65-301">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="20e65-301">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-302">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="20e65-302">VM</span></span>

* <span data-ttu-id="20e65-303">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="20e65-303">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="20e65-304">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="20e65-304">Exposed `list-skus` command</span></span>
* <span data-ttu-id="20e65-305">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="20e65-305">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="20e65-306">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="20e65-306">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="20e65-307">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="20e65-307">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="20e65-308">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-308">July 28, 2017</span></span>

<span data-ttu-id="20e65-309">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="20e65-309">Version 2.0.12</span></span>

* <span data-ttu-id="20e65-310">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="20e65-310">Added container commands</span></span>
* <span data-ttu-id="20e65-311">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="20e65-311">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="20e65-312">Núcleo</span><span class="sxs-lookup"><span data-stu-id="20e65-312">Core</span></span>

* <span data-ttu-id="20e65-313">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="20e65-313">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="20e65-314">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="20e65-314">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="20e65-315">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="20e65-315">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="20e65-316">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="20e65-316">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="20e65-317">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="20e65-317">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="20e65-318">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="20e65-318">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="20e65-319">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="20e65-319">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="20e65-320">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="20e65-320">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="20e65-321">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="20e65-321">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="20e65-322">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="20e65-322">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="20e65-323">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="20e65-323">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="20e65-324">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="20e65-324">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="20e65-325">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="20e65-325">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="20e65-326">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="20e65-326">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="20e65-327">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="20e65-327">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="20e65-328">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="20e65-328">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="20e65-329">ACR</span><span class="sxs-lookup"><span data-stu-id="20e65-329">ACR</span></span>

* <span data-ttu-id="20e65-330">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="20e65-330">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="20e65-331">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="20e65-331">Support SKU update for managed registries</span></span>
* <span data-ttu-id="20e65-332">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="20e65-332">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="20e65-333">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="20e65-333">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="20e65-334">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="20e65-334">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="20e65-335">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="20e65-335">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="20e65-336">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-336">ACS</span></span>

* <span data-ttu-id="20e65-337">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="20e65-337">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="20e65-338">Appservice</span><span class="sxs-lookup"><span data-stu-id="20e65-338">Appservice</span></span>

* <span data-ttu-id="20e65-339">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="20e65-339">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="20e65-340">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="20e65-340">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="20e65-341">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="20e65-341">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="20e65-342">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="20e65-342">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="20e65-343">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="20e65-343">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="20e65-344">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="20e65-344">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="20e65-345">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="20e65-345">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="20e65-346">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="20e65-346">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="20e65-347">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="20e65-347">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="20e65-348">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="20e65-348">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="20e65-349">Batch</span><span class="sxs-lookup"><span data-stu-id="20e65-349">Batch</span></span>

* <span data-ttu-id="20e65-350">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="20e65-350">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="20e65-351">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="20e65-351">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="20e65-352">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-352">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="20e65-353">CDN</span><span class="sxs-lookup"><span data-stu-id="20e65-353">CDN</span></span>

* <span data-ttu-id="20e65-354">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="20e65-354">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="20e65-355">Nube</span><span class="sxs-lookup"><span data-stu-id="20e65-355">Cloud</span></span>

* <span data-ttu-id="20e65-356">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="20e65-356">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="20e65-357">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="20e65-357">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="20e65-358">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="20e65-358">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="20e65-359">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="20e65-359">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="20e65-360">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="20e65-360">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="20e65-361">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="20e65-361">CosmosDB</span></span>

* <span data-ttu-id="20e65-362">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="20e65-362">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="20e65-363">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="20e65-363">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="20e65-364">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="20e65-364">Data Lake Analytics</span></span>

* <span data-ttu-id="20e65-365">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="20e65-365">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="20e65-366">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="20e65-366">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="20e65-367">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="20e65-367">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="20e65-368">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="20e65-368">Data Lake Store</span></span>

* <span data-ttu-id="20e65-369">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-369">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="20e65-370">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="20e65-370">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="20e65-371">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="20e65-371">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="20e65-372">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="20e65-372">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="20e65-373">Interactive</span><span class="sxs-lookup"><span data-stu-id="20e65-373">Interactive</span></span>

* <span data-ttu-id="20e65-374">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="20e65-374">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="20e65-375">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="20e65-375">Increased test coverage</span></span>
* <span data-ttu-id="20e65-376">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="20e65-376">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="20e65-377">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="20e65-377">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="20e65-378">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="20e65-378">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="20e65-379">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="20e65-379">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="20e65-380">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="20e65-380">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="20e65-381">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="20e65-381">Added `--progress` flag</span></span>
* <span data-ttu-id="20e65-382">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="20e65-382">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="20e65-383">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="20e65-383">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="20e65-384">IoT</span><span class="sxs-lookup"><span data-stu-id="20e65-384">IoT</span></span>

* <span data-ttu-id="20e65-385">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="20e65-385">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="20e65-386">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="20e65-386">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="20e65-387">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="20e65-387">Key vault</span></span>

* <span data-ttu-id="20e65-388">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="20e65-388">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="20e65-389">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="20e65-389">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="20e65-390">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="20e65-390">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="20e65-391">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="20e65-391">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="20e65-392">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="20e65-392">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="20e65-393">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="20e65-393">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="20e65-394">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="20e65-394">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="20e65-395">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="20e65-395">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="20e65-396">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="20e65-396">Lab</span></span>

* <span data-ttu-id="20e65-397">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="20e65-397">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="20e65-398">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="20e65-398">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="20e65-399">Supervisión</span><span class="sxs-lookup"><span data-stu-id="20e65-399">Monitor</span></span>

* <span data-ttu-id="20e65-400">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="20e65-400">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="20e65-401">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="20e65-401">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="20e65-402">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="20e65-402">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="20e65-403">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="20e65-403">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="20e65-404">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="20e65-404">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="20e65-405">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="20e65-405">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="20e65-406">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="20e65-406">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="20e65-407">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="20e65-407">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="20e65-408">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="20e65-408">`location` no longer required</span></span>
  * <span data-ttu-id="20e65-409">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="20e65-409">Add name and ID support for target</span></span>
  * <span data-ttu-id="20e65-410">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="20e65-410">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="20e65-411">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="20e65-411">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="20e65-412">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="20e65-412">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="20e65-413">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="20e65-413">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="20e65-414">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="20e65-414">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="20e65-415">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="20e65-415">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="20e65-416">Red</span><span class="sxs-lookup"><span data-stu-id="20e65-416">Network</span></span>

* <span data-ttu-id="20e65-417">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="20e65-417">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="20e65-418">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-418">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="20e65-419">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="20e65-419">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="20e65-420">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="20e65-420">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="20e65-421">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-421">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="20e65-422">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="20e65-422">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="20e65-423">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="20e65-423">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="20e65-424">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="20e65-424">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="20e65-425">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="20e65-425">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="20e65-426">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="20e65-426">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="20e65-427">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="20e65-427">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="20e65-428">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="20e65-428">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="20e65-429">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="20e65-429">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="20e65-430">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-430">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="20e65-431">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-431">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="20e65-432">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-432">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="20e65-433">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="20e65-433">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="20e65-434">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="20e65-434">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="20e65-435">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-435">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="20e65-436">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-436">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="20e65-437">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-437">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="20e65-438">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="20e65-438">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="20e65-439">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="20e65-439">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="20e65-440">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="20e65-440">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="20e65-441">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="20e65-441">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="20e65-442">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="20e65-442">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="20e65-443">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="20e65-443">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="20e65-444">Perfil</span><span class="sxs-lookup"><span data-stu-id="20e65-444">Profile</span></span>

* <span data-ttu-id="20e65-445">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="20e65-445">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="20e65-446">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="20e65-446">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="20e65-447">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="20e65-447">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="20e65-448">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="20e65-448">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="20e65-449">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="20e65-449">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="20e65-450">RDBMS</span><span class="sxs-lookup"><span data-stu-id="20e65-450">RDBMS</span></span>

* <span data-ttu-id="20e65-451">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="20e65-451">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="20e65-452">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="20e65-452">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="20e65-453">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="20e65-453">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="20e65-454">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="20e65-454">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="20e65-455">Recurso</span><span class="sxs-lookup"><span data-stu-id="20e65-455">Resource</span></span>

* <span data-ttu-id="20e65-456">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-456">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="20e65-457">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="20e65-457">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="20e65-458">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="20e65-458">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="20e65-459">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="20e65-459">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="20e65-460">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="20e65-460">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="20e65-461">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="20e65-461">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="20e65-462">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="20e65-462">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="20e65-463">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="20e65-463">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="20e65-464">Rol</span><span class="sxs-lookup"><span data-stu-id="20e65-464">Role</span></span>

* <span data-ttu-id="20e65-465">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="20e65-465">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="20e65-466">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="20e65-466">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="20e65-467">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="20e65-467">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="20e65-468">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="20e65-468">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="20e65-469">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="20e65-469">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="20e65-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="20e65-470">Service Fabric</span></span>
* <span data-ttu-id="20e65-471">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="20e65-471">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="20e65-472">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="20e65-472">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="20e65-473">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="20e65-473">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="20e65-474">SQL</span><span class="sxs-lookup"><span data-stu-id="20e65-474">SQL</span></span>

* <span data-ttu-id="20e65-475">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="20e65-475">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="20e65-476">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="20e65-476">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="20e65-477">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="20e65-477">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="20e65-478">Storage</span><span class="sxs-lookup"><span data-stu-id="20e65-478">Storage</span></span>

* <span data-ttu-id="20e65-479">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="20e65-479">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="20e65-480">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="20e65-480">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="20e65-481">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="20e65-481">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="20e65-482">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="20e65-482">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="20e65-483">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="20e65-483">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="20e65-484">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="20e65-484">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-485">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="20e65-485">VM</span></span>

* <span data-ttu-id="20e65-486">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="20e65-486">Support configuring nsg</span></span>
* <span data-ttu-id="20e65-487">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="20e65-487">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="20e65-488">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="20e65-488">Support managed service identities</span></span>
* <span data-ttu-id="20e65-489">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="20e65-489">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="20e65-490">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="20e65-490">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="20e65-491">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-491">May 10, 2017</span></span>

<span data-ttu-id="20e65-492">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="20e65-492">Version 2.0.6</span></span>

* <span data-ttu-id="20e65-493">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="20e65-493">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="20e65-494">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="20e65-494">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="20e65-495">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="20e65-495">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="20e65-496">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="20e65-496">Include Cognitive Services module.</span></span>
* <span data-ttu-id="20e65-497">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="20e65-497">Include Service Fabric module.</span></span>
* <span data-ttu-id="20e65-498">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="20e65-498">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="20e65-499">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="20e65-499">Add support for CDN commands.</span></span>
* <span data-ttu-id="20e65-500">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="20e65-500">Remove Container module.</span></span>
* <span data-ttu-id="20e65-501">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="20e65-501">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="20e65-502">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="20e65-502">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="20e65-503">Núcleo</span><span class="sxs-lookup"><span data-stu-id="20e65-503">Core</span></span>

* <span data-ttu-id="20e65-504">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="20e65-504">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="20e65-505">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="20e65-505">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="20e65-506">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="20e65-506">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="20e65-507">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="20e65-507">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="20e65-508">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="20e65-508">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="20e65-509">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="20e65-509">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="20e65-510">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="20e65-510">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="20e65-511">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="20e65-511">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="20e65-512">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="20e65-512">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="20e65-513">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="20e65-513">core: Improved performance</span></span>
* <span data-ttu-id="20e65-514">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="20e65-514">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="20e65-515">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="20e65-515">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="20e65-516">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-516">ACS</span></span>

* <span data-ttu-id="20e65-517">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="20e65-517">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="20e65-518">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="20e65-518">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="20e65-519">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="20e65-519">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="20e65-520">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="20e65-520">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="20e65-521">AppService</span><span class="sxs-lookup"><span data-stu-id="20e65-521">AppService</span></span>

* <span data-ttu-id="20e65-522">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="20e65-522">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="20e65-523">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="20e65-523">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="20e65-524">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="20e65-524">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="20e65-525">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="20e65-525">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="20e65-526">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="20e65-526">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="20e65-527">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="20e65-527">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="20e65-528">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="20e65-528">support slot swap with preview</span></span>
* <span data-ttu-id="20e65-529">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="20e65-529">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="20e65-530">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="20e65-530">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="20e65-531">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="20e65-531">CosmosDB</span></span>

* <span data-ttu-id="20e65-532">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="20e65-532">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="20e65-533">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="20e65-533">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="20e65-534">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="20e65-534">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="20e65-535">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="20e65-535">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="20e65-536">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="20e65-536">Data Lake Analytics</span></span>

* <span data-ttu-id="20e65-537">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="20e65-537">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="20e65-538">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="20e65-538">Add support for new catalog item type: package.</span></span> <span data-ttu-id="20e65-539">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="20e65-539">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="20e65-540">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="20e65-540">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="20e65-541">Tabla</span><span class="sxs-lookup"><span data-stu-id="20e65-541">Table</span></span>
  * <span data-ttu-id="20e65-542">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="20e65-542">Table valued function</span></span>
  * <span data-ttu-id="20e65-543">Ver</span><span class="sxs-lookup"><span data-stu-id="20e65-543">View</span></span>
  * <span data-ttu-id="20e65-544">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="20e65-544">Table Statistics.</span></span> <span data-ttu-id="20e65-545">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="20e65-545">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="20e65-546">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="20e65-546">Data Lake Store</span></span>

* <span data-ttu-id="20e65-547">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="20e65-547">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="20e65-548">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="20e65-548">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="20e65-549">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="20e65-549">missed help for access show.</span></span> <span data-ttu-id="20e65-550">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="20e65-550">adding it.</span></span> <span data-ttu-id="20e65-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="20e65-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="20e65-552">Buscar</span><span class="sxs-lookup"><span data-stu-id="20e65-552">Find</span></span>

* <span data-ttu-id="20e65-553">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="20e65-553">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="20e65-554">KeyVault</span><span class="sxs-lookup"><span data-stu-id="20e65-554">KeyVault</span></span>

* <span data-ttu-id="20e65-555">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="20e65-555">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="20e65-556">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="20e65-556">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="20e65-557">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="20e65-557">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="20e65-558">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="20e65-558">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="20e65-559">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="20e65-559">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="20e65-560">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="20e65-560">Lab</span></span>

* <span data-ttu-id="20e65-561">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="20e65-561">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="20e65-562">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="20e65-562">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="20e65-563">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="20e65-563">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="20e65-564">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="20e65-564">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="20e65-565">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="20e65-565">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="20e65-566">Supervisión</span><span class="sxs-lookup"><span data-stu-id="20e65-566">Monitor</span></span>

* <span data-ttu-id="20e65-567">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="20e65-567">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="20e65-568">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="20e65-568">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="20e65-569">Red</span><span class="sxs-lookup"><span data-stu-id="20e65-569">Network</span></span>

* <span data-ttu-id="20e65-570">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="20e65-570">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="20e65-571">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="20e65-571">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="20e65-572">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="20e65-572">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="20e65-573">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="20e65-573">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="20e65-574">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="20e65-574">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="20e65-575">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="20e65-575">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="20e65-576">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="20e65-576">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="20e65-577">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="20e65-577">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="20e65-578">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="20e65-578">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="20e65-579">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="20e65-579">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="20e65-580">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="20e65-580">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="20e65-581">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="20e65-581">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="20e65-582">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="20e65-582">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="20e65-583">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="20e65-583">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="20e65-584">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="20e65-584">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="20e65-585">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="20e65-585">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="20e65-586">Perfil</span><span class="sxs-lookup"><span data-stu-id="20e65-586">Profile</span></span>

* <span data-ttu-id="20e65-587">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="20e65-587">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="20e65-588">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="20e65-588">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="20e65-589">Redis</span><span class="sxs-lookup"><span data-stu-id="20e65-589">Redis</span></span>

* <span data-ttu-id="20e65-590">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="20e65-590">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="20e65-591">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="20e65-591">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="20e65-592">Recurso</span><span class="sxs-lookup"><span data-stu-id="20e65-592">Resource</span></span>

* <span data-ttu-id="20e65-593">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="20e65-593">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="20e65-594">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="20e65-594">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="20e65-595">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="20e65-595">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="20e65-596">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="20e65-596">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="20e65-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="20e65-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="20e65-598">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="20e65-598">Add docs for az lock update.</span></span> <span data-ttu-id="20e65-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="20e65-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="20e65-600">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="20e65-600">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="20e65-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="20e65-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="20e65-602">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="20e65-602">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="20e65-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="20e65-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="20e65-604">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="20e65-604">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="20e65-605">Rol</span><span class="sxs-lookup"><span data-stu-id="20e65-605">Role</span></span>

* <span data-ttu-id="20e65-606">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="20e65-606">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="20e65-607">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="20e65-607">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="20e65-608">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="20e65-608">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="20e65-609">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="20e65-609">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="20e65-610">SQL</span><span class="sxs-lookup"><span data-stu-id="20e65-610">SQL</span></span>

* <span data-ttu-id="20e65-611">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="20e65-611">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="20e65-612">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="20e65-612">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="20e65-613">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="20e65-613">Storage</span></span>

* <span data-ttu-id="20e65-614">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="20e65-614">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="20e65-615">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="20e65-615">Add support for incremental blob copy</span></span>
* <span data-ttu-id="20e65-616">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="20e65-616">Add support for large block blob upload</span></span>
* <span data-ttu-id="20e65-617">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="20e65-617">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-618">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="20e65-618">VM</span></span>

* <span data-ttu-id="20e65-619">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="20e65-619">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="20e65-620">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="20e65-620">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="20e65-621">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="20e65-621">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="20e65-622">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="20e65-622">az vm/vmss disk</span></span>
  3. <span data-ttu-id="20e65-623">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="20e65-623">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="20e65-624">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="20e65-624">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="20e65-625">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="20e65-625">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="20e65-626">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-626">April 3, 2017</span></span>

<span data-ttu-id="20e65-627">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="20e65-627">Version 2.0.2</span></span>

<span data-ttu-id="20e65-628">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="20e65-628">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="20e65-629">Núcleo</span><span class="sxs-lookup"><span data-stu-id="20e65-629">Core</span></span>

* <span data-ttu-id="20e65-630">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="20e65-630">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="20e65-631">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="20e65-631">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="20e65-632">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="20e65-632">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="20e65-633">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="20e65-633">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="20e65-634">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="20e65-634">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="20e65-635">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="20e65-635">Add prompting for missing template parameters.</span></span> <span data-ttu-id="20e65-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="20e65-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="20e65-637">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="20e65-637">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="20e65-638">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="20e65-638">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="20e65-639">ACS</span><span class="sxs-lookup"><span data-stu-id="20e65-639">ACS</span></span>

* <span data-ttu-id="20e65-640">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="20e65-640">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="20e65-641">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="20e65-641">Add support for ssh key password prompting.</span></span> <span data-ttu-id="20e65-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="20e65-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="20e65-643">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="20e65-643">Add support for windows clusters.</span></span> <span data-ttu-id="20e65-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="20e65-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="20e65-645">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="20e65-645">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="20e65-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="20e65-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="20e65-647">AppService</span><span class="sxs-lookup"><span data-stu-id="20e65-647">AppService</span></span>

* <span data-ttu-id="20e65-648">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="20e65-648">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="20e65-649">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="20e65-649">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="20e65-650">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="20e65-650">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="20e65-651">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="20e65-651">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="20e65-652">DataLake</span><span class="sxs-lookup"><span data-stu-id="20e65-652">DataLake</span></span>

* <span data-ttu-id="20e65-653">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="20e65-653">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="20e65-654">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="20e65-654">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="20e65-655">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="20e65-655">DocuemntDB</span></span>

* <span data-ttu-id="20e65-656">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="20e65-656">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="20e65-657">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="20e65-657">VM</span></span>

* <span data-ttu-id="20e65-658">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="20e65-658">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="20e65-659">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="20e65-659">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="20e65-660">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="20e65-660">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="20e65-661">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="20e65-661">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="20e65-662">Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="20e65-662">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="20e65-663">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="20e65-663">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="20e65-664">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="20e65-664">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="20e65-665">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="20e65-665">February 27, 2017</span></span>

<span data-ttu-id="20e65-666">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="20e65-666">Version 2.0.0</span></span>

<span data-ttu-id="20e65-667">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="20e65-667">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="20e65-668">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="20e65-668">General availability applies to these command modules:</span></span>
- <span data-ttu-id="20e65-669">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="20e65-669">Container Service (acs)</span></span>
- <span data-ttu-id="20e65-670">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="20e65-670">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="20e65-671">Redes</span><span class="sxs-lookup"><span data-stu-id="20e65-671">Networking</span></span>
- <span data-ttu-id="20e65-672">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="20e65-672">Storage</span></span>

<span data-ttu-id="20e65-673">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e65-673">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="20e65-674">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="20e65-674">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="20e65-675">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="20e65-675">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="20e65-676">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="20e65-676">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="20e65-677">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="20e65-677">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="20e65-678">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="20e65-678">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="20e65-679">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="20e65-679">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="20e65-680">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="20e65-680">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="20e65-681">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="20e65-681">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="20e65-682">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="20e65-682">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="20e65-683">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="20e65-683">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="20e65-684">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="20e65-684">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="20e65-685">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="20e65-685">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="20e65-686">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="20e65-686">Provide feedback from the command line with the `az feedback` command.</span></span>

