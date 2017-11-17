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
ms.openlocfilehash: 429b099dabd27d9356e88791f955ec52acd2a5f9
ms.sourcegitcommit: 9b36c15dc0e10024e23b8018604f5ef63c025de1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/24/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="5f12f-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5f12f-105">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-105">October 24, 2017</span></span>

<span data-ttu-id="5f12f-106">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5f12f-106">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f12f-107">Core</span></span>

* <span data-ttu-id="5f12f-108">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="5f12f-108">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-109">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-109">ACR</span></span>

* <span data-ttu-id="5f12f-110">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="5f12f-110">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5f12f-111">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="5f12f-111">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5f12f-112">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="5f12f-112">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-113">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-113">ACS</span></span>

* <span data-ttu-id="5f12f-114">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="5f12f-114">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5f12f-115">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5f12f-115">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-116">Appservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-116">Appservice</span></span>

* <span data-ttu-id="5f12f-117">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="5f12f-117">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5f12f-118">Componente</span><span class="sxs-lookup"><span data-stu-id="5f12f-118">Component</span></span>

* <span data-ttu-id="5f12f-119">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="5f12f-119">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-120">Supervisión</span><span class="sxs-lookup"><span data-stu-id="5f12f-120">Monitor</span></span>

* <span data-ttu-id="5f12f-121">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-121">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-122">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-122">Resource</span></span>

* <span data-ttu-id="5f12f-123">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="5f12f-123">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5f12f-124">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="5f12f-124">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-125">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-125">VM</span></span>

* <span data-ttu-id="5f12f-126">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-126">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5f12f-127">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-127">October 9, 2017</span></span>

<span data-ttu-id="5f12f-128">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5f12f-128">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-129">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f12f-129">Core</span></span>

* <span data-ttu-id="5f12f-130">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5f12f-130">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-131">Appservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-131">Appservice</span></span>

* <span data-ttu-id="5f12f-132">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="5f12f-132">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-133">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-133">Batch</span></span>

* <span data-ttu-id="5f12f-134">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-134">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5f12f-135">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="5f12f-135">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5f12f-136">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-136">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5f12f-137">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="5f12f-137">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5f12f-138">Batchai</span><span class="sxs-lookup"><span data-stu-id="5f12f-138">Batchai</span></span>

* <span data-ttu-id="5f12f-139">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-139">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-140">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f12f-140">Keyvault</span></span>

* <span data-ttu-id="5f12f-141">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5f12f-141">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5f12f-142">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5f12f-142">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5f12f-143">Red</span><span class="sxs-lookup"><span data-stu-id="5f12f-143">Network</span></span>

* <span data-ttu-id="5f12f-144">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="5f12f-144">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5f12f-145">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="5f12f-145">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-146">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-146">Resource</span></span>

* <span data-ttu-id="5f12f-147">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-147">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5f12f-148">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="5f12f-148">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5f12f-149">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="5f12f-149">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5f12f-150">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-150">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-151">Sql</span><span class="sxs-lookup"><span data-stu-id="5f12f-151">Sql</span></span>

* <span data-ttu-id="5f12f-152">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="5f12f-152">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5f12f-153">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="5f12f-153">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5f12f-154">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="5f12f-154">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-155">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-155">Storage</span></span>

* <span data-ttu-id="5f12f-156">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="5f12f-156">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-157">Vm</span><span class="sxs-lookup"><span data-stu-id="5f12f-157">Vm</span></span>

* <span data-ttu-id="5f12f-158">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="5f12f-158">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5f12f-159">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-159">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5f12f-160">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5f12f-160">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5f12f-161">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-161">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5f12f-162">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-162">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5f12f-163">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-163">September 22, 2017</span></span>

<span data-ttu-id="5f12f-164">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="5f12f-164">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-165">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-165">Resource</span></span>

* <span data-ttu-id="5f12f-166">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="5f12f-166">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5f12f-167">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="5f12f-167">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5f12f-168">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-168">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5f12f-169">[NUEVO CAMBIO] Se cambió el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="5f12f-169">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-170">Red</span><span class="sxs-lookup"><span data-stu-id="5f12f-170">Network</span></span>

* <span data-ttu-id="5f12f-171">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="5f12f-171">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5f12f-172">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="5f12f-172">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5f12f-173">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="5f12f-173">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5f12f-174">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="5f12f-174">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5f12f-175">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f12f-175">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f12f-176">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f12f-176">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5f12f-177">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-177">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-178">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-178">Storage</span></span>

* <span data-ttu-id="5f12f-179">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="5f12f-179">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f12f-180">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="5f12f-180">Eventgrid</span></span>

* <span data-ttu-id="5f12f-181">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="5f12f-181">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-182">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-182">SQL</span></span>

* <span data-ttu-id="5f12f-183">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="5f12f-183">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5f12f-184">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="5f12f-184">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5f12f-185">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f12f-185">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-186">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f12f-186">Keyvault</span></span>

* <span data-ttu-id="5f12f-187">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="5f12f-187">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-188">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-188">VM</span></span>

* <span data-ttu-id="5f12f-189">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-189">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5f12f-190">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="5f12f-190">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5f12f-191">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-191">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5f12f-192">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="5f12f-192">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5f12f-193">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="5f12f-193">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5f12f-194">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="5f12f-194">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-195">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-195">ACS</span></span>

* <span data-ttu-id="5f12f-196">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-196">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-197">Appservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-197">Appservice</span></span>

* <span data-ttu-id="5f12f-198">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="5f12f-198">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-199">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-199">Backup</span></span>

* <span data-ttu-id="5f12f-200">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="5f12f-200">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5f12f-201">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-201">September 11, 2017</span></span>

<span data-ttu-id="5f12f-202">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5f12f-202">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-203">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f12f-203">Core</span></span>

* <span data-ttu-id="5f12f-204">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="5f12f-204">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5f12f-205">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="5f12f-205">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-206">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-206">Acs</span></span>

* <span data-ttu-id="5f12f-207">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-207">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5f12f-208">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="5f12f-208">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-209">Appservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-209">Appservice</span></span>

* <span data-ttu-id="5f12f-210">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="5f12f-210">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-211">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-211">CDN</span></span>

* <span data-ttu-id="5f12f-212">Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-212">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-213">Extensión</span><span class="sxs-lookup"><span data-stu-id="5f12f-213">Extension</span></span>

* <span data-ttu-id="5f12f-214">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="5f12f-214">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-215">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f12f-215">Keyvault</span></span>

* <span data-ttu-id="5f12f-216">Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-216">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-217">Red</span><span class="sxs-lookup"><span data-stu-id="5f12f-217">Network</span></span>

* <span data-ttu-id="5f12f-218">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-218">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f12f-219">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-219">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5f12f-220">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-220">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5f12f-221">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f12f-222">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-222">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-223">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-223">Resource</span></span>

* <span data-ttu-id="5f12f-224">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-224">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5f12f-225">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-225">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5f12f-226">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="5f12f-226">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5f12f-227">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="5f12f-227">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-228">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-228">SQL</span></span>

* <span data-ttu-id="5f12f-229">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-229">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-230">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-230">VM</span></span>

* <span data-ttu-id="5f12f-231">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-231">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5f12f-232">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="5f12f-232">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5f12f-233">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-233">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5f12f-234">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-234">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5f12f-235">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="5f12f-235">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5f12f-236">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-236">August 31, 2017</span></span>

<span data-ttu-id="5f12f-237">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5f12f-237">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-238">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f12f-238">Keyvault</span></span>

* <span data-ttu-id="5f12f-239">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-239">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5f12f-240">Sf</span><span class="sxs-lookup"><span data-stu-id="5f12f-240">Sf</span></span>

* <span data-ttu-id="5f12f-241">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="5f12f-241">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-242">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-242">Storage</span></span>

* <span data-ttu-id="5f12f-243">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="5f12f-243">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5f12f-244">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="5f12f-244">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5f12f-245">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-245">August 28, 2017</span></span>

<span data-ttu-id="5f12f-246">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5f12f-246">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5f12f-247">CLI</span><span class="sxs-lookup"><span data-stu-id="5f12f-247">CLI</span></span>

* <span data-ttu-id="5f12f-248">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-248">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-249">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-249">ACS</span></span>

* <span data-ttu-id="5f12f-250">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="5f12f-250">Corrected preview regions.</span></span>
* <span data-ttu-id="5f12f-251">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="5f12f-251">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="5f12f-252">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="5f12f-252">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-253">Appservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-253">Appservice</span></span>

* <span data-ttu-id="5f12f-254">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-254">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5f12f-255">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-255">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5f12f-256">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-256">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5f12f-257">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="5f12f-257">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5f12f-258">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="5f12f-258">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-259">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-259">IoT</span></span>

* <span data-ttu-id="5f12f-260">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="5f12f-260">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-261">Red</span><span class="sxs-lookup"><span data-stu-id="5f12f-261">Network</span></span>

* <span data-ttu-id="5f12f-262">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-262">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f12f-263">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-263">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5f12f-264">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-264">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f12f-265">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-265">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f12f-266">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-266">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-267">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f12f-267">Profile</span></span>

* <span data-ttu-id="5f12f-268">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="5f12f-268">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f12f-269">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-269">Service Fabric</span></span>

* <span data-ttu-id="5f12f-270">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="5f12f-270">Preview release</span></span>
* <span data-ttu-id="5f12f-271">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="5f12f-271">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5f12f-272">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="5f12f-272">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5f12f-273">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-273">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-274">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-274">Storage</span></span>

* <span data-ttu-id="5f12f-275">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="5f12f-275">Enabled setting blob tier</span></span>
* <span data-ttu-id="5f12f-276">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="5f12f-276">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5f12f-277">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-277">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="5f12f-278">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="5f12f-278">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5f12f-279">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-279">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5f12f-280">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="5f12f-280">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-281">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-281">VM</span></span>

* <span data-ttu-id="5f12f-282">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-282">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5f12f-283">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-283">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="5f12f-284">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-284">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="5f12f-285">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-285">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5f12f-286">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="5f12f-286">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5f12f-287">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-287">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5f12f-288">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-288">August 15, 2017</span></span>

<span data-ttu-id="5f12f-289">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5f12f-289">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-290">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-290">ACS</span></span>

* <span data-ttu-id="5f12f-291">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5f12f-291">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-292">Appservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-292">Appservice</span></span>

* <span data-ttu-id="5f12f-293">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="5f12f-293">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f12f-294">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5f12f-294">Event Grid</span></span>

* <span data-ttu-id="5f12f-295">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="5f12f-295">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5f12f-296">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-296">August 11, 2017</span></span>

<span data-ttu-id="5f12f-297">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5f12f-297">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-298">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-298">ACS</span></span>

* <span data-ttu-id="5f12f-299">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="5f12f-299">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-300">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-300">Batch</span></span>

* <span data-ttu-id="5f12f-301">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="5f12f-301">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5f12f-302">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="5f12f-302">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5f12f-303">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="5f12f-303">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5f12f-304">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="5f12f-304">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5f12f-305">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="5f12f-305">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5f12f-306">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="5f12f-306">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5f12f-307">Componente</span><span class="sxs-lookup"><span data-stu-id="5f12f-307">Component</span></span>

* <span data-ttu-id="5f12f-308">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="5f12f-308">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-309">Contenedor</span><span class="sxs-lookup"><span data-stu-id="5f12f-309">Container</span></span>

* <span data-ttu-id="5f12f-310">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="5f12f-310">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5f12f-311">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f12f-311">Data Lake Store</span></span>

* <span data-ttu-id="5f12f-312">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="5f12f-312">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f12f-313">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5f12f-313">Event Grid</span></span>

* <span data-ttu-id="5f12f-314">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="5f12f-314">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-315">Red</span><span class="sxs-lookup"><span data-stu-id="5f12f-315">Network</span></span>

* <span data-ttu-id="5f12f-316">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="5f12f-316">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5f12f-317">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-317">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5f12f-318">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="5f12f-318">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5f12f-319">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-319">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-320">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f12f-320">Profile</span></span>

* <span data-ttu-id="5f12f-321">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="5f12f-321">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-322">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-322">Storage</span></span>

* <span data-ttu-id="5f12f-323">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="5f12f-323">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-324">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-324">VM</span></span>

* <span data-ttu-id="5f12f-325">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="5f12f-325">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5f12f-326">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-326">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5f12f-327">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="5f12f-327">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5f12f-328">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="5f12f-328">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5f12f-329">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="5f12f-329">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5f12f-330">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-330">July 28, 2017</span></span>

<span data-ttu-id="5f12f-331">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5f12f-331">Version 2.0.12</span></span>

* <span data-ttu-id="5f12f-332">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="5f12f-332">Added container commands</span></span>
* <span data-ttu-id="5f12f-333">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="5f12f-333">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="5f12f-334">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f12f-334">Core</span></span>

* <span data-ttu-id="5f12f-335">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="5f12f-335">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5f12f-336">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="5f12f-336">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5f12f-337">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="5f12f-337">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5f12f-338">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="5f12f-338">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5f12f-339">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="5f12f-339">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5f12f-340">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="5f12f-340">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5f12f-341">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="5f12f-341">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f12f-342">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="5f12f-342">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5f12f-343">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="5f12f-343">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5f12f-344">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="5f12f-344">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5f12f-345">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="5f12f-345">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5f12f-346">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="5f12f-346">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5f12f-347">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5f12f-347">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5f12f-348">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5f12f-348">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5f12f-349">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5f12f-349">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5f12f-350">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="5f12f-350">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-351">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-351">ACR</span></span>

* <span data-ttu-id="5f12f-352">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="5f12f-352">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5f12f-353">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="5f12f-353">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5f12f-354">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="5f12f-354">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5f12f-355">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="5f12f-355">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5f12f-356">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="5f12f-356">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5f12f-357">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="5f12f-357">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-358">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-358">ACS</span></span>

* <span data-ttu-id="5f12f-359">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="5f12f-359">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-360">Appservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-360">Appservice</span></span>

* <span data-ttu-id="5f12f-361">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="5f12f-361">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5f12f-362">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="5f12f-362">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5f12f-363">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-363">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5f12f-364">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="5f12f-364">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5f12f-365">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="5f12f-365">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5f12f-366">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="5f12f-366">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5f12f-367">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="5f12f-367">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5f12f-368">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="5f12f-368">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5f12f-369">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="5f12f-369">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5f12f-370">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="5f12f-370">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-371">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-371">Batch</span></span>

* <span data-ttu-id="5f12f-372">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="5f12f-372">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5f12f-373">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-373">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5f12f-374">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-374">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-375">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-375">CDN</span></span>

* <span data-ttu-id="5f12f-376">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="5f12f-376">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="5f12f-377">Nube</span><span class="sxs-lookup"><span data-stu-id="5f12f-377">Cloud</span></span>

* <span data-ttu-id="5f12f-378">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="5f12f-378">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5f12f-379">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="5f12f-379">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5f12f-380">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="5f12f-380">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5f12f-381">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="5f12f-381">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5f12f-382">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-382">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-383">CosmosDB</span></span>

* <span data-ttu-id="5f12f-384">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="5f12f-384">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5f12f-385">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="5f12f-385">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f12f-386">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f12f-386">Data Lake Analytics</span></span>

* <span data-ttu-id="5f12f-387">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-387">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5f12f-388">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-388">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5f12f-389">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-389">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f12f-390">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f12f-390">Data Lake Store</span></span>

* <span data-ttu-id="5f12f-391">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-391">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5f12f-392">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="5f12f-392">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5f12f-393">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-393">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5f12f-394">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5f12f-394">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-395">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-395">Interactive</span></span>

* <span data-ttu-id="5f12f-396">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="5f12f-396">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5f12f-397">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="5f12f-397">Increased test coverage</span></span>
* <span data-ttu-id="5f12f-398">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="5f12f-398">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5f12f-399">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="5f12f-399">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5f12f-400">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="5f12f-400">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5f12f-401">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="5f12f-401">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5f12f-402">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="5f12f-402">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f12f-403">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-403">Added `--progress` flag</span></span>
* <span data-ttu-id="5f12f-404">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="5f12f-404">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5f12f-405">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="5f12f-405">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-406">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-406">IoT</span></span>

* <span data-ttu-id="5f12f-407">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="5f12f-407">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5f12f-408">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="5f12f-408">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-409">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="5f12f-409">Key vault</span></span>

* <span data-ttu-id="5f12f-410">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="5f12f-410">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5f12f-411">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-411">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5f12f-412">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-412">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f12f-413">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-413">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f12f-414">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-414">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5f12f-415">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="5f12f-415">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5f12f-416">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="5f12f-416">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5f12f-417">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="5f12f-417">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5f12f-418">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="5f12f-418">Lab</span></span>

* <span data-ttu-id="5f12f-419">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-419">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5f12f-420">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-420">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-421">Supervisión</span><span class="sxs-lookup"><span data-stu-id="5f12f-421">Monitor</span></span>

* <span data-ttu-id="5f12f-422">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="5f12f-422">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5f12f-423">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-423">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5f12f-424">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-424">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5f12f-425">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-425">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5f12f-426">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-426">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5f12f-427">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="5f12f-427">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5f12f-428">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="5f12f-428">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5f12f-429">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="5f12f-429">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5f12f-430">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="5f12f-430">`location` no longer required</span></span>
  * <span data-ttu-id="5f12f-431">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="5f12f-431">Add name and ID support for target</span></span>
  * <span data-ttu-id="5f12f-432">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-432">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5f12f-433">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="5f12f-433">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5f12f-434">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="5f12f-434">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5f12f-435">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="5f12f-435">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5f12f-436">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-436">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5f12f-437">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="5f12f-437">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-438">Red</span><span class="sxs-lookup"><span data-stu-id="5f12f-438">Network</span></span>

* <span data-ttu-id="5f12f-439">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-439">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5f12f-440">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-440">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5f12f-441">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="5f12f-441">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5f12f-442">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="5f12f-442">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5f12f-443">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-443">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5f12f-444">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-444">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5f12f-445">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="5f12f-445">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5f12f-446">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="5f12f-446">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5f12f-447">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="5f12f-447">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5f12f-448">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5f12f-448">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5f12f-449">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-449">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5f12f-450">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-450">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5f12f-451">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="5f12f-451">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5f12f-452">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-452">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5f12f-453">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-453">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5f12f-454">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-454">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5f12f-455">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="5f12f-455">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5f12f-456">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-456">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5f12f-457">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-457">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5f12f-458">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-458">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5f12f-459">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-459">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5f12f-460">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-460">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5f12f-461">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-461">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5f12f-462">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="5f12f-462">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5f12f-463">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="5f12f-463">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5f12f-464">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="5f12f-464">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5f12f-465">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="5f12f-465">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-466">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f12f-466">Profile</span></span>

* <span data-ttu-id="5f12f-467">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="5f12f-467">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5f12f-468">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="5f12f-468">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5f12f-469">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="5f12f-469">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5f12f-470">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="5f12f-470">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5f12f-471">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="5f12f-471">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-472">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-472">RDBMS</span></span>

* <span data-ttu-id="5f12f-473">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="5f12f-473">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5f12f-474">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="5f12f-474">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5f12f-475">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="5f12f-475">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5f12f-476">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="5f12f-476">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-477">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-477">Resource</span></span>

* <span data-ttu-id="5f12f-478">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-478">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5f12f-479">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-479">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5f12f-480">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-480">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5f12f-481">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-481">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5f12f-482">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="5f12f-482">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5f12f-483">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-483">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5f12f-484">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="5f12f-484">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5f12f-485">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-485">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-486">Rol</span><span class="sxs-lookup"><span data-stu-id="5f12f-486">Role</span></span>

* <span data-ttu-id="5f12f-487">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="5f12f-487">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5f12f-488">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="5f12f-488">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5f12f-489">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-489">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5f12f-490">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-490">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5f12f-491">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-491">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f12f-492">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-492">Service Fabric</span></span>
* <span data-ttu-id="5f12f-493">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="5f12f-493">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5f12f-494">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="5f12f-494">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5f12f-495">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="5f12f-495">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-496">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-496">SQL</span></span>

* <span data-ttu-id="5f12f-497">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="5f12f-497">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5f12f-498">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-498">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5f12f-499">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-499">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-500">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-500">Storage</span></span>

* <span data-ttu-id="5f12f-501">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="5f12f-501">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5f12f-502">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="5f12f-502">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5f12f-503">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="5f12f-503">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5f12f-504">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="5f12f-504">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="5f12f-505">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="5f12f-505">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="5f12f-506">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="5f12f-506">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-507">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-507">VM</span></span>

* <span data-ttu-id="5f12f-508">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="5f12f-508">Support configuring nsg</span></span>
* <span data-ttu-id="5f12f-509">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="5f12f-509">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5f12f-510">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="5f12f-510">Support managed service identities</span></span>
* <span data-ttu-id="5f12f-511">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-511">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="5f12f-512">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="5f12f-512">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5f12f-513">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-513">May 10, 2017</span></span>

<span data-ttu-id="5f12f-514">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5f12f-514">Version 2.0.6</span></span>

* <span data-ttu-id="5f12f-515">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="5f12f-515">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5f12f-516">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="5f12f-516">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5f12f-517">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5f12f-517">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="5f12f-518">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5f12f-518">Include Cognitive Services module.</span></span>
* <span data-ttu-id="5f12f-519">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="5f12f-519">Include Service Fabric module.</span></span>
* <span data-ttu-id="5f12f-520">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="5f12f-520">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="5f12f-521">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="5f12f-521">Add support for CDN commands.</span></span>
* <span data-ttu-id="5f12f-522">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="5f12f-522">Remove Container module.</span></span>
* <span data-ttu-id="5f12f-523">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="5f12f-523">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5f12f-524">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5f12f-524">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="5f12f-525">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f12f-525">Core</span></span>

* <span data-ttu-id="5f12f-526">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="5f12f-526">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="5f12f-527">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="5f12f-527">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5f12f-528">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="5f12f-528">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5f12f-529">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="5f12f-529">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5f12f-530">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="5f12f-530">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5f12f-531">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="5f12f-531">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5f12f-532">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="5f12f-532">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5f12f-533">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="5f12f-533">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5f12f-534">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="5f12f-534">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5f12f-535">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="5f12f-535">core: Improved performance</span></span>
* <span data-ttu-id="5f12f-536">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="5f12f-536">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5f12f-537">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="5f12f-537">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-538">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-538">ACS</span></span>

* <span data-ttu-id="5f12f-539">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="5f12f-539">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5f12f-540">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="5f12f-540">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5f12f-541">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="5f12f-541">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5f12f-542">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="5f12f-542">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-543">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-543">AppService</span></span>

* <span data-ttu-id="5f12f-544">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="5f12f-544">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5f12f-545">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="5f12f-545">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5f12f-546">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="5f12f-546">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5f12f-547">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="5f12f-547">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5f12f-548">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="5f12f-548">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5f12f-549">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="5f12f-549">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5f12f-550">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="5f12f-550">support slot swap with preview</span></span>
* <span data-ttu-id="5f12f-551">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="5f12f-551">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5f12f-552">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="5f12f-552">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-553">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-553">CosmosDB</span></span>

* <span data-ttu-id="5f12f-554">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-554">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="5f12f-555">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="5f12f-555">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5f12f-556">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="5f12f-556">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5f12f-557">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="5f12f-557">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f12f-558">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f12f-558">Data Lake Analytics</span></span>

* <span data-ttu-id="5f12f-559">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="5f12f-559">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="5f12f-560">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="5f12f-560">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5f12f-561">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="5f12f-561">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5f12f-562">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="5f12f-562">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5f12f-563">Tabla</span><span class="sxs-lookup"><span data-stu-id="5f12f-563">Table</span></span>
  * <span data-ttu-id="5f12f-564">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="5f12f-564">Table valued function</span></span>
  * <span data-ttu-id="5f12f-565">Ver</span><span class="sxs-lookup"><span data-stu-id="5f12f-565">View</span></span>
  * <span data-ttu-id="5f12f-566">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="5f12f-566">Table Statistics.</span></span> <span data-ttu-id="5f12f-567">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="5f12f-567">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f12f-568">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f12f-568">Data Lake Store</span></span>

* <span data-ttu-id="5f12f-569">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="5f12f-569">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="5f12f-570">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5f12f-570">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5f12f-571">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="5f12f-571">missed help for access show.</span></span> <span data-ttu-id="5f12f-572">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="5f12f-572">adding it.</span></span> <span data-ttu-id="5f12f-573">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5f12f-573">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5f12f-574">Buscar</span><span class="sxs-lookup"><span data-stu-id="5f12f-574">Find</span></span>

* <span data-ttu-id="5f12f-575">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="5f12f-575">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-576">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-576">KeyVault</span></span>

* <span data-ttu-id="5f12f-577">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="5f12f-577">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5f12f-578">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="5f12f-578">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="5f12f-579">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="5f12f-579">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5f12f-580">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="5f12f-580">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="5f12f-581">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="5f12f-581">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5f12f-582">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="5f12f-582">Lab</span></span>

* <span data-ttu-id="5f12f-583">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="5f12f-583">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="5f12f-584">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="5f12f-584">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="5f12f-585">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="5f12f-585">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="5f12f-586">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="5f12f-586">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="5f12f-587">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="5f12f-587">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-588">Supervisión</span><span class="sxs-lookup"><span data-stu-id="5f12f-588">Monitor</span></span>

* <span data-ttu-id="5f12f-589">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="5f12f-589">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5f12f-590">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="5f12f-590">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-591">Red</span><span class="sxs-lookup"><span data-stu-id="5f12f-591">Network</span></span>

* <span data-ttu-id="5f12f-592">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="5f12f-592">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="5f12f-593">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-593">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="5f12f-594">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="5f12f-594">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="5f12f-595">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="5f12f-595">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="5f12f-596">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="5f12f-596">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="5f12f-597">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5f12f-597">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="5f12f-598">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="5f12f-598">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="5f12f-599">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="5f12f-599">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="5f12f-600">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="5f12f-600">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="5f12f-601">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="5f12f-601">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5f12f-602">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="5f12f-602">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="5f12f-603">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-603">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="5f12f-604">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="5f12f-604">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="5f12f-605">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="5f12f-605">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="5f12f-606">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="5f12f-606">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="5f12f-607">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="5f12f-607">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-608">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f12f-608">Profile</span></span>

* <span data-ttu-id="5f12f-609">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="5f12f-609">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5f12f-610">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="5f12f-610">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5f12f-611">Redis</span><span class="sxs-lookup"><span data-stu-id="5f12f-611">Redis</span></span>

* <span data-ttu-id="5f12f-612">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="5f12f-612">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5f12f-613">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="5f12f-613">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-614">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f12f-614">Resource</span></span>

* <span data-ttu-id="5f12f-615">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="5f12f-615">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5f12f-616">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="5f12f-616">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5f12f-617">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="5f12f-617">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5f12f-618">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="5f12f-618">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5f12f-619">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5f12f-619">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5f12f-620">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="5f12f-620">Add docs for az lock update.</span></span> <span data-ttu-id="5f12f-621">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5f12f-621">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5f12f-622">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="5f12f-622">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5f12f-623">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5f12f-623">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5f12f-624">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-624">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5f12f-625">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5f12f-625">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5f12f-626">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="5f12f-626">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-627">Rol</span><span class="sxs-lookup"><span data-stu-id="5f12f-627">Role</span></span>

* <span data-ttu-id="5f12f-628">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="5f12f-628">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5f12f-629">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="5f12f-629">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5f12f-630">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="5f12f-630">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5f12f-631">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="5f12f-631">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-632">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-632">SQL</span></span>

* <span data-ttu-id="5f12f-633">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="5f12f-633">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="5f12f-634">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="5f12f-634">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-635">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="5f12f-635">Storage</span></span>

* <span data-ttu-id="5f12f-636">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-636">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="5f12f-637">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="5f12f-637">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5f12f-638">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="5f12f-638">Add support for large block blob upload</span></span>
* <span data-ttu-id="5f12f-639">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="5f12f-639">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-640">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-640">VM</span></span>

* <span data-ttu-id="5f12f-641">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="5f12f-641">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5f12f-642">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="5f12f-642">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5f12f-643">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5f12f-643">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5f12f-644">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5f12f-644">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5f12f-645">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="5f12f-645">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5f12f-646">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="5f12f-646">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5f12f-647">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="5f12f-647">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5f12f-648">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-648">April 3, 2017</span></span>

<span data-ttu-id="5f12f-649">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5f12f-649">Version 2.0.2</span></span>

<span data-ttu-id="5f12f-650">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="5f12f-650">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="5f12f-651">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f12f-651">Core</span></span>

* <span data-ttu-id="5f12f-652">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="5f12f-652">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="5f12f-653">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="5f12f-653">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5f12f-654">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="5f12f-654">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5f12f-655">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5f12f-655">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f12f-656">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="5f12f-656">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5f12f-657">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="5f12f-657">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5f12f-658">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="5f12f-658">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5f12f-659">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="5f12f-659">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5f12f-660">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="5f12f-660">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="5f12f-661">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-661">ACS</span></span>

* <span data-ttu-id="5f12f-662">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="5f12f-662">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5f12f-663">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="5f12f-663">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5f12f-664">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="5f12f-664">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5f12f-665">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="5f12f-665">Add support for windows clusters.</span></span> <span data-ttu-id="5f12f-666">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="5f12f-666">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5f12f-667">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="5f12f-667">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5f12f-668">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="5f12f-668">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="5f12f-669">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-669">AppService</span></span>

* <span data-ttu-id="5f12f-670">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="5f12f-670">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5f12f-671">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="5f12f-671">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5f12f-672">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="5f12f-672">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5f12f-673">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="5f12f-673">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="5f12f-674">DataLake</span><span class="sxs-lookup"><span data-stu-id="5f12f-674">DataLake</span></span>

* <span data-ttu-id="5f12f-675">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5f12f-675">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="5f12f-676">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5f12f-676">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="5f12f-677">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-677">DocuemntDB</span></span>

* <span data-ttu-id="5f12f-678">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="5f12f-678">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-679">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f12f-679">VM</span></span>

* <span data-ttu-id="5f12f-680">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="5f12f-680">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5f12f-681">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="5f12f-681">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5f12f-682">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="5f12f-682">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5f12f-683">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5f12f-683">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f12f-684">Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="5f12f-684">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5f12f-685">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="5f12f-685">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="5f12f-686">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="5f12f-686">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5f12f-687">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-687">February 27, 2017</span></span>

<span data-ttu-id="5f12f-688">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-688">Version 2.0.0</span></span>

<span data-ttu-id="5f12f-689">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="5f12f-689">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="5f12f-690">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="5f12f-690">General availability applies to these command modules:</span></span>
- <span data-ttu-id="5f12f-691">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="5f12f-691">Container Service (acs)</span></span>
- <span data-ttu-id="5f12f-692">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="5f12f-692">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5f12f-693">Redes</span><span class="sxs-lookup"><span data-stu-id="5f12f-693">Networking</span></span>
- <span data-ttu-id="5f12f-694">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="5f12f-694">Storage</span></span>

<span data-ttu-id="5f12f-695">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5f12f-695">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="5f12f-696">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="5f12f-696">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="5f12f-697">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-697">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="5f12f-698">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="5f12f-698">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="5f12f-699">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-699">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="5f12f-700">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="5f12f-700">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="5f12f-701">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="5f12f-701">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="5f12f-702">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="5f12f-702">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="5f12f-703">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="5f12f-703">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="5f12f-704">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="5f12f-704">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="5f12f-705">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="5f12f-705">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5f12f-706">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="5f12f-706">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5f12f-707">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="5f12f-707">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="5f12f-708">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-708">Provide feedback from the command line with the `az feedback` command.</span></span>

