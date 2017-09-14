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
ms.openlocfilehash: e893b99349bbf2a5eec8af254158eb07001f1da7
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/04/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="60fff-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="60fff-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="60fff-105">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="60fff-105">August 28, 2017</span></span>

<span data-ttu-id="60fff-106">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="60fff-106">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="60fff-107">CLI</span><span class="sxs-lookup"><span data-stu-id="60fff-107">CLI</span></span>

* <span data-ttu-id="60fff-108">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="60fff-108">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="60fff-109">ACS</span><span class="sxs-lookup"><span data-stu-id="60fff-109">ACS</span></span>

* <span data-ttu-id="60fff-110">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="60fff-110">Corrected preview regions.</span></span>
* <span data-ttu-id="60fff-111">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="60fff-111">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="60fff-112">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="60fff-112">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="60fff-113">Appservice</span><span class="sxs-lookup"><span data-stu-id="60fff-113">Appservice</span></span>

* <span data-ttu-id="60fff-114">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="60fff-114">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="60fff-115">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="60fff-115">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="60fff-116">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="60fff-116">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="60fff-117">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="60fff-117">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="60fff-118">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="60fff-118">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="60fff-119">IoT</span><span class="sxs-lookup"><span data-stu-id="60fff-119">IoT</span></span>

* <span data-ttu-id="60fff-120">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="60fff-120">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="60fff-121">Red</span><span class="sxs-lookup"><span data-stu-id="60fff-121">Network</span></span>

* <span data-ttu-id="60fff-122">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="60fff-122">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="60fff-123">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="60fff-123">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="60fff-124">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="60fff-124">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="60fff-125">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="60fff-126">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-126">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="60fff-127">Perfil</span><span class="sxs-lookup"><span data-stu-id="60fff-127">Profile</span></span>

* <span data-ttu-id="60fff-128">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="60fff-128">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="60fff-129">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="60fff-129">Service Fabric</span></span>

* <span data-ttu-id="60fff-130">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="60fff-130">Preview release</span></span>
* <span data-ttu-id="60fff-131">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="60fff-131">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="60fff-132">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="60fff-132">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="60fff-133">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="60fff-133">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="60fff-134">Storage</span><span class="sxs-lookup"><span data-stu-id="60fff-134">Storage</span></span>

* <span data-ttu-id="60fff-135">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="60fff-135">Enabled setting blob tier</span></span>
* <span data-ttu-id="60fff-136">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="60fff-136">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="60fff-137">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="60fff-137">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="60fff-138">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="60fff-138">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="60fff-139">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-139">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="60fff-140">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="60fff-140">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="60fff-141">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="60fff-141">VM</span></span>

* <span data-ttu-id="60fff-142">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="60fff-142">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="60fff-143">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-143">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="60fff-144">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-144">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="60fff-145">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="60fff-145">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="60fff-146">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="60fff-146">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="60fff-147">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-147">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="60fff-148">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="60fff-148">August 15, 2017</span></span>

<span data-ttu-id="60fff-149">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="60fff-149">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="60fff-150">ACS</span><span class="sxs-lookup"><span data-stu-id="60fff-150">ACS</span></span>

* <span data-ttu-id="60fff-151">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="60fff-151">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="60fff-152">Appservice</span><span class="sxs-lookup"><span data-stu-id="60fff-152">Appservice</span></span>

* <span data-ttu-id="60fff-153">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="60fff-153">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="60fff-154">Event Grid</span><span class="sxs-lookup"><span data-stu-id="60fff-154">Event Grid</span></span>

* <span data-ttu-id="60fff-155">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="60fff-155">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="60fff-156">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="60fff-156">August 11, 2017</span></span>

<span data-ttu-id="60fff-157">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="60fff-157">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="60fff-158">ACS</span><span class="sxs-lookup"><span data-stu-id="60fff-158">ACS</span></span>

* <span data-ttu-id="60fff-159">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="60fff-159">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="60fff-160">Batch</span><span class="sxs-lookup"><span data-stu-id="60fff-160">Batch</span></span>

* <span data-ttu-id="60fff-161">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="60fff-161">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="60fff-162">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="60fff-162">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="60fff-163">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="60fff-163">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="60fff-164">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="60fff-164">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="60fff-165">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="60fff-165">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="60fff-166">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="60fff-166">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="60fff-167">Componente</span><span class="sxs-lookup"><span data-stu-id="60fff-167">Component</span></span>

* <span data-ttu-id="60fff-168">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="60fff-168">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="60fff-169">Contenedor</span><span class="sxs-lookup"><span data-stu-id="60fff-169">Container</span></span>

* <span data-ttu-id="60fff-170">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="60fff-170">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="60fff-171">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="60fff-171">Data Lake Store</span></span>

* <span data-ttu-id="60fff-172">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="60fff-172">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="60fff-173">Event Grid</span><span class="sxs-lookup"><span data-stu-id="60fff-173">Event Grid</span></span>

* <span data-ttu-id="60fff-174">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="60fff-174">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="60fff-175">Red</span><span class="sxs-lookup"><span data-stu-id="60fff-175">Network</span></span>

* <span data-ttu-id="60fff-176">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="60fff-176">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="60fff-177">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="60fff-177">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="60fff-178">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="60fff-178">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="60fff-179">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="60fff-179">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="60fff-180">Perfil</span><span class="sxs-lookup"><span data-stu-id="60fff-180">Profile</span></span>

* <span data-ttu-id="60fff-181">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="60fff-181">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="60fff-182">Storage</span><span class="sxs-lookup"><span data-stu-id="60fff-182">Storage</span></span>

* <span data-ttu-id="60fff-183">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="60fff-183">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="60fff-184">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="60fff-184">VM</span></span>

* <span data-ttu-id="60fff-185">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="60fff-185">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="60fff-186">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="60fff-186">Exposed `list-skus` command</span></span>
* <span data-ttu-id="60fff-187">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="60fff-187">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="60fff-188">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="60fff-188">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="60fff-189">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="60fff-189">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="60fff-190">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="60fff-190">July 28, 2017</span></span>

<span data-ttu-id="60fff-191">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="60fff-191">Version 2.0.12</span></span>

* <span data-ttu-id="60fff-192">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="60fff-192">Added container commands</span></span>
* <span data-ttu-id="60fff-193">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="60fff-193">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="60fff-194">Núcleo</span><span class="sxs-lookup"><span data-stu-id="60fff-194">Core</span></span>

* <span data-ttu-id="60fff-195">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="60fff-195">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="60fff-196">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="60fff-196">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="60fff-197">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="60fff-197">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="60fff-198">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="60fff-198">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="60fff-199">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="60fff-199">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="60fff-200">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="60fff-200">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="60fff-201">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="60fff-201">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="60fff-202">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="60fff-202">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="60fff-203">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="60fff-203">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="60fff-204">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="60fff-204">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="60fff-205">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="60fff-205">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="60fff-206">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="60fff-206">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="60fff-207">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="60fff-207">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="60fff-208">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="60fff-208">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="60fff-209">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="60fff-209">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="60fff-210">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="60fff-210">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="60fff-211">ACR</span><span class="sxs-lookup"><span data-stu-id="60fff-211">ACR</span></span>

* <span data-ttu-id="60fff-212">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="60fff-212">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="60fff-213">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="60fff-213">Support SKU update for managed registries</span></span>
* <span data-ttu-id="60fff-214">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="60fff-214">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="60fff-215">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="60fff-215">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="60fff-216">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="60fff-216">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="60fff-217">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="60fff-217">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="60fff-218">ACS</span><span class="sxs-lookup"><span data-stu-id="60fff-218">ACS</span></span>

* <span data-ttu-id="60fff-219">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="60fff-219">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="60fff-220">Appservice</span><span class="sxs-lookup"><span data-stu-id="60fff-220">Appservice</span></span>

* <span data-ttu-id="60fff-221">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="60fff-221">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="60fff-222">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="60fff-222">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="60fff-223">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="60fff-223">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="60fff-224">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="60fff-224">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="60fff-225">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="60fff-225">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="60fff-226">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="60fff-226">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="60fff-227">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="60fff-227">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="60fff-228">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="60fff-228">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="60fff-229">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="60fff-229">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="60fff-230">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="60fff-230">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="60fff-231">Batch</span><span class="sxs-lookup"><span data-stu-id="60fff-231">Batch</span></span>

* <span data-ttu-id="60fff-232">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="60fff-232">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="60fff-233">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="60fff-233">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="60fff-234">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-234">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="60fff-235">CDN</span><span class="sxs-lookup"><span data-stu-id="60fff-235">CDN</span></span>

* <span data-ttu-id="60fff-236">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="60fff-236">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="60fff-237">Nube</span><span class="sxs-lookup"><span data-stu-id="60fff-237">Cloud</span></span>

* <span data-ttu-id="60fff-238">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="60fff-238">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="60fff-239">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="60fff-239">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="60fff-240">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="60fff-240">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="60fff-241">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="60fff-241">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="60fff-242">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="60fff-242">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="60fff-243">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60fff-243">CosmosDB</span></span>

* <span data-ttu-id="60fff-244">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="60fff-244">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="60fff-245">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="60fff-245">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="60fff-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="60fff-246">Data Lake Analytics</span></span>

* <span data-ttu-id="60fff-247">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="60fff-247">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="60fff-248">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="60fff-248">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="60fff-249">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="60fff-249">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="60fff-250">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="60fff-250">Data Lake Store</span></span>

* <span data-ttu-id="60fff-251">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-251">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="60fff-252">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="60fff-252">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="60fff-253">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="60fff-253">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="60fff-254">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="60fff-254">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="60fff-255">Interactive</span><span class="sxs-lookup"><span data-stu-id="60fff-255">Interactive</span></span>

* <span data-ttu-id="60fff-256">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="60fff-256">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="60fff-257">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="60fff-257">Increased test coverage</span></span>
* <span data-ttu-id="60fff-258">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="60fff-258">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="60fff-259">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="60fff-259">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="60fff-260">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="60fff-260">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="60fff-261">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="60fff-261">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="60fff-262">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="60fff-262">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="60fff-263">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="60fff-263">Added `--progress` flag</span></span>
* <span data-ttu-id="60fff-264">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="60fff-264">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="60fff-265">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="60fff-265">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="60fff-266">IoT</span><span class="sxs-lookup"><span data-stu-id="60fff-266">IoT</span></span>

* <span data-ttu-id="60fff-267">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="60fff-267">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="60fff-268">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="60fff-268">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="60fff-269">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="60fff-269">Key vault</span></span>

* <span data-ttu-id="60fff-270">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="60fff-270">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="60fff-271">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60fff-271">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="60fff-272">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60fff-272">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="60fff-273">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60fff-273">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="60fff-274">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60fff-274">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="60fff-275">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="60fff-275">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="60fff-276">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="60fff-276">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="60fff-277">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="60fff-277">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="60fff-278">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="60fff-278">Lab</span></span>

* <span data-ttu-id="60fff-279">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="60fff-279">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="60fff-280">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="60fff-280">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="60fff-281">Supervisión</span><span class="sxs-lookup"><span data-stu-id="60fff-281">Monitor</span></span>

* <span data-ttu-id="60fff-282">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="60fff-282">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="60fff-283">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="60fff-283">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="60fff-284">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="60fff-284">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="60fff-285">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="60fff-285">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="60fff-286">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="60fff-286">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="60fff-287">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="60fff-287">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="60fff-288">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="60fff-288">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="60fff-289">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="60fff-289">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="60fff-290">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="60fff-290">`location` no longer required</span></span>
  * <span data-ttu-id="60fff-291">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="60fff-291">Add name and ID support for target</span></span>
  * <span data-ttu-id="60fff-292">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="60fff-292">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="60fff-293">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="60fff-293">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="60fff-294">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="60fff-294">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="60fff-295">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="60fff-295">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="60fff-296">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="60fff-296">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="60fff-297">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="60fff-297">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="60fff-298">Red</span><span class="sxs-lookup"><span data-stu-id="60fff-298">Network</span></span>

* <span data-ttu-id="60fff-299">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="60fff-299">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="60fff-300">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-300">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="60fff-301">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="60fff-301">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="60fff-302">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="60fff-302">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="60fff-303">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-303">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="60fff-304">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="60fff-304">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="60fff-305">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="60fff-305">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="60fff-306">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="60fff-306">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="60fff-307">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="60fff-307">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="60fff-308">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="60fff-308">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="60fff-309">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="60fff-309">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="60fff-310">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="60fff-310">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="60fff-311">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="60fff-311">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="60fff-312">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-312">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="60fff-313">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-313">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="60fff-314">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-314">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="60fff-315">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="60fff-315">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="60fff-316">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="60fff-316">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="60fff-317">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-317">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="60fff-318">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-318">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="60fff-319">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-319">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="60fff-320">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="60fff-320">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="60fff-321">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="60fff-321">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="60fff-322">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="60fff-322">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="60fff-323">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="60fff-323">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="60fff-324">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="60fff-324">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="60fff-325">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="60fff-325">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="60fff-326">Perfil</span><span class="sxs-lookup"><span data-stu-id="60fff-326">Profile</span></span>

* <span data-ttu-id="60fff-327">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="60fff-327">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="60fff-328">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="60fff-328">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="60fff-329">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="60fff-329">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="60fff-330">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="60fff-330">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="60fff-331">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="60fff-331">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="60fff-332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="60fff-332">RDBMS</span></span>

* <span data-ttu-id="60fff-333">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="60fff-333">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="60fff-334">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="60fff-334">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="60fff-335">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="60fff-335">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="60fff-336">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="60fff-336">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="60fff-337">Recurso</span><span class="sxs-lookup"><span data-stu-id="60fff-337">Resource</span></span>

* <span data-ttu-id="60fff-338">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-338">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="60fff-339">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="60fff-339">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="60fff-340">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="60fff-340">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="60fff-341">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="60fff-341">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="60fff-342">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="60fff-342">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="60fff-343">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="60fff-343">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="60fff-344">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="60fff-344">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="60fff-345">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="60fff-345">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="60fff-346">Rol</span><span class="sxs-lookup"><span data-stu-id="60fff-346">Role</span></span>

* <span data-ttu-id="60fff-347">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="60fff-347">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="60fff-348">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="60fff-348">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="60fff-349">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="60fff-349">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="60fff-350">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="60fff-350">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="60fff-351">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="60fff-351">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="60fff-352">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="60fff-352">Service Fabric</span></span>
* <span data-ttu-id="60fff-353">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="60fff-353">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="60fff-354">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="60fff-354">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="60fff-355">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="60fff-355">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="60fff-356">SQL</span><span class="sxs-lookup"><span data-stu-id="60fff-356">SQL</span></span>

* <span data-ttu-id="60fff-357">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="60fff-357">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="60fff-358">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="60fff-358">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="60fff-359">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="60fff-359">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="60fff-360">Storage</span><span class="sxs-lookup"><span data-stu-id="60fff-360">Storage</span></span>

* <span data-ttu-id="60fff-361">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="60fff-361">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="60fff-362">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="60fff-362">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="60fff-363">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="60fff-363">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="60fff-364">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="60fff-364">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="60fff-365">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="60fff-365">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="60fff-366">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="60fff-366">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="60fff-367">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="60fff-367">VM</span></span>

* <span data-ttu-id="60fff-368">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="60fff-368">Support configuring nsg</span></span>
* <span data-ttu-id="60fff-369">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="60fff-369">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="60fff-370">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="60fff-370">Support managed service identities</span></span>
* <span data-ttu-id="60fff-371">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="60fff-371">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="60fff-372">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="60fff-372">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="60fff-373">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="60fff-373">May 10, 2017</span></span>

<span data-ttu-id="60fff-374">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="60fff-374">Version 2.0.6</span></span>

* <span data-ttu-id="60fff-375">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="60fff-375">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="60fff-376">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="60fff-376">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="60fff-377">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="60fff-377">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="60fff-378">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="60fff-378">Include Cognitive Services module.</span></span>
* <span data-ttu-id="60fff-379">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="60fff-379">Include Service Fabric module.</span></span>
* <span data-ttu-id="60fff-380">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="60fff-380">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="60fff-381">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="60fff-381">Add support for CDN commands.</span></span>
* <span data-ttu-id="60fff-382">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="60fff-382">Remove Container module.</span></span>
* <span data-ttu-id="60fff-383">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="60fff-383">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="60fff-384">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="60fff-384">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="60fff-385">Núcleo</span><span class="sxs-lookup"><span data-stu-id="60fff-385">Core</span></span>

* <span data-ttu-id="60fff-386">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="60fff-386">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="60fff-387">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="60fff-387">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="60fff-388">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="60fff-388">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="60fff-389">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="60fff-389">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="60fff-390">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="60fff-390">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="60fff-391">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="60fff-391">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="60fff-392">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="60fff-392">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="60fff-393">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="60fff-393">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="60fff-394">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="60fff-394">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="60fff-395">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="60fff-395">core: Improved performance</span></span>
* <span data-ttu-id="60fff-396">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="60fff-396">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="60fff-397">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="60fff-397">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="60fff-398">ACS</span><span class="sxs-lookup"><span data-stu-id="60fff-398">ACS</span></span>

* <span data-ttu-id="60fff-399">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="60fff-399">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="60fff-400">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="60fff-400">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="60fff-401">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="60fff-401">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="60fff-402">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="60fff-402">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="60fff-403">AppService</span><span class="sxs-lookup"><span data-stu-id="60fff-403">AppService</span></span>

* <span data-ttu-id="60fff-404">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="60fff-404">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="60fff-405">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="60fff-405">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="60fff-406">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="60fff-406">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="60fff-407">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="60fff-407">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="60fff-408">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="60fff-408">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="60fff-409">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="60fff-409">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="60fff-410">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="60fff-410">support slot swap with preview</span></span>
* <span data-ttu-id="60fff-411">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="60fff-411">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="60fff-412">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="60fff-412">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="60fff-413">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60fff-413">CosmosDB</span></span>

* <span data-ttu-id="60fff-414">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60fff-414">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="60fff-415">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="60fff-415">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="60fff-416">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="60fff-416">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="60fff-417">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="60fff-417">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="60fff-418">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="60fff-418">Data Lake Analytics</span></span>

* <span data-ttu-id="60fff-419">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="60fff-419">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="60fff-420">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="60fff-420">Add support for new catalog item type: package.</span></span> <span data-ttu-id="60fff-421">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="60fff-421">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="60fff-422">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="60fff-422">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="60fff-423">Tabla</span><span class="sxs-lookup"><span data-stu-id="60fff-423">Table</span></span>
  * <span data-ttu-id="60fff-424">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="60fff-424">Table valued function</span></span>
  * <span data-ttu-id="60fff-425">Ver</span><span class="sxs-lookup"><span data-stu-id="60fff-425">View</span></span>
  * <span data-ttu-id="60fff-426">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="60fff-426">Table Statistics.</span></span> <span data-ttu-id="60fff-427">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="60fff-427">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="60fff-428">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="60fff-428">Data Lake Store</span></span>

* <span data-ttu-id="60fff-429">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="60fff-429">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="60fff-430">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="60fff-430">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="60fff-431">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="60fff-431">missed help for access show.</span></span> <span data-ttu-id="60fff-432">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="60fff-432">adding it.</span></span> <span data-ttu-id="60fff-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="60fff-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="60fff-434">Buscar</span><span class="sxs-lookup"><span data-stu-id="60fff-434">Find</span></span>

* <span data-ttu-id="60fff-435">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="60fff-435">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="60fff-436">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60fff-436">KeyVault</span></span>

* <span data-ttu-id="60fff-437">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="60fff-437">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="60fff-438">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="60fff-438">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="60fff-439">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="60fff-439">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="60fff-440">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="60fff-440">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="60fff-441">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="60fff-441">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="60fff-442">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="60fff-442">Lab</span></span>

* <span data-ttu-id="60fff-443">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="60fff-443">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="60fff-444">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="60fff-444">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="60fff-445">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="60fff-445">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="60fff-446">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="60fff-446">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="60fff-447">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="60fff-447">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="60fff-448">Supervisión</span><span class="sxs-lookup"><span data-stu-id="60fff-448">Monitor</span></span>

* <span data-ttu-id="60fff-449">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="60fff-449">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="60fff-450">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="60fff-450">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="60fff-451">Red</span><span class="sxs-lookup"><span data-stu-id="60fff-451">Network</span></span>

* <span data-ttu-id="60fff-452">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="60fff-452">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="60fff-453">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="60fff-453">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="60fff-454">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="60fff-454">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="60fff-455">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="60fff-455">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="60fff-456">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="60fff-456">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="60fff-457">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="60fff-457">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="60fff-458">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="60fff-458">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="60fff-459">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="60fff-459">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="60fff-460">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="60fff-460">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="60fff-461">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="60fff-461">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="60fff-462">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="60fff-462">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="60fff-463">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="60fff-463">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="60fff-464">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="60fff-464">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="60fff-465">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="60fff-465">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="60fff-466">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="60fff-466">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="60fff-467">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="60fff-467">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="60fff-468">Perfil</span><span class="sxs-lookup"><span data-stu-id="60fff-468">Profile</span></span>

* <span data-ttu-id="60fff-469">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="60fff-469">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="60fff-470">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="60fff-470">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="60fff-471">Redis</span><span class="sxs-lookup"><span data-stu-id="60fff-471">Redis</span></span>

* <span data-ttu-id="60fff-472">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="60fff-472">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="60fff-473">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="60fff-473">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="60fff-474">Recurso</span><span class="sxs-lookup"><span data-stu-id="60fff-474">Resource</span></span>

* <span data-ttu-id="60fff-475">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="60fff-475">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="60fff-476">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="60fff-476">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="60fff-477">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="60fff-477">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="60fff-478">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="60fff-478">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="60fff-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="60fff-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="60fff-480">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="60fff-480">Add docs for az lock update.</span></span> <span data-ttu-id="60fff-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="60fff-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="60fff-482">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="60fff-482">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="60fff-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="60fff-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="60fff-484">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="60fff-484">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="60fff-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="60fff-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="60fff-486">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="60fff-486">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="60fff-487">Rol</span><span class="sxs-lookup"><span data-stu-id="60fff-487">Role</span></span>

* <span data-ttu-id="60fff-488">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="60fff-488">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="60fff-489">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="60fff-489">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="60fff-490">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="60fff-490">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="60fff-491">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="60fff-491">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="60fff-492">SQL</span><span class="sxs-lookup"><span data-stu-id="60fff-492">SQL</span></span>

* <span data-ttu-id="60fff-493">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="60fff-493">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="60fff-494">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="60fff-494">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="60fff-495">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="60fff-495">Storage</span></span>

* <span data-ttu-id="60fff-496">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="60fff-496">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="60fff-497">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="60fff-497">Add support for incremental blob copy</span></span>
* <span data-ttu-id="60fff-498">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="60fff-498">Add support for large block blob upload</span></span>
* <span data-ttu-id="60fff-499">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="60fff-499">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="60fff-500">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="60fff-500">VM</span></span>

* <span data-ttu-id="60fff-501">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="60fff-501">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="60fff-502">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="60fff-502">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="60fff-503">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="60fff-503">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="60fff-504">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="60fff-504">az vm/vmss disk</span></span>
  3. <span data-ttu-id="60fff-505">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="60fff-505">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="60fff-506">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="60fff-506">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="60fff-507">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="60fff-507">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="60fff-508">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="60fff-508">April 3, 2017</span></span>

<span data-ttu-id="60fff-509">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="60fff-509">Version 2.0.2</span></span>

<span data-ttu-id="60fff-510">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="60fff-510">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="60fff-511">Núcleo</span><span class="sxs-lookup"><span data-stu-id="60fff-511">Core</span></span>

* <span data-ttu-id="60fff-512">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="60fff-512">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="60fff-513">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="60fff-513">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="60fff-514">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="60fff-514">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="60fff-515">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="60fff-515">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="60fff-516">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="60fff-516">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="60fff-517">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="60fff-517">Add prompting for missing template parameters.</span></span> <span data-ttu-id="60fff-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="60fff-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="60fff-519">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="60fff-519">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="60fff-520">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="60fff-520">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="60fff-521">ACS</span><span class="sxs-lookup"><span data-stu-id="60fff-521">ACS</span></span>

* <span data-ttu-id="60fff-522">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="60fff-522">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="60fff-523">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="60fff-523">Add support for ssh key password prompting.</span></span> <span data-ttu-id="60fff-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="60fff-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="60fff-525">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="60fff-525">Add support for windows clusters.</span></span> <span data-ttu-id="60fff-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="60fff-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="60fff-527">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="60fff-527">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="60fff-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="60fff-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="60fff-529">AppService</span><span class="sxs-lookup"><span data-stu-id="60fff-529">AppService</span></span>

* <span data-ttu-id="60fff-530">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="60fff-530">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="60fff-531">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="60fff-531">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="60fff-532">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="60fff-532">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="60fff-533">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="60fff-533">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="60fff-534">DataLake</span><span class="sxs-lookup"><span data-stu-id="60fff-534">DataLake</span></span>

* <span data-ttu-id="60fff-535">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="60fff-535">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="60fff-536">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="60fff-536">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="60fff-537">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="60fff-537">DocuemntDB</span></span>

* <span data-ttu-id="60fff-538">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="60fff-538">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="60fff-539">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="60fff-539">VM</span></span>

* <span data-ttu-id="60fff-540">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="60fff-540">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="60fff-541">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="60fff-541">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="60fff-542">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="60fff-542">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="60fff-543">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="60fff-543">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="60fff-544">Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="60fff-544">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="60fff-545">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="60fff-545">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="60fff-546">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="60fff-546">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="60fff-547">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="60fff-547">February 27, 2017</span></span>

<span data-ttu-id="60fff-548">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="60fff-548">Version 2.0.0</span></span>

<span data-ttu-id="60fff-549">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="60fff-549">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="60fff-550">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="60fff-550">General availability applies to these command modules:</span></span>
- <span data-ttu-id="60fff-551">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="60fff-551">Container Service (acs)</span></span>
- <span data-ttu-id="60fff-552">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="60fff-552">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="60fff-553">Redes</span><span class="sxs-lookup"><span data-stu-id="60fff-553">Networking</span></span>
- <span data-ttu-id="60fff-554">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="60fff-554">Storage</span></span>

<span data-ttu-id="60fff-555">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60fff-555">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="60fff-556">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="60fff-556">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="60fff-557">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="60fff-557">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="60fff-558">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="60fff-558">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="60fff-559">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="60fff-559">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="60fff-560">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="60fff-560">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="60fff-561">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="60fff-561">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="60fff-562">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="60fff-562">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="60fff-563">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="60fff-563">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="60fff-564">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="60fff-564">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="60fff-565">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="60fff-565">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="60fff-566">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="60fff-566">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="60fff-567">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="60fff-567">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="60fff-568">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="60fff-568">Provide feedback from the command line with the `az feedback` command.</span></span>

