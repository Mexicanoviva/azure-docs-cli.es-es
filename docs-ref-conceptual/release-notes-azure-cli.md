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
ms.openlocfilehash: 39e4710a29ac57730919b82ab76b9c9a4b9ca786
ms.sourcegitcommit: 43d4f838d132ab9bcfa59dbda3b544c06373b6a9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/22/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="ee7b6-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="ee7b6-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-15-2017"></a><span data-ttu-id="ee7b6-105">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ee7b6-105">August 15, 2017</span></span>

<span data-ttu-id="ee7b6-106">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ee7b6-106">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ee7b6-107">ACS</span><span class="sxs-lookup"><span data-stu-id="ee7b6-107">ACS</span></span>

* <span data-ttu-id="ee7b6-108">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="ee7b6-108">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ee7b6-109">Appservice</span><span class="sxs-lookup"><span data-stu-id="ee7b6-109">Appservice</span></span>

* <span data-ttu-id="ee7b6-110">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-110">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ee7b6-111">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ee7b6-111">Event Grid</span></span>

* <span data-ttu-id="ee7b6-112">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-112">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ee7b6-113">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ee7b6-113">August 11, 2017</span></span>

<span data-ttu-id="ee7b6-114">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ee7b6-114">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ee7b6-115">ACS</span><span class="sxs-lookup"><span data-stu-id="ee7b6-115">ACS</span></span>

* <span data-ttu-id="ee7b6-116">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ee7b6-116">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ee7b6-117">Batch</span><span class="sxs-lookup"><span data-stu-id="ee7b6-117">Batch</span></span>

* <span data-ttu-id="ee7b6-118">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-118">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ee7b6-119">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-119">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ee7b6-120">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-120">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ee7b6-121">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-121">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ee7b6-122">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-122">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ee7b6-123">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-123">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ee7b6-124">Componente</span><span class="sxs-lookup"><span data-stu-id="ee7b6-124">Component</span></span>

* <span data-ttu-id="ee7b6-125">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-125">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ee7b6-126">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ee7b6-126">Container</span></span>

* <span data-ttu-id="ee7b6-127">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-127">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ee7b6-128">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ee7b6-128">Data Lake Store</span></span>

* <span data-ttu-id="ee7b6-129">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-129">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ee7b6-130">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ee7b6-130">Event Grid</span></span>

* <span data-ttu-id="ee7b6-131">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-131">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ee7b6-132">Red</span><span class="sxs-lookup"><span data-stu-id="ee7b6-132">Network</span></span>

* <span data-ttu-id="ee7b6-133">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-133">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ee7b6-134">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-134">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ee7b6-135">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-135">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ee7b6-136">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-136">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ee7b6-137">Perfil</span><span class="sxs-lookup"><span data-stu-id="ee7b6-137">Profile</span></span>

* <span data-ttu-id="ee7b6-138">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-138">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ee7b6-139">Storage</span><span class="sxs-lookup"><span data-stu-id="ee7b6-139">Storage</span></span>

* <span data-ttu-id="ee7b6-140">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-140">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ee7b6-141">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ee7b6-141">VM</span></span>

* <span data-ttu-id="ee7b6-142">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-142">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ee7b6-143">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-143">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ee7b6-144">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-144">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ee7b6-145">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-145">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ee7b6-146">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-146">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ee7b6-147">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="ee7b6-147">July 28, 2017</span></span>

<span data-ttu-id="ee7b6-148">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ee7b6-148">Version 2.0.12</span></span>

* <span data-ttu-id="ee7b6-149">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-149">Added container commands</span></span>
* <span data-ttu-id="ee7b6-150">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-150">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ee7b6-151">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ee7b6-151">Core</span></span>

* <span data-ttu-id="ee7b6-152">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-152">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ee7b6-153">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-153">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ee7b6-154">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-154">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ee7b6-155">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-155">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ee7b6-156">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-156">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ee7b6-157">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-157">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ee7b6-158">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-158">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ee7b6-159">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-159">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ee7b6-160">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-160">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ee7b6-161">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-161">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ee7b6-162">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-162">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ee7b6-163">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-163">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ee7b6-164">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-164">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ee7b6-165">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-165">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ee7b6-166">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-166">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ee7b6-167">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-167">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ee7b6-168">ACR</span><span class="sxs-lookup"><span data-stu-id="ee7b6-168">ACR</span></span>

* <span data-ttu-id="ee7b6-169">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-169">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ee7b6-170">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-170">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ee7b6-171">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-171">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ee7b6-172">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-172">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ee7b6-173">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-173">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ee7b6-174">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-174">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ee7b6-175">ACS</span><span class="sxs-lookup"><span data-stu-id="ee7b6-175">ACS</span></span>

* <span data-ttu-id="ee7b6-176">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-176">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ee7b6-177">Appservice</span><span class="sxs-lookup"><span data-stu-id="ee7b6-177">Appservice</span></span>

* <span data-ttu-id="ee7b6-178">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-178">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ee7b6-179">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-179">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ee7b6-180">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-180">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ee7b6-181">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-181">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ee7b6-182">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-182">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ee7b6-183">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-183">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ee7b6-184">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-184">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ee7b6-185">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-185">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ee7b6-186">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-186">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ee7b6-187">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-187">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ee7b6-188">Batch</span><span class="sxs-lookup"><span data-stu-id="ee7b6-188">Batch</span></span>

* <span data-ttu-id="ee7b6-189">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-189">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ee7b6-190">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-190">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ee7b6-191">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-191">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ee7b6-192">CDN</span><span class="sxs-lookup"><span data-stu-id="ee7b6-192">CDN</span></span>

* <span data-ttu-id="ee7b6-193">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-193">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="ee7b6-194">Nube</span><span class="sxs-lookup"><span data-stu-id="ee7b6-194">Cloud</span></span>

* <span data-ttu-id="ee7b6-195">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-195">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ee7b6-196">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-196">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ee7b6-197">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-197">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ee7b6-198">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-198">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ee7b6-199">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-199">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ee7b6-200">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ee7b6-200">CosmosDB</span></span>

* <span data-ttu-id="ee7b6-201">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-201">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ee7b6-202">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-202">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ee7b6-203">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ee7b6-203">Data Lake Analytics</span></span>

* <span data-ttu-id="ee7b6-204">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-204">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ee7b6-205">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-205">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ee7b6-206">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-206">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ee7b6-207">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ee7b6-207">Data Lake Store</span></span>

* <span data-ttu-id="ee7b6-208">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-208">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ee7b6-209">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-209">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ee7b6-210">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-210">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ee7b6-211">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-211">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ee7b6-212">Interactive</span><span class="sxs-lookup"><span data-stu-id="ee7b6-212">Interactive</span></span>

* <span data-ttu-id="ee7b6-213">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-213">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ee7b6-214">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-214">Increased test coverage</span></span>
* <span data-ttu-id="ee7b6-215">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-215">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ee7b6-216">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-216">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ee7b6-217">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-217">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ee7b6-218">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-218">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ee7b6-219">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-219">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ee7b6-220">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-220">Added `--progress` flag</span></span>
* <span data-ttu-id="ee7b6-221">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-221">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ee7b6-222">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-222">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ee7b6-223">IoT</span><span class="sxs-lookup"><span data-stu-id="ee7b6-223">IoT</span></span>

* <span data-ttu-id="ee7b6-224">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-224">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ee7b6-225">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="ee7b6-225">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ee7b6-226">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="ee7b6-226">Key vault</span></span>

* <span data-ttu-id="ee7b6-227">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="ee7b6-227">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ee7b6-228">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-228">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ee7b6-229">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-229">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ee7b6-230">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-230">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ee7b6-231">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-231">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ee7b6-232">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-232">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ee7b6-233">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="ee7b6-233">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ee7b6-234">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-234">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ee7b6-235">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="ee7b6-235">Lab</span></span>

* <span data-ttu-id="ee7b6-236">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-236">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ee7b6-237">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-237">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ee7b6-238">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ee7b6-238">Monitor</span></span>

* <span data-ttu-id="ee7b6-239">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-239">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ee7b6-240">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-240">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ee7b6-241">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-241">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ee7b6-242">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-242">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ee7b6-243">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-243">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ee7b6-244">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="ee7b6-244">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ee7b6-245">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-245">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ee7b6-246">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-246">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ee7b6-247">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-247">`location` no longer required</span></span>
  * <span data-ttu-id="ee7b6-248">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-248">Add name and ID support for target</span></span>
  * <span data-ttu-id="ee7b6-249">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-249">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ee7b6-250">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-250">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ee7b6-251">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-251">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ee7b6-252">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-252">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ee7b6-253">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-253">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ee7b6-254">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-254">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ee7b6-255">Red</span><span class="sxs-lookup"><span data-stu-id="ee7b6-255">Network</span></span>

* <span data-ttu-id="ee7b6-256">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-256">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ee7b6-257">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-257">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ee7b6-258">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-258">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ee7b6-259">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-259">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ee7b6-260">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-260">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ee7b6-261">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-261">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ee7b6-262">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-262">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ee7b6-263">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-263">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ee7b6-264">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-264">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ee7b6-265">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-265">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ee7b6-266">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-266">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ee7b6-267">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-267">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ee7b6-268">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-268">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ee7b6-269">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-269">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ee7b6-270">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-270">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ee7b6-271">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-271">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ee7b6-272">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-272">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ee7b6-273">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-273">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ee7b6-274">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-274">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ee7b6-275">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-275">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ee7b6-276">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-276">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ee7b6-277">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-277">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ee7b6-278">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-278">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ee7b6-279">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-279">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ee7b6-280">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-280">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ee7b6-281">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-281">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ee7b6-282">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-282">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ee7b6-283">Perfil</span><span class="sxs-lookup"><span data-stu-id="ee7b6-283">Profile</span></span>

* <span data-ttu-id="ee7b6-284">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-284">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ee7b6-285">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-285">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ee7b6-286">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="ee7b6-286">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ee7b6-287">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-287">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ee7b6-288">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-288">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ee7b6-289">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ee7b6-289">RDBMS</span></span>

* <span data-ttu-id="ee7b6-290">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-290">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ee7b6-291">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-291">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ee7b6-292">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-292">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ee7b6-293">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-293">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ee7b6-294">Recurso</span><span class="sxs-lookup"><span data-stu-id="ee7b6-294">Resource</span></span>

* <span data-ttu-id="ee7b6-295">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-295">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ee7b6-296">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-296">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ee7b6-297">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-297">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ee7b6-298">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-298">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ee7b6-299">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-299">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ee7b6-300">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-300">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ee7b6-301">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-301">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ee7b6-302">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-302">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ee7b6-303">Rol</span><span class="sxs-lookup"><span data-stu-id="ee7b6-303">Role</span></span>

* <span data-ttu-id="ee7b6-304">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-304">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ee7b6-305">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-305">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ee7b6-306">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-306">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ee7b6-307">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-307">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ee7b6-308">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-308">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ee7b6-309">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ee7b6-309">Service Fabric</span></span>
* <span data-ttu-id="ee7b6-310">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-310">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ee7b6-311">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-311">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ee7b6-312">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-312">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ee7b6-313">SQL</span><span class="sxs-lookup"><span data-stu-id="ee7b6-313">SQL</span></span>

* <span data-ttu-id="ee7b6-314">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-314">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ee7b6-315">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-315">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ee7b6-316">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-316">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ee7b6-317">Storage</span><span class="sxs-lookup"><span data-stu-id="ee7b6-317">Storage</span></span>

* <span data-ttu-id="ee7b6-318">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-318">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ee7b6-319">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-319">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ee7b6-320">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-320">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ee7b6-321">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-321">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="ee7b6-322">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-322">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="ee7b6-323">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-323">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ee7b6-324">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ee7b6-324">VM</span></span>

* <span data-ttu-id="ee7b6-325">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="ee7b6-325">Support configuring nsg</span></span>
* <span data-ttu-id="ee7b6-326">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-326">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ee7b6-327">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-327">Support managed service identities</span></span>
* <span data-ttu-id="ee7b6-328">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-328">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="ee7b6-329">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="ee7b6-329">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ee7b6-330">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="ee7b6-330">May 10, 2017</span></span>

<span data-ttu-id="ee7b6-331">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ee7b6-331">Version 2.0.6</span></span>

* <span data-ttu-id="ee7b6-332">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-332">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ee7b6-333">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-333">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ee7b6-334">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-334">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="ee7b6-335">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-335">Include Cognitive Services module.</span></span>
* <span data-ttu-id="ee7b6-336">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-336">Include Service Fabric module.</span></span>
* <span data-ttu-id="ee7b6-337">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-337">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="ee7b6-338">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-338">Add support for CDN commands.</span></span>
* <span data-ttu-id="ee7b6-339">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-339">Remove Container module.</span></span>
* <span data-ttu-id="ee7b6-340">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-340">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ee7b6-341">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-341">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ee7b6-342">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ee7b6-342">Core</span></span>

* <span data-ttu-id="ee7b6-343">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="ee7b6-343">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="ee7b6-344">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-344">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ee7b6-345">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-345">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ee7b6-346">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-346">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ee7b6-347">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-347">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ee7b6-348">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-348">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ee7b6-349">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-349">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ee7b6-350">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-350">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ee7b6-351">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-351">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ee7b6-352">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="ee7b6-352">core: Improved performance</span></span>
* <span data-ttu-id="ee7b6-353">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="ee7b6-353">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ee7b6-354">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="ee7b6-354">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ee7b6-355">ACS</span><span class="sxs-lookup"><span data-stu-id="ee7b6-355">ACS</span></span>

* <span data-ttu-id="ee7b6-356">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="ee7b6-356">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ee7b6-357">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="ee7b6-357">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ee7b6-358">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="ee7b6-358">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ee7b6-359">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-359">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ee7b6-360">AppService</span><span class="sxs-lookup"><span data-stu-id="ee7b6-360">AppService</span></span>

* <span data-ttu-id="ee7b6-361">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-361">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ee7b6-362">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="ee7b6-362">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ee7b6-363">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="ee7b6-363">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ee7b6-364">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="ee7b6-364">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ee7b6-365">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="ee7b6-365">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ee7b6-366">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-366">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ee7b6-367">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ee7b6-367">support slot swap with preview</span></span>
* <span data-ttu-id="ee7b6-368">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-368">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ee7b6-369">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-369">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ee7b6-370">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ee7b6-370">CosmosDB</span></span>

* <span data-ttu-id="ee7b6-371">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ee7b6-371">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="ee7b6-372">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="ee7b6-372">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ee7b6-373">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="ee7b6-373">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ee7b6-374">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="ee7b6-374">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ee7b6-375">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ee7b6-375">Data Lake Analytics</span></span>

* <span data-ttu-id="ee7b6-376">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="ee7b6-376">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="ee7b6-377">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="ee7b6-377">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ee7b6-378">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-378">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ee7b6-379">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="ee7b6-379">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ee7b6-380">Tabla</span><span class="sxs-lookup"><span data-stu-id="ee7b6-380">Table</span></span>
  * <span data-ttu-id="ee7b6-381">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="ee7b6-381">Table valued function</span></span>
  * <span data-ttu-id="ee7b6-382">Ver</span><span class="sxs-lookup"><span data-stu-id="ee7b6-382">View</span></span>
  * <span data-ttu-id="ee7b6-383">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-383">Table Statistics.</span></span> <span data-ttu-id="ee7b6-384">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="ee7b6-384">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ee7b6-385">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ee7b6-385">Data Lake Store</span></span>

* <span data-ttu-id="ee7b6-386">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-386">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="ee7b6-387">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-387">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ee7b6-388">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-388">missed help for access show.</span></span> <span data-ttu-id="ee7b6-389">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-389">adding it.</span></span> <span data-ttu-id="ee7b6-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ee7b6-391">Buscar</span><span class="sxs-lookup"><span data-stu-id="ee7b6-391">Find</span></span>

* <span data-ttu-id="ee7b6-392">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="ee7b6-392">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ee7b6-393">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ee7b6-393">KeyVault</span></span>

* <span data-ttu-id="ee7b6-394">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="ee7b6-394">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ee7b6-395">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="ee7b6-395">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="ee7b6-396">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="ee7b6-396">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ee7b6-397">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="ee7b6-397">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="ee7b6-398">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-398">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ee7b6-399">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="ee7b6-399">Lab</span></span>

* <span data-ttu-id="ee7b6-400">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="ee7b6-400">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="ee7b6-401">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="ee7b6-401">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="ee7b6-402">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="ee7b6-402">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="ee7b6-403">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="ee7b6-403">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="ee7b6-404">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="ee7b6-404">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="ee7b6-405">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ee7b6-405">Monitor</span></span>

* <span data-ttu-id="ee7b6-406">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-406">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ee7b6-407">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-407">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ee7b6-408">Red</span><span class="sxs-lookup"><span data-stu-id="ee7b6-408">Network</span></span>

* <span data-ttu-id="ee7b6-409">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-409">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="ee7b6-410">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-410">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="ee7b6-411">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="ee7b6-411">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="ee7b6-412">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="ee7b6-412">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="ee7b6-413">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="ee7b6-413">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="ee7b6-414">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ee7b6-414">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="ee7b6-415">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="ee7b6-415">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="ee7b6-416">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="ee7b6-416">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="ee7b6-417">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-417">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="ee7b6-418">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="ee7b6-418">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ee7b6-419">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-419">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="ee7b6-420">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-420">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="ee7b6-421">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="ee7b6-421">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="ee7b6-422">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="ee7b6-422">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="ee7b6-423">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="ee7b6-423">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="ee7b6-424">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="ee7b6-424">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="ee7b6-425">Perfil</span><span class="sxs-lookup"><span data-stu-id="ee7b6-425">Profile</span></span>

* <span data-ttu-id="ee7b6-426">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-426">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ee7b6-427">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-427">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ee7b6-428">Redis</span><span class="sxs-lookup"><span data-stu-id="ee7b6-428">Redis</span></span>

* <span data-ttu-id="ee7b6-429">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="ee7b6-429">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ee7b6-430">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="ee7b6-430">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="ee7b6-431">Recurso</span><span class="sxs-lookup"><span data-stu-id="ee7b6-431">Resource</span></span>

* <span data-ttu-id="ee7b6-432">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-432">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ee7b6-433">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-433">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ee7b6-434">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-434">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ee7b6-435">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="ee7b6-435">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ee7b6-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ee7b6-437">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="ee7b6-437">Add docs for az lock update.</span></span> <span data-ttu-id="ee7b6-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ee7b6-439">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="ee7b6-439">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ee7b6-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ee7b6-441">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="ee7b6-441">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ee7b6-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ee7b6-443">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-443">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ee7b6-444">Rol</span><span class="sxs-lookup"><span data-stu-id="ee7b6-444">Role</span></span>

* <span data-ttu-id="ee7b6-445">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-445">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ee7b6-446">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-446">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ee7b6-447">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-447">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ee7b6-448">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="ee7b6-448">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ee7b6-449">SQL</span><span class="sxs-lookup"><span data-stu-id="ee7b6-449">SQL</span></span>

* <span data-ttu-id="ee7b6-450">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="ee7b6-450">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="ee7b6-451">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-451">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ee7b6-452">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="ee7b6-452">Storage</span></span>

* <span data-ttu-id="ee7b6-453">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="ee7b6-453">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="ee7b6-454">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="ee7b6-454">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ee7b6-455">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="ee7b6-455">Add support for large block blob upload</span></span>
* <span data-ttu-id="ee7b6-456">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="ee7b6-456">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ee7b6-457">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ee7b6-457">VM</span></span>

* <span data-ttu-id="ee7b6-458">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="ee7b6-458">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ee7b6-459">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="ee7b6-459">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ee7b6-460">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ee7b6-460">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ee7b6-461">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ee7b6-461">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ee7b6-462">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="ee7b6-462">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ee7b6-463">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="ee7b6-463">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ee7b6-464">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-464">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ee7b6-465">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="ee7b6-465">April 3, 2017</span></span>

<span data-ttu-id="ee7b6-466">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ee7b6-466">Version 2.0.2</span></span>

<span data-ttu-id="ee7b6-467">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-467">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="ee7b6-468">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ee7b6-468">Core</span></span>

* <span data-ttu-id="ee7b6-469">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-469">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="ee7b6-470">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-470">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ee7b6-471">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-471">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ee7b6-472">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-472">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ee7b6-473">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-473">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ee7b6-474">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-474">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ee7b6-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ee7b6-476">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="ee7b6-476">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ee7b6-477">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="ee7b6-477">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="ee7b6-478">ACS</span><span class="sxs-lookup"><span data-stu-id="ee7b6-478">ACS</span></span>

* <span data-ttu-id="ee7b6-479">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-479">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ee7b6-480">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-480">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ee7b6-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ee7b6-482">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-482">Add support for windows clusters.</span></span> <span data-ttu-id="ee7b6-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ee7b6-484">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-484">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ee7b6-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="ee7b6-486">AppService</span><span class="sxs-lookup"><span data-stu-id="ee7b6-486">AppService</span></span>

* <span data-ttu-id="ee7b6-487">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-487">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ee7b6-488">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-488">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ee7b6-489">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-489">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ee7b6-490">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-490">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="ee7b6-491">DataLake</span><span class="sxs-lookup"><span data-stu-id="ee7b6-491">DataLake</span></span>

* <span data-ttu-id="ee7b6-492">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-492">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="ee7b6-493">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-493">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="ee7b6-494">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ee7b6-494">DocuemntDB</span></span>

* <span data-ttu-id="ee7b6-495">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-495">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ee7b6-496">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ee7b6-496">VM</span></span>

* <span data-ttu-id="ee7b6-497">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-497">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ee7b6-498">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-498">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ee7b6-499">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-499">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ee7b6-500">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-500">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ee7b6-501">Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-501">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ee7b6-502">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-502">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="ee7b6-503">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="ee7b6-503">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ee7b6-504">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="ee7b6-504">February 27, 2017</span></span>

<span data-ttu-id="ee7b6-505">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ee7b6-505">Version 2.0.0</span></span>

<span data-ttu-id="ee7b6-506">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-506">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="ee7b6-507">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="ee7b6-507">General availability applies to these command modules:</span></span>
- <span data-ttu-id="ee7b6-508">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="ee7b6-508">Container Service (acs)</span></span>
- <span data-ttu-id="ee7b6-509">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="ee7b6-509">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ee7b6-510">Redes</span><span class="sxs-lookup"><span data-stu-id="ee7b6-510">Networking</span></span>
- <span data-ttu-id="ee7b6-511">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="ee7b6-511">Storage</span></span>

<span data-ttu-id="ee7b6-512">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-512">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="ee7b6-513">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-513">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="ee7b6-514">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-514">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="ee7b6-515">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-515">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="ee7b6-516">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-516">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="ee7b6-517">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-517">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="ee7b6-518">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="ee7b6-518">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="ee7b6-519">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-519">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="ee7b6-520">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-520">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="ee7b6-521">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-521">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="ee7b6-522">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="ee7b6-522">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ee7b6-523">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="ee7b6-523">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ee7b6-524">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="ee7b6-524">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="ee7b6-525">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ee7b6-525">Provide feedback from the command line with the `az feedback` command.</span></span>

