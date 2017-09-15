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
ms.openlocfilehash: ad30efeb7efafcc5816160ee130665d37adb62c6
ms.sourcegitcommit: e866977985ba0286fa05f41729dd7e7d9ce86f8e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/13/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="36a9d-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="36a9d-104">Azure CLI 2.0 release notes</span></span>

## <a name="september-11-2017"></a><span data-ttu-id="36a9d-105">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-105">September 11, 2017</span></span>

<span data-ttu-id="36a9d-106">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="36a9d-106">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="36a9d-107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="36a9d-107">Core</span></span>

* <span data-ttu-id="36a9d-108">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="36a9d-108">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="36a9d-109">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="36a9d-109">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="36a9d-110">ACS</span><span class="sxs-lookup"><span data-stu-id="36a9d-110">Acs</span></span>

* <span data-ttu-id="36a9d-111">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-111">Added `acs list-locations` command</span></span>
* <span data-ttu-id="36a9d-112">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="36a9d-112">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="36a9d-113">Appservice</span><span class="sxs-lookup"><span data-stu-id="36a9d-113">Appservice</span></span>

* <span data-ttu-id="36a9d-114">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="36a9d-114">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="36a9d-115">CDN</span><span class="sxs-lookup"><span data-stu-id="36a9d-115">CDN</span></span>

* <span data-ttu-id="36a9d-116">Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-116">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="36a9d-117">Extensión</span><span class="sxs-lookup"><span data-stu-id="36a9d-117">Extension</span></span>

* <span data-ttu-id="36a9d-118">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="36a9d-118">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="36a9d-119">Keyvault</span><span class="sxs-lookup"><span data-stu-id="36a9d-119">Keyvault</span></span>

* <span data-ttu-id="36a9d-120">Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-120">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="36a9d-121">Red</span><span class="sxs-lookup"><span data-stu-id="36a9d-121">Network</span></span>

* <span data-ttu-id="36a9d-122">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-122">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="36a9d-123">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-123">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="36a9d-124">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-124">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="36a9d-125">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="36a9d-126">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-126">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="36a9d-127">Recurso</span><span class="sxs-lookup"><span data-stu-id="36a9d-127">Resource</span></span>

* <span data-ttu-id="36a9d-128">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-128">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="36a9d-129">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-129">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="36a9d-130">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="36a9d-130">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="36a9d-131">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="36a9d-131">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="36a9d-132">SQL</span><span class="sxs-lookup"><span data-stu-id="36a9d-132">SQL</span></span>

* <span data-ttu-id="36a9d-133">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-133">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="36a9d-134">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="36a9d-134">VM</span></span>

* <span data-ttu-id="36a9d-135">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-135">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="36a9d-136">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="36a9d-136">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="36a9d-137">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-137">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="36a9d-138">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="36a9d-138">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="36a9d-139">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="36a9d-139">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="36a9d-140">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-140">August 31, 2017</span></span>

<span data-ttu-id="36a9d-141">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="36a9d-141">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="36a9d-142">Keyvault</span><span class="sxs-lookup"><span data-stu-id="36a9d-142">Keyvault</span></span>

* <span data-ttu-id="36a9d-143">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-143">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="36a9d-144">Sf</span><span class="sxs-lookup"><span data-stu-id="36a9d-144">Sf</span></span>

* <span data-ttu-id="36a9d-145">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="36a9d-145">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="36a9d-146">Storage</span><span class="sxs-lookup"><span data-stu-id="36a9d-146">Storage</span></span>

* <span data-ttu-id="36a9d-147">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="36a9d-147">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="36a9d-148">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="36a9d-148">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="36a9d-149">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-149">August 28, 2017</span></span>

<span data-ttu-id="36a9d-150">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="36a9d-150">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="36a9d-151">CLI</span><span class="sxs-lookup"><span data-stu-id="36a9d-151">CLI</span></span>

* <span data-ttu-id="36a9d-152">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-152">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="36a9d-153">ACS</span><span class="sxs-lookup"><span data-stu-id="36a9d-153">ACS</span></span>

* <span data-ttu-id="36a9d-154">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="36a9d-154">Corrected preview regions.</span></span>
* <span data-ttu-id="36a9d-155">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="36a9d-155">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="36a9d-156">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="36a9d-156">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="36a9d-157">Appservice</span><span class="sxs-lookup"><span data-stu-id="36a9d-157">Appservice</span></span>

* <span data-ttu-id="36a9d-158">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-158">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="36a9d-159">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-159">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="36a9d-160">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-160">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="36a9d-161">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="36a9d-161">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="36a9d-162">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="36a9d-162">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="36a9d-163">IoT</span><span class="sxs-lookup"><span data-stu-id="36a9d-163">IoT</span></span>

* <span data-ttu-id="36a9d-164">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="36a9d-164">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="36a9d-165">Red</span><span class="sxs-lookup"><span data-stu-id="36a9d-165">Network</span></span>

* <span data-ttu-id="36a9d-166">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-166">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="36a9d-167">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-167">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="36a9d-168">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-168">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="36a9d-169">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-169">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="36a9d-170">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-170">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="36a9d-171">Perfil</span><span class="sxs-lookup"><span data-stu-id="36a9d-171">Profile</span></span>

* <span data-ttu-id="36a9d-172">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="36a9d-172">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="36a9d-173">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="36a9d-173">Service Fabric</span></span>

* <span data-ttu-id="36a9d-174">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="36a9d-174">Preview release</span></span>
* <span data-ttu-id="36a9d-175">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="36a9d-175">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="36a9d-176">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="36a9d-176">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="36a9d-177">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-177">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="36a9d-178">Storage</span><span class="sxs-lookup"><span data-stu-id="36a9d-178">Storage</span></span>

* <span data-ttu-id="36a9d-179">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="36a9d-179">Enabled setting blob tier</span></span>
* <span data-ttu-id="36a9d-180">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="36a9d-180">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="36a9d-181">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-181">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="36a9d-182">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="36a9d-182">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="36a9d-183">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-183">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="36a9d-184">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="36a9d-184">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="36a9d-185">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="36a9d-185">VM</span></span>

* <span data-ttu-id="36a9d-186">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-186">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="36a9d-187">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-187">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="36a9d-188">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-188">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="36a9d-189">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="36a9d-189">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="36a9d-190">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="36a9d-190">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="36a9d-191">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-191">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="36a9d-192">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-192">August 15, 2017</span></span>

<span data-ttu-id="36a9d-193">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="36a9d-193">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="36a9d-194">ACS</span><span class="sxs-lookup"><span data-stu-id="36a9d-194">ACS</span></span>

* <span data-ttu-id="36a9d-195">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="36a9d-195">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="36a9d-196">Appservice</span><span class="sxs-lookup"><span data-stu-id="36a9d-196">Appservice</span></span>

* <span data-ttu-id="36a9d-197">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="36a9d-197">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="36a9d-198">Event Grid</span><span class="sxs-lookup"><span data-stu-id="36a9d-198">Event Grid</span></span>

* <span data-ttu-id="36a9d-199">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="36a9d-199">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="36a9d-200">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-200">August 11, 2017</span></span>

<span data-ttu-id="36a9d-201">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="36a9d-201">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="36a9d-202">ACS</span><span class="sxs-lookup"><span data-stu-id="36a9d-202">ACS</span></span>

* <span data-ttu-id="36a9d-203">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="36a9d-203">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="36a9d-204">Batch</span><span class="sxs-lookup"><span data-stu-id="36a9d-204">Batch</span></span>

* <span data-ttu-id="36a9d-205">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="36a9d-205">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="36a9d-206">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="36a9d-206">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="36a9d-207">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="36a9d-207">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="36a9d-208">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="36a9d-208">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="36a9d-209">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="36a9d-209">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="36a9d-210">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="36a9d-210">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="36a9d-211">Componente</span><span class="sxs-lookup"><span data-stu-id="36a9d-211">Component</span></span>

* <span data-ttu-id="36a9d-212">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="36a9d-212">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="36a9d-213">Contenedor</span><span class="sxs-lookup"><span data-stu-id="36a9d-213">Container</span></span>

* <span data-ttu-id="36a9d-214">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="36a9d-214">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="36a9d-215">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="36a9d-215">Data Lake Store</span></span>

* <span data-ttu-id="36a9d-216">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="36a9d-216">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="36a9d-217">Event Grid</span><span class="sxs-lookup"><span data-stu-id="36a9d-217">Event Grid</span></span>

* <span data-ttu-id="36a9d-218">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="36a9d-218">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="36a9d-219">Red</span><span class="sxs-lookup"><span data-stu-id="36a9d-219">Network</span></span>

* <span data-ttu-id="36a9d-220">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="36a9d-220">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="36a9d-221">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-221">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="36a9d-222">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="36a9d-222">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="36a9d-223">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-223">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="36a9d-224">Perfil</span><span class="sxs-lookup"><span data-stu-id="36a9d-224">Profile</span></span>

* <span data-ttu-id="36a9d-225">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="36a9d-225">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="36a9d-226">Storage</span><span class="sxs-lookup"><span data-stu-id="36a9d-226">Storage</span></span>

* <span data-ttu-id="36a9d-227">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="36a9d-227">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="36a9d-228">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="36a9d-228">VM</span></span>

* <span data-ttu-id="36a9d-229">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="36a9d-229">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="36a9d-230">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-230">Exposed `list-skus` command</span></span>
* <span data-ttu-id="36a9d-231">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="36a9d-231">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="36a9d-232">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="36a9d-232">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="36a9d-233">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="36a9d-233">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="36a9d-234">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-234">July 28, 2017</span></span>

<span data-ttu-id="36a9d-235">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="36a9d-235">Version 2.0.12</span></span>

* <span data-ttu-id="36a9d-236">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="36a9d-236">Added container commands</span></span>
* <span data-ttu-id="36a9d-237">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="36a9d-237">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="36a9d-238">Núcleo</span><span class="sxs-lookup"><span data-stu-id="36a9d-238">Core</span></span>

* <span data-ttu-id="36a9d-239">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="36a9d-239">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="36a9d-240">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="36a9d-240">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="36a9d-241">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="36a9d-241">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="36a9d-242">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="36a9d-242">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="36a9d-243">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="36a9d-243">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="36a9d-244">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="36a9d-244">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="36a9d-245">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="36a9d-245">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="36a9d-246">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="36a9d-246">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="36a9d-247">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="36a9d-247">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="36a9d-248">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="36a9d-248">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="36a9d-249">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="36a9d-249">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="36a9d-250">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="36a9d-250">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="36a9d-251">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="36a9d-251">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="36a9d-252">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="36a9d-252">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="36a9d-253">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="36a9d-253">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="36a9d-254">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="36a9d-254">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="36a9d-255">ACR</span><span class="sxs-lookup"><span data-stu-id="36a9d-255">ACR</span></span>

* <span data-ttu-id="36a9d-256">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="36a9d-256">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="36a9d-257">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="36a9d-257">Support SKU update for managed registries</span></span>
* <span data-ttu-id="36a9d-258">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="36a9d-258">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="36a9d-259">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="36a9d-259">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="36a9d-260">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="36a9d-260">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="36a9d-261">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="36a9d-261">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="36a9d-262">ACS</span><span class="sxs-lookup"><span data-stu-id="36a9d-262">ACS</span></span>

* <span data-ttu-id="36a9d-263">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="36a9d-263">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="36a9d-264">Appservice</span><span class="sxs-lookup"><span data-stu-id="36a9d-264">Appservice</span></span>

* <span data-ttu-id="36a9d-265">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="36a9d-265">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="36a9d-266">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="36a9d-266">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="36a9d-267">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-267">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="36a9d-268">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="36a9d-268">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="36a9d-269">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="36a9d-269">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="36a9d-270">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="36a9d-270">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="36a9d-271">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="36a9d-271">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="36a9d-272">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="36a9d-272">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="36a9d-273">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="36a9d-273">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="36a9d-274">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="36a9d-274">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="36a9d-275">Batch</span><span class="sxs-lookup"><span data-stu-id="36a9d-275">Batch</span></span>

* <span data-ttu-id="36a9d-276">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="36a9d-276">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="36a9d-277">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-277">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="36a9d-278">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-278">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="36a9d-279">CDN</span><span class="sxs-lookup"><span data-stu-id="36a9d-279">CDN</span></span>

* <span data-ttu-id="36a9d-280">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="36a9d-280">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="36a9d-281">Nube</span><span class="sxs-lookup"><span data-stu-id="36a9d-281">Cloud</span></span>

* <span data-ttu-id="36a9d-282">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="36a9d-282">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="36a9d-283">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="36a9d-283">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="36a9d-284">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="36a9d-284">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="36a9d-285">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="36a9d-285">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="36a9d-286">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-286">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="36a9d-287">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="36a9d-287">CosmosDB</span></span>

* <span data-ttu-id="36a9d-288">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="36a9d-288">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="36a9d-289">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="36a9d-289">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="36a9d-290">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="36a9d-290">Data Lake Analytics</span></span>

* <span data-ttu-id="36a9d-291">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-291">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="36a9d-292">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-292">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="36a9d-293">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-293">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="36a9d-294">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="36a9d-294">Data Lake Store</span></span>

* <span data-ttu-id="36a9d-295">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-295">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="36a9d-296">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="36a9d-296">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="36a9d-297">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-297">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="36a9d-298">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="36a9d-298">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="36a9d-299">Interactive</span><span class="sxs-lookup"><span data-stu-id="36a9d-299">Interactive</span></span>

* <span data-ttu-id="36a9d-300">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="36a9d-300">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="36a9d-301">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="36a9d-301">Increased test coverage</span></span>
* <span data-ttu-id="36a9d-302">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="36a9d-302">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="36a9d-303">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="36a9d-303">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="36a9d-304">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="36a9d-304">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="36a9d-305">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="36a9d-305">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="36a9d-306">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="36a9d-306">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="36a9d-307">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-307">Added `--progress` flag</span></span>
* <span data-ttu-id="36a9d-308">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="36a9d-308">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="36a9d-309">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="36a9d-309">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="36a9d-310">IoT</span><span class="sxs-lookup"><span data-stu-id="36a9d-310">IoT</span></span>

* <span data-ttu-id="36a9d-311">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="36a9d-311">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="36a9d-312">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="36a9d-312">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="36a9d-313">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="36a9d-313">Key vault</span></span>

* <span data-ttu-id="36a9d-314">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="36a9d-314">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="36a9d-315">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="36a9d-315">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="36a9d-316">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="36a9d-316">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="36a9d-317">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="36a9d-317">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="36a9d-318">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="36a9d-318">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="36a9d-319">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="36a9d-319">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="36a9d-320">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="36a9d-320">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="36a9d-321">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="36a9d-321">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="36a9d-322">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="36a9d-322">Lab</span></span>

* <span data-ttu-id="36a9d-323">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-323">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="36a9d-324">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-324">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="36a9d-325">Supervisión</span><span class="sxs-lookup"><span data-stu-id="36a9d-325">Monitor</span></span>

* <span data-ttu-id="36a9d-326">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="36a9d-326">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="36a9d-327">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-327">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="36a9d-328">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-328">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="36a9d-329">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-329">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="36a9d-330">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-330">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="36a9d-331">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="36a9d-331">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="36a9d-332">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="36a9d-332">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="36a9d-333">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="36a9d-333">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="36a9d-334">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="36a9d-334">`location` no longer required</span></span>
  * <span data-ttu-id="36a9d-335">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="36a9d-335">Add name and ID support for target</span></span>
  * <span data-ttu-id="36a9d-336">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-336">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="36a9d-337">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="36a9d-337">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="36a9d-338">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="36a9d-338">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="36a9d-339">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="36a9d-339">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="36a9d-340">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-340">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="36a9d-341">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="36a9d-341">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="36a9d-342">Red</span><span class="sxs-lookup"><span data-stu-id="36a9d-342">Network</span></span>

* <span data-ttu-id="36a9d-343">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-343">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="36a9d-344">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-344">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="36a9d-345">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="36a9d-345">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="36a9d-346">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="36a9d-346">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="36a9d-347">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-347">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="36a9d-348">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-348">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="36a9d-349">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="36a9d-349">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="36a9d-350">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="36a9d-350">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="36a9d-351">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="36a9d-351">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="36a9d-352">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="36a9d-352">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="36a9d-353">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="36a9d-353">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="36a9d-354">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-354">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="36a9d-355">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="36a9d-355">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="36a9d-356">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-356">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="36a9d-357">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-357">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="36a9d-358">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-358">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="36a9d-359">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="36a9d-359">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="36a9d-360">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-360">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="36a9d-361">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-361">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="36a9d-362">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-362">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="36a9d-363">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-363">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="36a9d-364">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-364">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="36a9d-365">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-365">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="36a9d-366">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="36a9d-366">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="36a9d-367">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="36a9d-367">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="36a9d-368">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="36a9d-368">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="36a9d-369">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="36a9d-369">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="36a9d-370">Perfil</span><span class="sxs-lookup"><span data-stu-id="36a9d-370">Profile</span></span>

* <span data-ttu-id="36a9d-371">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="36a9d-371">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="36a9d-372">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="36a9d-372">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="36a9d-373">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="36a9d-373">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="36a9d-374">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="36a9d-374">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="36a9d-375">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="36a9d-375">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="36a9d-376">RDBMS</span><span class="sxs-lookup"><span data-stu-id="36a9d-376">RDBMS</span></span>

* <span data-ttu-id="36a9d-377">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="36a9d-377">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="36a9d-378">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="36a9d-378">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="36a9d-379">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="36a9d-379">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="36a9d-380">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="36a9d-380">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="36a9d-381">Recurso</span><span class="sxs-lookup"><span data-stu-id="36a9d-381">Resource</span></span>

* <span data-ttu-id="36a9d-382">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-382">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="36a9d-383">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-383">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="36a9d-384">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-384">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="36a9d-385">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-385">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="36a9d-386">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="36a9d-386">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="36a9d-387">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-387">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="36a9d-388">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="36a9d-388">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="36a9d-389">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-389">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="36a9d-390">Rol</span><span class="sxs-lookup"><span data-stu-id="36a9d-390">Role</span></span>

* <span data-ttu-id="36a9d-391">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="36a9d-391">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="36a9d-392">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="36a9d-392">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="36a9d-393">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-393">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="36a9d-394">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-394">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="36a9d-395">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-395">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="36a9d-396">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="36a9d-396">Service Fabric</span></span>
* <span data-ttu-id="36a9d-397">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="36a9d-397">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="36a9d-398">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="36a9d-398">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="36a9d-399">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="36a9d-399">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="36a9d-400">SQL</span><span class="sxs-lookup"><span data-stu-id="36a9d-400">SQL</span></span>

* <span data-ttu-id="36a9d-401">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="36a9d-401">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="36a9d-402">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-402">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="36a9d-403">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-403">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="36a9d-404">Storage</span><span class="sxs-lookup"><span data-stu-id="36a9d-404">Storage</span></span>

* <span data-ttu-id="36a9d-405">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="36a9d-405">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="36a9d-406">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="36a9d-406">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="36a9d-407">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="36a9d-407">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="36a9d-408">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="36a9d-408">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="36a9d-409">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="36a9d-409">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="36a9d-410">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="36a9d-410">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="36a9d-411">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="36a9d-411">VM</span></span>

* <span data-ttu-id="36a9d-412">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="36a9d-412">Support configuring nsg</span></span>
* <span data-ttu-id="36a9d-413">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="36a9d-413">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="36a9d-414">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="36a9d-414">Support managed service identities</span></span>
* <span data-ttu-id="36a9d-415">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-415">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="36a9d-416">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="36a9d-416">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="36a9d-417">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-417">May 10, 2017</span></span>

<span data-ttu-id="36a9d-418">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="36a9d-418">Version 2.0.6</span></span>

* <span data-ttu-id="36a9d-419">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="36a9d-419">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="36a9d-420">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="36a9d-420">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="36a9d-421">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="36a9d-421">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="36a9d-422">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="36a9d-422">Include Cognitive Services module.</span></span>
* <span data-ttu-id="36a9d-423">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="36a9d-423">Include Service Fabric module.</span></span>
* <span data-ttu-id="36a9d-424">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="36a9d-424">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="36a9d-425">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="36a9d-425">Add support for CDN commands.</span></span>
* <span data-ttu-id="36a9d-426">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="36a9d-426">Remove Container module.</span></span>
* <span data-ttu-id="36a9d-427">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="36a9d-427">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="36a9d-428">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="36a9d-428">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="36a9d-429">Núcleo</span><span class="sxs-lookup"><span data-stu-id="36a9d-429">Core</span></span>

* <span data-ttu-id="36a9d-430">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="36a9d-430">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="36a9d-431">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="36a9d-431">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="36a9d-432">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="36a9d-432">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="36a9d-433">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="36a9d-433">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="36a9d-434">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="36a9d-434">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="36a9d-435">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="36a9d-435">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="36a9d-436">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="36a9d-436">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="36a9d-437">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="36a9d-437">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="36a9d-438">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="36a9d-438">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="36a9d-439">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="36a9d-439">core: Improved performance</span></span>
* <span data-ttu-id="36a9d-440">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="36a9d-440">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="36a9d-441">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="36a9d-441">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="36a9d-442">ACS</span><span class="sxs-lookup"><span data-stu-id="36a9d-442">ACS</span></span>

* <span data-ttu-id="36a9d-443">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="36a9d-443">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="36a9d-444">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="36a9d-444">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="36a9d-445">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="36a9d-445">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="36a9d-446">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="36a9d-446">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="36a9d-447">AppService</span><span class="sxs-lookup"><span data-stu-id="36a9d-447">AppService</span></span>

* <span data-ttu-id="36a9d-448">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="36a9d-448">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="36a9d-449">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="36a9d-449">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="36a9d-450">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="36a9d-450">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="36a9d-451">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="36a9d-451">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="36a9d-452">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="36a9d-452">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="36a9d-453">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="36a9d-453">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="36a9d-454">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="36a9d-454">support slot swap with preview</span></span>
* <span data-ttu-id="36a9d-455">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="36a9d-455">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="36a9d-456">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="36a9d-456">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="36a9d-457">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="36a9d-457">CosmosDB</span></span>

* <span data-ttu-id="36a9d-458">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="36a9d-458">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="36a9d-459">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="36a9d-459">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="36a9d-460">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="36a9d-460">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="36a9d-461">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="36a9d-461">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="36a9d-462">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="36a9d-462">Data Lake Analytics</span></span>

* <span data-ttu-id="36a9d-463">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="36a9d-463">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="36a9d-464">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="36a9d-464">Add support for new catalog item type: package.</span></span> <span data-ttu-id="36a9d-465">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="36a9d-465">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="36a9d-466">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="36a9d-466">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="36a9d-467">Tabla</span><span class="sxs-lookup"><span data-stu-id="36a9d-467">Table</span></span>
  * <span data-ttu-id="36a9d-468">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="36a9d-468">Table valued function</span></span>
  * <span data-ttu-id="36a9d-469">Ver</span><span class="sxs-lookup"><span data-stu-id="36a9d-469">View</span></span>
  * <span data-ttu-id="36a9d-470">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="36a9d-470">Table Statistics.</span></span> <span data-ttu-id="36a9d-471">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="36a9d-471">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="36a9d-472">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="36a9d-472">Data Lake Store</span></span>

* <span data-ttu-id="36a9d-473">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="36a9d-473">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="36a9d-474">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="36a9d-474">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="36a9d-475">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="36a9d-475">missed help for access show.</span></span> <span data-ttu-id="36a9d-476">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="36a9d-476">adding it.</span></span> <span data-ttu-id="36a9d-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="36a9d-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="36a9d-478">Buscar</span><span class="sxs-lookup"><span data-stu-id="36a9d-478">Find</span></span>

* <span data-ttu-id="36a9d-479">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="36a9d-479">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="36a9d-480">KeyVault</span><span class="sxs-lookup"><span data-stu-id="36a9d-480">KeyVault</span></span>

* <span data-ttu-id="36a9d-481">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="36a9d-481">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="36a9d-482">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="36a9d-482">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="36a9d-483">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="36a9d-483">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="36a9d-484">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="36a9d-484">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="36a9d-485">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="36a9d-485">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="36a9d-486">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="36a9d-486">Lab</span></span>

* <span data-ttu-id="36a9d-487">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="36a9d-487">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="36a9d-488">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="36a9d-488">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="36a9d-489">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="36a9d-489">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="36a9d-490">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="36a9d-490">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="36a9d-491">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="36a9d-491">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="36a9d-492">Supervisión</span><span class="sxs-lookup"><span data-stu-id="36a9d-492">Monitor</span></span>

* <span data-ttu-id="36a9d-493">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="36a9d-493">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="36a9d-494">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="36a9d-494">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="36a9d-495">Red</span><span class="sxs-lookup"><span data-stu-id="36a9d-495">Network</span></span>

* <span data-ttu-id="36a9d-496">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="36a9d-496">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="36a9d-497">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="36a9d-497">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="36a9d-498">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="36a9d-498">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="36a9d-499">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="36a9d-499">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="36a9d-500">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="36a9d-500">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="36a9d-501">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="36a9d-501">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="36a9d-502">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="36a9d-502">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="36a9d-503">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="36a9d-503">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="36a9d-504">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="36a9d-504">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="36a9d-505">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="36a9d-505">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="36a9d-506">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="36a9d-506">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="36a9d-507">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="36a9d-507">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="36a9d-508">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="36a9d-508">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="36a9d-509">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="36a9d-509">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="36a9d-510">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="36a9d-510">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="36a9d-511">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="36a9d-511">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="36a9d-512">Perfil</span><span class="sxs-lookup"><span data-stu-id="36a9d-512">Profile</span></span>

* <span data-ttu-id="36a9d-513">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="36a9d-513">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="36a9d-514">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="36a9d-514">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="36a9d-515">Redis</span><span class="sxs-lookup"><span data-stu-id="36a9d-515">Redis</span></span>

* <span data-ttu-id="36a9d-516">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="36a9d-516">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="36a9d-517">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="36a9d-517">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="36a9d-518">Recurso</span><span class="sxs-lookup"><span data-stu-id="36a9d-518">Resource</span></span>

* <span data-ttu-id="36a9d-519">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="36a9d-519">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="36a9d-520">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="36a9d-520">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="36a9d-521">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="36a9d-521">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="36a9d-522">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="36a9d-522">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="36a9d-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="36a9d-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="36a9d-524">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="36a9d-524">Add docs for az lock update.</span></span> <span data-ttu-id="36a9d-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="36a9d-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="36a9d-526">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="36a9d-526">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="36a9d-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="36a9d-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="36a9d-528">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="36a9d-528">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="36a9d-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="36a9d-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="36a9d-530">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="36a9d-530">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="36a9d-531">Rol</span><span class="sxs-lookup"><span data-stu-id="36a9d-531">Role</span></span>

* <span data-ttu-id="36a9d-532">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="36a9d-532">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="36a9d-533">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="36a9d-533">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="36a9d-534">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="36a9d-534">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="36a9d-535">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="36a9d-535">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="36a9d-536">SQL</span><span class="sxs-lookup"><span data-stu-id="36a9d-536">SQL</span></span>

* <span data-ttu-id="36a9d-537">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="36a9d-537">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="36a9d-538">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="36a9d-538">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="36a9d-539">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="36a9d-539">Storage</span></span>

* <span data-ttu-id="36a9d-540">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="36a9d-540">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="36a9d-541">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="36a9d-541">Add support for incremental blob copy</span></span>
* <span data-ttu-id="36a9d-542">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="36a9d-542">Add support for large block blob upload</span></span>
* <span data-ttu-id="36a9d-543">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="36a9d-543">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="36a9d-544">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="36a9d-544">VM</span></span>

* <span data-ttu-id="36a9d-545">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="36a9d-545">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="36a9d-546">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="36a9d-546">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="36a9d-547">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="36a9d-547">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="36a9d-548">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="36a9d-548">az vm/vmss disk</span></span>
  3. <span data-ttu-id="36a9d-549">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="36a9d-549">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="36a9d-550">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="36a9d-550">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="36a9d-551">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="36a9d-551">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="36a9d-552">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-552">April 3, 2017</span></span>

<span data-ttu-id="36a9d-553">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="36a9d-553">Version 2.0.2</span></span>

<span data-ttu-id="36a9d-554">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="36a9d-554">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="36a9d-555">Núcleo</span><span class="sxs-lookup"><span data-stu-id="36a9d-555">Core</span></span>

* <span data-ttu-id="36a9d-556">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="36a9d-556">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="36a9d-557">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="36a9d-557">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="36a9d-558">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="36a9d-558">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="36a9d-559">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="36a9d-559">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="36a9d-560">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="36a9d-560">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="36a9d-561">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="36a9d-561">Add prompting for missing template parameters.</span></span> <span data-ttu-id="36a9d-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="36a9d-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="36a9d-563">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="36a9d-563">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="36a9d-564">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="36a9d-564">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="36a9d-565">ACS</span><span class="sxs-lookup"><span data-stu-id="36a9d-565">ACS</span></span>

* <span data-ttu-id="36a9d-566">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="36a9d-566">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="36a9d-567">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="36a9d-567">Add support for ssh key password prompting.</span></span> <span data-ttu-id="36a9d-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="36a9d-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="36a9d-569">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="36a9d-569">Add support for windows clusters.</span></span> <span data-ttu-id="36a9d-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="36a9d-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="36a9d-571">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="36a9d-571">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="36a9d-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="36a9d-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="36a9d-573">AppService</span><span class="sxs-lookup"><span data-stu-id="36a9d-573">AppService</span></span>

* <span data-ttu-id="36a9d-574">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="36a9d-574">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="36a9d-575">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="36a9d-575">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="36a9d-576">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="36a9d-576">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="36a9d-577">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="36a9d-577">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="36a9d-578">DataLake</span><span class="sxs-lookup"><span data-stu-id="36a9d-578">DataLake</span></span>

* <span data-ttu-id="36a9d-579">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="36a9d-579">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="36a9d-580">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="36a9d-580">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="36a9d-581">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="36a9d-581">DocuemntDB</span></span>

* <span data-ttu-id="36a9d-582">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="36a9d-582">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="36a9d-583">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="36a9d-583">VM</span></span>

* <span data-ttu-id="36a9d-584">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="36a9d-584">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="36a9d-585">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="36a9d-585">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="36a9d-586">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="36a9d-586">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="36a9d-587">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="36a9d-587">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="36a9d-588">Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="36a9d-588">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="36a9d-589">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="36a9d-589">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="36a9d-590">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="36a9d-590">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="36a9d-591">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="36a9d-591">February 27, 2017</span></span>

<span data-ttu-id="36a9d-592">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="36a9d-592">Version 2.0.0</span></span>

<span data-ttu-id="36a9d-593">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="36a9d-593">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="36a9d-594">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="36a9d-594">General availability applies to these command modules:</span></span>
- <span data-ttu-id="36a9d-595">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="36a9d-595">Container Service (acs)</span></span>
- <span data-ttu-id="36a9d-596">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="36a9d-596">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="36a9d-597">Redes</span><span class="sxs-lookup"><span data-stu-id="36a9d-597">Networking</span></span>
- <span data-ttu-id="36a9d-598">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="36a9d-598">Storage</span></span>

<span data-ttu-id="36a9d-599">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="36a9d-599">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="36a9d-600">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="36a9d-600">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="36a9d-601">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-601">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="36a9d-602">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="36a9d-602">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="36a9d-603">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-603">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="36a9d-604">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="36a9d-604">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="36a9d-605">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="36a9d-605">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="36a9d-606">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="36a9d-606">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="36a9d-607">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="36a9d-607">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="36a9d-608">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="36a9d-608">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="36a9d-609">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="36a9d-609">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="36a9d-610">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="36a9d-610">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="36a9d-611">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="36a9d-611">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="36a9d-612">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="36a9d-612">Provide feedback from the command line with the `az feedback` command.</span></span>

