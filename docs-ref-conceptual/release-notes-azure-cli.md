---
title: Notas de la versión de la CLI de Azure 2.0
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 1e6bd4cd8bab853fb417ed9c4dd71d56e5de7cdc
ms.sourcegitcommit: 204fd027d3668959b98b936969ccb41eada0fd29
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/16/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="4c0d8-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="4c0d8-103">Azure CLI 2.0 release notes</span></span>

## <a name="april-10-2018"></a><span data-ttu-id="4c0d8-104">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="4c0d8-104">April 10, 2018</span></span>

<span data-ttu-id="4c0d8-105">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="4c0d8-105">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="4c0d8-106">ACR</span><span class="sxs-lookup"><span data-stu-id="4c0d8-106">ACR</span></span>

* <span data-ttu-id="4c0d8-107">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="4c0d8-107">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-108">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-108">ACS</span></span>

* <span data-ttu-id="4c0d8-109">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="4c0d8-109">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-110">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-110">Appservice</span></span>

* <span data-ttu-id="4c0d8-111">[[CAMBIO IMPORTANTE]]: Removed `assign-identity`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-111">[BREAKING CHANGE]: Removed `assign-identity`</span></span>
* <span data-ttu-id="4c0d8-112">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-112">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="4c0d8-113">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-113">BatchAI</span></span>

* <span data-ttu-id="4c0d8-114">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="4c0d8-114">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="4c0d8-115">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-115">Job level mounting</span></span>
 - <span data-ttu-id="4c0d8-116">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="4c0d8-116">Environment variables with secret values</span></span>
 - <span data-ttu-id="4c0d8-117">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="4c0d8-117">Performance counters settings</span></span>
 - <span data-ttu-id="4c0d8-118">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-118">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="4c0d8-119">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-119">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="4c0d8-120">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-120">Usage and limits reporting</span></span>
 - <span data-ttu-id="4c0d8-121">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-121">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="4c0d8-122">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-122">Support for custom images</span></span>
 - <span data-ttu-id="4c0d8-123">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-123">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="4c0d8-124">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-124">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="4c0d8-125">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="4c0d8-125">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="4c0d8-126">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="4c0d8-126">National clouds are supported</span></span>
* <span data-ttu-id="4c0d8-127">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="4c0d8-127">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="4c0d8-128">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="4c0d8-128">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="4c0d8-129">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-129">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="4c0d8-130">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-130">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="4c0d8-131">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-131">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="4c0d8-132">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-132">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="4c0d8-133">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-133">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="4c0d8-134">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-134">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="4c0d8-135">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="4c0d8-135">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="4c0d8-136">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-136">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="4c0d8-137">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-137">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="4c0d8-138">[[CAMBIO IMPORTANTE]] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-138">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="4c0d8-139">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-139">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="4c0d8-140">Facturación</span><span class="sxs-lookup"><span data-stu-id="4c0d8-140">Billing</span></span>

* <span data-ttu-id="4c0d8-141">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="4c0d8-141">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="4c0d8-142">Consumo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-142">Consumption</span></span>

* <span data-ttu-id="4c0d8-143">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-143">Added `marketplace` commands</span></span>
* <span data-ttu-id="4c0d8-144">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-144">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="4c0d8-145">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-145">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="4c0d8-146">[[CAMBIO IMPORTANTE]] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-146">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="4c0d8-147">[[CAMBIO IMPORTANTE]] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-147">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="4c0d8-148">[[CAMBIO IMPORTANTE]] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-148">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-149">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-149">Container</span></span>

* <span data-ttu-id="4c0d8-150">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-150">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="4c0d8-151">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="4c0d8-151">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="4c0d8-152">Extensión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-152">Extension</span></span>

* <span data-ttu-id="4c0d8-153">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="4c0d8-153">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="4c0d8-154">Interactive</span><span class="sxs-lookup"><span data-stu-id="4c0d8-154">Interactive</span></span>

* <span data-ttu-id="4c0d8-155">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-155">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="4c0d8-156">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-156">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="4c0d8-157">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-157">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-158">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-158">Network</span></span>

* <span data-ttu-id="4c0d8-159">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-159">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="4c0d8-160">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-160">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="4c0d8-161">4910</span><span class="sxs-lookup"><span data-stu-id="4c0d8-161">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="4c0d8-162">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="4c0d8-162">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="4c0d8-163">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="4c0d8-163">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="4c0d8-164">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-164">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="4c0d8-165">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-165">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="4c0d8-166">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-166">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-167">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-167">Profile</span></span>

* <span data-ttu-id="4c0d8-168">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-168">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="4c0d8-169">[[CAMBIO IMPORTANTE]] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-169">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="4c0d8-170">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-170">RDBMS</span></span>

* <span data-ttu-id="4c0d8-171">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-171">Added `georestore` command</span></span>
* <span data-ttu-id="4c0d8-172">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-172">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-173">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-173">Resource</span></span>

* <span data-ttu-id="4c0d8-174">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-174">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="4c0d8-175">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-175">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-176">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-176">SQL</span></span>

* <span data-ttu-id="4c0d8-177">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-177">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-178">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-178">Storage</span></span>

* <span data-ttu-id="4c0d8-179">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="4c0d8-179">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-180">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-180">VM</span></span>

* <span data-ttu-id="4c0d8-181">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-181">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="4c0d8-182">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="4c0d8-182">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="4c0d8-184">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-184">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="4c0d8-185">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-185">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="4c0d8-186">5718</span><span class="sxs-lookup"><span data-stu-id="4c0d8-186">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="4c0d8-187">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-187">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="4c0d8-188">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="4c0d8-188">March 27, 2018</span></span>

<span data-ttu-id="4c0d8-189">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="4c0d8-189">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-190">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-190">Core</span></span>

* <span data-ttu-id="4c0d8-191">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="4c0d8-191">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-192">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-192">ACS</span></span>

* <span data-ttu-id="4c0d8-193">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4c0d8-193">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-194">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-194">Appservice</span></span>

* <span data-ttu-id="4c0d8-195">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-195">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="4c0d8-196">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-196">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4c0d8-197">Backup</span><span class="sxs-lookup"><span data-stu-id="4c0d8-197">Backup</span></span>

* <span data-ttu-id="4c0d8-198">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-198">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="4c0d8-199">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-199">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="4c0d8-200">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-200">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="4c0d8-201">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-201">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-202">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-202">Container</span></span>

* <span data-ttu-id="4c0d8-203">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-203">Added `container exec` command.</span></span> <span data-ttu-id="4c0d8-204">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="4c0d8-204">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="4c0d8-205">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="4c0d8-205">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4c0d8-206">Extensión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-206">Extension</span></span>

* <span data-ttu-id="4c0d8-207">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-207">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="4c0d8-208">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-208">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="4c0d8-209">[[CAMBIO IMPORTANTE]] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="4c0d8-209">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="4c0d8-210">Interactive</span><span class="sxs-lookup"><span data-stu-id="4c0d8-210">Interactive</span></span>

* <span data-ttu-id="4c0d8-211">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-211">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="4c0d8-212">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-212">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="4c0d8-213">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-213">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="4c0d8-214">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="4c0d8-214">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="4c0d8-215">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-215">Lab</span></span>

* <span data-ttu-id="4c0d8-216">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-216">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-217">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-217">Monitor</span></span>

* <span data-ttu-id="4c0d8-218">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-218">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="4c0d8-219">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-219">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="4c0d8-220">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-220">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-221">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-221">Network</span></span>

* <span data-ttu-id="4c0d8-222">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-222">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-223">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-223">Profile</span></span>

* <span data-ttu-id="4c0d8-224">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-224">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4c0d8-225">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-225">RDBMS</span></span>

* <span data-ttu-id="4c0d8-226">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="4c0d8-226">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-227">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-227">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="4c0d8-229">Rol</span><span class="sxs-lookup"><span data-stu-id="4c0d8-229">Role</span></span>

* <span data-ttu-id="4c0d8-230">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-230">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="4c0d8-231">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="4c0d8-231">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="4c0d8-232">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-232">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="4c0d8-233">[[CAMBIO IMPORTANTE]] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-233">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="4c0d8-234">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-234">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-235">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-235">Storage</span></span>

* <span data-ttu-id="4c0d8-236">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-236">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="4c0d8-237">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="4c0d8-237">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-238">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-238">VM</span></span>

* <span data-ttu-id="4c0d8-239">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="4c0d8-239">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="4c0d8-240">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-240">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="4c0d8-241">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="4c0d8-241">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="4c0d8-242">[[CAMBIO IMPORTANTE]] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="4c0d8-242">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="4c0d8-243">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="4c0d8-243">March 13, 2018</span></span>

<span data-ttu-id="4c0d8-244">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="4c0d8-244">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="4c0d8-245">ACR</span><span class="sxs-lookup"><span data-stu-id="4c0d8-245">ACR</span></span>

* <span data-ttu-id="4c0d8-246">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-246">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="4c0d8-247">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-247">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="4c0d8-248">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-248">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-249">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-249">ACS</span></span>

* <span data-ttu-id="4c0d8-250">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-250">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="4c0d8-251">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-251">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="4c0d8-252">Advisor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-252">Advisor</span></span>

* <span data-ttu-id="4c0d8-253">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-253">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="4c0d8-254">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-254">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="4c0d8-255">[[CAMBIO IMPORTANTE]] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-255">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="4c0d8-256">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-256">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="4c0d8-257">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-257">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-258">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-258">Appservice</span></span>

* <span data-ttu-id="4c0d8-259">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-259">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="4c0d8-260">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-260">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4c0d8-261">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="4c0d8-261">Eventhubs</span></span>

* <span data-ttu-id="4c0d8-262">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-262">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="4c0d8-263">Extensión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-263">Extension</span></span>

* <span data-ttu-id="4c0d8-264">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-264">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="4c0d8-265">Interactive</span><span class="sxs-lookup"><span data-stu-id="4c0d8-265">Interactive</span></span>

* <span data-ttu-id="4c0d8-266">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-266">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="4c0d8-267">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-267">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="4c0d8-268">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-268">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="4c0d8-269">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-269">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-270">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-270">Monitor</span></span>

* <span data-ttu-id="4c0d8-271">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-271">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="4c0d8-272">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-272">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="4c0d8-273">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-273">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="4c0d8-274">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-274">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-275">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-275">Network</span></span>

* <span data-ttu-id="4c0d8-276">[[CAMBIO IMPORTANTE]] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-276">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="4c0d8-277">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-277">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="4c0d8-278">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-278">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="4c0d8-279">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-279">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-280">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-280">Profile</span></span>

* <span data-ttu-id="4c0d8-281">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-281">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="4c0d8-282">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-282">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4c0d8-283">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-283">RDBMS</span></span>

* <span data-ttu-id="4c0d8-284">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="4c0d8-284">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="4c0d8-285">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="4c0d8-285">Service Bus</span></span>

* <span data-ttu-id="4c0d8-286">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-286">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-287">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-287">Storage</span></span>

* <span data-ttu-id="4c0d8-288">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-288">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="4c0d8-289">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-289">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-290">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-290">VM</span></span>

* <span data-ttu-id="4c0d8-291">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-291">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="4c0d8-292">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-292">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="4c0d8-293">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-293">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="4c0d8-294">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-294">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="4c0d8-295">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="4c0d8-295">February 27, 2018</span></span>

<span data-ttu-id="4c0d8-296">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="4c0d8-296">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-297">Core</span></span>

* <span data-ttu-id="4c0d8-298">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="4c0d8-298">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="4c0d8-299">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-299">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="4c0d8-300">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-300">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-301">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-301">ACS</span></span>

* <span data-ttu-id="4c0d8-302">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="4c0d8-302">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="4c0d8-303">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-303">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="4c0d8-304">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-304">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="4c0d8-305">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-305">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-306">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-306">Appservice</span></span>

* <span data-ttu-id="4c0d8-307">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-307">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="4c0d8-308">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="4c0d8-308">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4c0d8-309">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4c0d8-309">Cognitive Services</span></span>

* <span data-ttu-id="4c0d8-310">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4c0d8-310">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="4c0d8-311">Consumo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-311">Consumption</span></span>

* <span data-ttu-id="4c0d8-312">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="4c0d8-312">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="4c0d8-313">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="4c0d8-313">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-314">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-314">Container</span></span>

* <span data-ttu-id="4c0d8-315">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-315">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-316">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-316">Network</span></span>

* <span data-ttu-id="4c0d8-317">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-317">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-318">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-318">Resource</span></span>

* <span data-ttu-id="4c0d8-319">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="4c0d8-319">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="4c0d8-320">Rol</span><span class="sxs-lookup"><span data-stu-id="4c0d8-320">Role</span></span>

* <span data-ttu-id="4c0d8-321">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-321">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-322">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-322">SQL</span></span>

* <span data-ttu-id="4c0d8-323">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="4c0d8-323">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-324">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-324">Storage</span></span>

* <span data-ttu-id="4c0d8-325">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-325">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-326">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-326">VM</span></span>

* <span data-ttu-id="4c0d8-327">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-327">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="4c0d8-328">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="4c0d8-328">February 13, 2018</span></span>

<span data-ttu-id="4c0d8-329">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="4c0d8-329">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-330">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-330">Core</span></span>

* <span data-ttu-id="4c0d8-331">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="4c0d8-331">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-332">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-332">ACS</span></span>

* <span data-ttu-id="4c0d8-333">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-333">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="4c0d8-334">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-334">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="4c0d8-335">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-335">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="4c0d8-336">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-336">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="4c0d8-337">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-337">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="4c0d8-338">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-338">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="4c0d8-339">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-339">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="4c0d8-340">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-340">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-341">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-341">Appservice</span></span>

* <span data-ttu-id="4c0d8-342">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="4c0d8-342">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="4c0d8-343">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-343">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="4c0d8-344">CDN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-344">CDN</span></span>

* <span data-ttu-id="4c0d8-345">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-345">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-346">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-346">Container</span></span>

* <span data-ttu-id="4c0d8-347">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="4c0d8-347">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="4c0d8-348">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="4c0d8-348">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4c0d8-349">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-349">CosmosDB</span></span>

* <span data-ttu-id="4c0d8-350">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="4c0d8-350">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="4c0d8-351">Extensión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-351">Extension</span></span>

* <span data-ttu-id="4c0d8-352">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-352">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="4c0d8-353">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-353">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="4c0d8-354">Comentarios</span><span class="sxs-lookup"><span data-stu-id="4c0d8-354">Feedback</span></span>

* <span data-ttu-id="4c0d8-355">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="4c0d8-355">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="4c0d8-356">Interactive</span><span class="sxs-lookup"><span data-stu-id="4c0d8-356">Interactive</span></span>

* <span data-ttu-id="4c0d8-357">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4c0d8-357">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="4c0d8-358">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="4c0d8-358">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="4c0d8-359">IoT</span><span class="sxs-lookup"><span data-stu-id="4c0d8-359">IoT</span></span>

* <span data-ttu-id="4c0d8-360">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-360">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4c0d8-361">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-361">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4c0d8-362">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-362">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="4c0d8-363">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="4c0d8-363">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-364">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-364">Monitor</span></span>

* <span data-ttu-id="4c0d8-365">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-365">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-366">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-366">Network</span></span>

* <span data-ttu-id="4c0d8-367">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-367">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="4c0d8-368">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-368">Profile</span></span>

* <span data-ttu-id="4c0d8-369">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-369">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-370">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-370">Resource</span></span>

* <span data-ttu-id="4c0d8-371">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-371">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="4c0d8-372">Rol</span><span class="sxs-lookup"><span data-stu-id="4c0d8-372">Role</span></span>

* <span data-ttu-id="4c0d8-373">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-373">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-374">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-374">SQL</span></span>

* <span data-ttu-id="4c0d8-375">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-375">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="4c0d8-376">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-376">Added `sql db rename`</span></span>
* <span data-ttu-id="4c0d8-377">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="4c0d8-377">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-378">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-378">Storage</span></span>

* <span data-ttu-id="4c0d8-379">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="4c0d8-379">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-380">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-380">VM</span></span>

* <span data-ttu-id="4c0d8-381">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="4c0d8-381">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="4c0d8-382">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-382">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="4c0d8-383">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="4c0d8-383">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="4c0d8-384">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="4c0d8-384">January 31, 2018</span></span>

<span data-ttu-id="4c0d8-385">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="4c0d8-385">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-386">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-386">Core</span></span>

* <span data-ttu-id="4c0d8-387">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-387">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="4c0d8-388">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="4c0d8-388">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="4c0d8-389">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-389">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="4c0d8-390">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-390">Use `--verbose` to see</span></span>
* <span data-ttu-id="4c0d8-391">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="4c0d8-391">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-392">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-392">ACS</span></span>

* <span data-ttu-id="4c0d8-393">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-393">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="4c0d8-394">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-394">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-395">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-395">Appservice</span></span>

* <span data-ttu-id="4c0d8-396">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="4c0d8-396">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="4c0d8-397">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="4c0d8-397">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="4c0d8-398">CDN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-398">CDN</span></span>

* <span data-ttu-id="4c0d8-399">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-399">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4c0d8-400">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-400">CosmosDB</span></span>

* <span data-ttu-id="4c0d8-401">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="4c0d8-401">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="4c0d8-402">Interactive</span><span class="sxs-lookup"><span data-stu-id="4c0d8-402">Interactive</span></span>

* <span data-ttu-id="4c0d8-403">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="4c0d8-403">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-404">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-404">Network</span></span>

* <span data-ttu-id="4c0d8-405">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-405">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="4c0d8-406">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="4c0d8-406">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="4c0d8-407">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-407">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="4c0d8-408">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-408">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="4c0d8-409">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-409">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="4c0d8-410">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-410">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="4c0d8-411">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-411">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="4c0d8-412">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="4c0d8-412">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="4c0d8-413">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-413">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="4c0d8-414">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-414">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-415">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-415">Profile</span></span>

* <span data-ttu-id="4c0d8-416">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="4c0d8-416">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-417">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-417">Resource</span></span>

* <span data-ttu-id="4c0d8-418">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-418">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-419">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-419">Storage</span></span>

* <span data-ttu-id="4c0d8-420">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="4c0d8-420">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="4c0d8-421">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="4c0d8-421">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="4c0d8-422">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-422">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="4c0d8-423">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-423">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="4c0d8-424">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="4c0d8-424">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-425">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-425">VM</span></span>

* <span data-ttu-id="4c0d8-426">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="4c0d8-426">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="4c0d8-427">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-427">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="4c0d8-428">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="4c0d8-428">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="4c0d8-429">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-429">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="4c0d8-430">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="4c0d8-430">January 17, 2018</span></span>

<span data-ttu-id="4c0d8-431">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="4c0d8-431">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="4c0d8-432">ACR</span><span class="sxs-lookup"><span data-stu-id="4c0d8-432">ACR</span></span>

* <span data-ttu-id="4c0d8-433">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="4c0d8-433">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="4c0d8-434">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="4c0d8-434">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-435">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-435">ACS</span></span>

* <span data-ttu-id="4c0d8-436">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-436">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="4c0d8-437">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-437">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-438">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-438">Appservice</span></span>

* <span data-ttu-id="4c0d8-439">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-439">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="4c0d8-440">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-440">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="4c0d8-441">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-441">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="4c0d8-442">Backup</span><span class="sxs-lookup"><span data-stu-id="4c0d8-442">Backup</span></span>

* <span data-ttu-id="4c0d8-443">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="4c0d8-443">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="4c0d8-444">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-444">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="4c0d8-445">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-445">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="4c0d8-446">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="4c0d8-446">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="4c0d8-447">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="4c0d8-447">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="4c0d8-448">Batch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-448">Batch</span></span>

* <span data-ttu-id="4c0d8-449">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="4c0d8-449">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="4c0d8-450">Nube</span><span class="sxs-lookup"><span data-stu-id="4c0d8-450">Cloud</span></span>

* <span data-ttu-id="4c0d8-451">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="4c0d8-451">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="4c0d8-452">Consumo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-452">Consumption</span></span>

* <span data-ttu-id="4c0d8-453">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-453">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="4c0d8-454">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4c0d8-454">Event Grid</span></span>

* <span data-ttu-id="4c0d8-455">[[CAMBIO IMPORTANTE]] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-455">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4c0d8-456">[[CAMBIO IMPORTANTE]] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-456">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4c0d8-457">[[CAMBIO IMPORTANTE]] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-457">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="4c0d8-458">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-458">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="4c0d8-459">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-459">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="4c0d8-460">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-460">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="4c0d8-461">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-461">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="4c0d8-462">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="4c0d8-462">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="4c0d8-463">Interactive</span><span class="sxs-lookup"><span data-stu-id="4c0d8-463">Interactive</span></span>

* <span data-ttu-id="4c0d8-464">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="4c0d8-464">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="4c0d8-465">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-465">Fixed errors on startup</span></span>
* <span data-ttu-id="4c0d8-466">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-466">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="4c0d8-467">IoT</span><span class="sxs-lookup"><span data-stu-id="4c0d8-467">IoT</span></span>

* <span data-ttu-id="4c0d8-468">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-468">Added support for device provisioning service</span></span>
* <span data-ttu-id="4c0d8-469">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-469">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="4c0d8-470">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="4c0d8-470">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-471">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-471">Monitor</span></span>

* <span data-ttu-id="4c0d8-472">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-472">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="4c0d8-473">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-473">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="4c0d8-474">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-474">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-475">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-475">Network</span></span>

* <span data-ttu-id="4c0d8-476">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-476">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="4c0d8-477">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-477">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-478">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-478">Profile</span></span>

* <span data-ttu-id="4c0d8-479">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="4c0d8-479">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="4c0d8-480">Rol</span><span class="sxs-lookup"><span data-stu-id="4c0d8-480">Role</span></span>

* <span data-ttu-id="4c0d8-481">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="4c0d8-481">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4c0d8-482">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4c0d8-482">Service Fabric</span></span>

* <span data-ttu-id="4c0d8-483">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="4c0d8-483">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="4c0d8-484">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-484">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-485">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-485">VM</span></span>

* <span data-ttu-id="4c0d8-486">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-486">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="4c0d8-487">[[CAMBIO IMPORTANTE]] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-487">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="4c0d8-488">[[CAMBIO IMPORTANTE]] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-488">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="4c0d8-489">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-489">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="4c0d8-490">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="4c0d8-490">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="4c0d8-491">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-491">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4c0d8-492">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-492">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="4c0d8-493">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-493">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="4c0d8-494">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-494">December 19, 2017</span></span>

<span data-ttu-id="4c0d8-495">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="4c0d8-495">Version 2.0.23</span></span>

* <span data-ttu-id="4c0d8-496">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="4c0d8-496">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-497">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-497">Container</span></span>

* <span data-ttu-id="4c0d8-498">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-498">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-499">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-499">Network</span></span>

* <span data-ttu-id="4c0d8-500">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-500">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="4c0d8-501">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-501">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-502">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-502">Storage</span></span>

* <span data-ttu-id="4c0d8-503">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="4c0d8-503">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-504">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-504">VM</span></span>

* <span data-ttu-id="4c0d8-505">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="4c0d8-505">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="4c0d8-506">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-506">December 5, 2017</span></span>

<span data-ttu-id="4c0d8-507">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="4c0d8-507">Version 2.0.22</span></span>

* <span data-ttu-id="4c0d8-508">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-508">Removed `az component` commands.</span></span> <span data-ttu-id="4c0d8-509">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-509">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-510">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-510">Core</span></span>
* <span data-ttu-id="4c0d8-511">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="4c0d8-511">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="4c0d8-512">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="4c0d8-512">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-513">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-513">ACS</span></span>

* <span data-ttu-id="4c0d8-514">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-514">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="4c0d8-515">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-515">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="4c0d8-516">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="4c0d8-516">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="4c0d8-517">Advisor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-517">Advisor</span></span>

* <span data-ttu-id="4c0d8-518">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-518">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-519">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-519">Appservice</span></span>

* <span data-ttu-id="4c0d8-520">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-520">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="4c0d8-521">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-521">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="4c0d8-522">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-522">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="4c0d8-523">Consumo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-523">Consumption</span></span>

* <span data-ttu-id="4c0d8-524">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="4c0d8-524">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-525">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-525">Container</span></span>

* <span data-ttu-id="4c0d8-526">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="4c0d8-526">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-527">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-527">Monitor</span></span>

* <span data-ttu-id="4c0d8-528">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="4c0d8-528">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-529">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-529">Resource</span></span>

* <span data-ttu-id="4c0d8-530">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-530">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="4c0d8-531">Rol</span><span class="sxs-lookup"><span data-stu-id="4c0d8-531">Role</span></span>

* <span data-ttu-id="4c0d8-532">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-532">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="4c0d8-533">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="4c0d8-533">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="4c0d8-534">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-534">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-535">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-535">SQL</span></span>

* <span data-ttu-id="4c0d8-536">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-536">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="4c0d8-537">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-537">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-538">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-538">VM</span></span>

* <span data-ttu-id="4c0d8-539">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-539">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="4c0d8-540">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-540">November 14, 2017</span></span>

<span data-ttu-id="4c0d8-541">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4c0d8-541">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4c0d8-542">ACR</span><span class="sxs-lookup"><span data-stu-id="4c0d8-542">ACR</span></span>

* <span data-ttu-id="4c0d8-543">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="4c0d8-543">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4c0d8-544">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-544">ACS</span></span>

* <span data-ttu-id="4c0d8-545">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-545">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4c0d8-546">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-546">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4c0d8-547">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-547">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4c0d8-548">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="4c0d8-548">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4c0d8-549">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="4c0d8-549">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-550">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-550">Appservice</span></span>

* <span data-ttu-id="4c0d8-551">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="4c0d8-551">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4c0d8-552">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-552">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4c0d8-553">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-553">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4c0d8-554">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-554">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4c0d8-555">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="4c0d8-555">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4c0d8-556">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="4c0d8-556">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4c0d8-557">Batch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-557">Batch</span></span>

* <span data-ttu-id="4c0d8-558">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-558">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4c0d8-559">Batchai</span><span class="sxs-lookup"><span data-stu-id="4c0d8-559">Batchai</span></span>

* <span data-ttu-id="4c0d8-560">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-560">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4c0d8-561">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-561">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4c0d8-562">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-562">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4c0d8-563">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-563">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4c0d8-564">Nube</span><span class="sxs-lookup"><span data-stu-id="4c0d8-564">Cloud</span></span>

* <span data-ttu-id="4c0d8-565">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="4c0d8-565">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-566">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-566">Container</span></span>

* <span data-ttu-id="4c0d8-567">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-567">Added support to open multiple ports</span></span>
* <span data-ttu-id="4c0d8-568">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="4c0d8-568">Added container group restart policy</span></span>
* <span data-ttu-id="4c0d8-569">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="4c0d8-569">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4c0d8-570">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="4c0d8-570">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4c0d8-571">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4c0d8-571">Data Lake Analytics</span></span>

* <span data-ttu-id="4c0d8-572">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="4c0d8-572">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4c0d8-573">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="4c0d8-573">Data Lake Store</span></span>

* <span data-ttu-id="4c0d8-574">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="4c0d8-574">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4c0d8-575">Extensión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-575">Extension</span></span>

* <span data-ttu-id="4c0d8-576">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="4c0d8-576">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4c0d8-577">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="4c0d8-577">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4c0d8-578">IoT</span><span class="sxs-lookup"><span data-stu-id="4c0d8-578">IoT</span></span>

* <span data-ttu-id="4c0d8-579">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="4c0d8-579">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-580">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-580">Monitor</span></span>

* <span data-ttu-id="4c0d8-581">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-581">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-582">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-582">Network</span></span>

* <span data-ttu-id="4c0d8-583">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="4c0d8-583">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4c0d8-584">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-584">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4c0d8-585">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-585">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4c0d8-586">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-586">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4c0d8-587">Reservations</span><span class="sxs-lookup"><span data-stu-id="4c0d8-587">Reservations</span></span>

* <span data-ttu-id="4c0d8-588">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="4c0d8-588">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-589">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-589">Resource</span></span>

* <span data-ttu-id="4c0d8-590">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-590">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-591">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-591">SQL</span></span>

* <span data-ttu-id="4c0d8-592">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-592">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-593">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-593">Storage</span></span>

* <span data-ttu-id="4c0d8-594">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="4c0d8-594">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4c0d8-595">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="4c0d8-595">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4c0d8-596">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-596">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4c0d8-597">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-597">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4c0d8-598">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-598">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4c0d8-599">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-599">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4c0d8-600">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-600">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-601">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-601">VM</span></span>

* <span data-ttu-id="4c0d8-602">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-602">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4c0d8-603">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="4c0d8-603">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4c0d8-604">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="4c0d8-604">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4c0d8-605">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-605">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4c0d8-606">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-606">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4c0d8-607">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-607">October 24, 2017</span></span>

<span data-ttu-id="4c0d8-608">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4c0d8-608">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-609">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-609">Core</span></span>

* <span data-ttu-id="4c0d8-610">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-610">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4c0d8-611">ACR</span><span class="sxs-lookup"><span data-stu-id="4c0d8-611">ACR</span></span>

* <span data-ttu-id="4c0d8-612">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="4c0d8-612">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4c0d8-613">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="4c0d8-613">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4c0d8-614">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="4c0d8-614">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-615">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-615">ACS</span></span>

* <span data-ttu-id="4c0d8-616">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-616">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4c0d8-617">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-617">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-618">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-618">Appservice</span></span>

* <span data-ttu-id="4c0d8-619">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-619">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4c0d8-620">Componente</span><span class="sxs-lookup"><span data-stu-id="4c0d8-620">Component</span></span>

* <span data-ttu-id="4c0d8-621">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="4c0d8-621">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-622">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-622">Monitor</span></span>

* <span data-ttu-id="4c0d8-623">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-623">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-624">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-624">Resource</span></span>

* <span data-ttu-id="4c0d8-625">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-625">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4c0d8-626">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-626">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-627">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-627">VM</span></span>

* <span data-ttu-id="4c0d8-628">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-628">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4c0d8-629">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-629">October 9, 2017</span></span>

<span data-ttu-id="4c0d8-630">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4c0d8-630">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-631">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-631">Core</span></span>

* <span data-ttu-id="4c0d8-632">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4c0d8-632">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-633">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-633">Appservice</span></span>

* <span data-ttu-id="4c0d8-634">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-634">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4c0d8-635">Batch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-635">Batch</span></span>

* <span data-ttu-id="4c0d8-636">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4c0d8-636">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4c0d8-637">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="4c0d8-637">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4c0d8-638">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-638">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4c0d8-639">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="4c0d8-639">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4c0d8-640">Batchai</span><span class="sxs-lookup"><span data-stu-id="4c0d8-640">Batchai</span></span>

* <span data-ttu-id="4c0d8-641">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-641">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4c0d8-642">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4c0d8-642">Keyvault</span></span>

* <span data-ttu-id="4c0d8-643">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-643">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4c0d8-644">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-644">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4c0d8-645">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-645">Network</span></span>

* <span data-ttu-id="4c0d8-646">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-646">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4c0d8-647">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-647">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-648">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-648">Resource</span></span>

* <span data-ttu-id="4c0d8-649">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-649">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4c0d8-650">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="4c0d8-650">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4c0d8-651">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-651">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4c0d8-652">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-652">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-653">Sql</span><span class="sxs-lookup"><span data-stu-id="4c0d8-653">Sql</span></span>

* <span data-ttu-id="4c0d8-654">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="4c0d8-654">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4c0d8-655">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-655">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4c0d8-656">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-656">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-657">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-657">Storage</span></span>

* <span data-ttu-id="4c0d8-658">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-658">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-659">Vm</span><span class="sxs-lookup"><span data-stu-id="4c0d8-659">Vm</span></span>

* <span data-ttu-id="4c0d8-660">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="4c0d8-660">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4c0d8-661">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-661">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4c0d8-662">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-662">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4c0d8-663">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-663">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4c0d8-664">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-664">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4c0d8-665">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-665">September 22, 2017</span></span>

<span data-ttu-id="4c0d8-666">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4c0d8-666">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-667">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-667">Resource</span></span>

* <span data-ttu-id="4c0d8-668">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-668">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4c0d8-669">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="4c0d8-669">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4c0d8-670">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-670">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4c0d8-671">[[CAMBIO IMPORTANTE]] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-671">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-672">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-672">Network</span></span>

* <span data-ttu-id="4c0d8-673">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-673">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4c0d8-674">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-674">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4c0d8-675">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-675">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4c0d8-676">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-676">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4c0d8-677">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-677">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4c0d8-678">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-678">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4c0d8-679">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-679">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-680">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-680">Storage</span></span>

* <span data-ttu-id="4c0d8-681">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="4c0d8-681">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4c0d8-682">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="4c0d8-682">Eventgrid</span></span>

* <span data-ttu-id="4c0d8-683">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-683">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-684">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-684">SQL</span></span>

* <span data-ttu-id="4c0d8-685">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-685">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4c0d8-686">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="4c0d8-686">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4c0d8-687">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-687">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4c0d8-688">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4c0d8-688">Keyvault</span></span>

* <span data-ttu-id="4c0d8-689">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="4c0d8-689">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-690">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-690">VM</span></span>

* <span data-ttu-id="4c0d8-691">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-691">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4c0d8-692">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="4c0d8-692">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4c0d8-693">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-693">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4c0d8-694">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-694">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4c0d8-695">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-695">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4c0d8-696">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-696">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-697">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-697">ACS</span></span>

* <span data-ttu-id="4c0d8-698">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-698">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-699">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-699">Appservice</span></span>

* <span data-ttu-id="4c0d8-700">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-700">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4c0d8-701">Backup</span><span class="sxs-lookup"><span data-stu-id="4c0d8-701">Backup</span></span>

* <span data-ttu-id="4c0d8-702">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-702">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4c0d8-703">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-703">September 11, 2017</span></span>

<span data-ttu-id="4c0d8-704">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4c0d8-704">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4c0d8-705">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-705">Core</span></span>

* <span data-ttu-id="4c0d8-706">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-706">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4c0d8-707">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-707">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-708">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-708">Acs</span></span>

* <span data-ttu-id="4c0d8-709">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-709">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4c0d8-710">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-710">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-711">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-711">Appservice</span></span>

* <span data-ttu-id="4c0d8-712">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-712">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4c0d8-713">CDN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-713">CDN</span></span>

* <span data-ttu-id="4c0d8-714">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-714">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="4c0d8-715">Extensión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-715">Extension</span></span>

* <span data-ttu-id="4c0d8-716">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="4c0d8-716">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="4c0d8-717">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4c0d8-717">Keyvault</span></span>

* <span data-ttu-id="4c0d8-718">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-718">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-719">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-719">Network</span></span>

* <span data-ttu-id="4c0d8-720">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-720">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4c0d8-721">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-721">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4c0d8-722">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-722">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4c0d8-723">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-723">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4c0d8-724">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-724">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-725">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-725">Resource</span></span>

* <span data-ttu-id="4c0d8-726">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-726">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4c0d8-727">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-727">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4c0d8-728">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-728">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4c0d8-729">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="4c0d8-729">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-730">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-730">SQL</span></span>

* <span data-ttu-id="4c0d8-731">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-731">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-732">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-732">VM</span></span>

* <span data-ttu-id="4c0d8-733">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-733">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4c0d8-734">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-734">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4c0d8-735">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-735">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4c0d8-736">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-736">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4c0d8-737">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-737">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4c0d8-738">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-738">August 31, 2017</span></span>

<span data-ttu-id="4c0d8-739">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4c0d8-739">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4c0d8-740">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4c0d8-740">Keyvault</span></span>

* <span data-ttu-id="4c0d8-741">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-741">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4c0d8-742">Sf</span><span class="sxs-lookup"><span data-stu-id="4c0d8-742">Sf</span></span>

* <span data-ttu-id="4c0d8-743">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-743">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-744">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-744">Storage</span></span>

* <span data-ttu-id="4c0d8-745">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-745">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4c0d8-746">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-746">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4c0d8-747">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-747">August 28, 2017</span></span>

<span data-ttu-id="4c0d8-748">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4c0d8-748">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4c0d8-749">CLI</span><span class="sxs-lookup"><span data-stu-id="4c0d8-749">CLI</span></span>

* <span data-ttu-id="4c0d8-750">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-750">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-751">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-751">ACS</span></span>

* <span data-ttu-id="4c0d8-752">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-752">Corrected preview regions</span></span>
* <span data-ttu-id="4c0d8-753">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-753">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="4c0d8-754">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="4c0d8-754">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-755">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-755">Appservice</span></span>

* <span data-ttu-id="4c0d8-756">[[CAMBIO IMPORTANTE]] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-756">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4c0d8-757">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-757">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4c0d8-758">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-758">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4c0d8-759">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-759">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4c0d8-760">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-760">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4c0d8-761">IoT</span><span class="sxs-lookup"><span data-stu-id="4c0d8-761">IoT</span></span>

* <span data-ttu-id="4c0d8-762">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-762">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-763">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-763">Network</span></span>

* <span data-ttu-id="4c0d8-764">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-764">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4c0d8-765">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-765">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4c0d8-766">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-766">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4c0d8-767">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-767">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4c0d8-768">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-768">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-769">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-769">Profile</span></span>

* <span data-ttu-id="4c0d8-770">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-770">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4c0d8-771">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4c0d8-771">Service Fabric</span></span>

* <span data-ttu-id="4c0d8-772">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-772">Preview release</span></span>
* <span data-ttu-id="4c0d8-773">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-773">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4c0d8-774">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-774">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4c0d8-775">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-775">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-776">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-776">Storage</span></span>

* <span data-ttu-id="4c0d8-777">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-777">Enabled setting blob tier</span></span>
* <span data-ttu-id="4c0d8-778">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-778">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4c0d8-779">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-779">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="4c0d8-780">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-780">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4c0d8-781">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-781">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4c0d8-782">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="4c0d8-782">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-783">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-783">VM</span></span>

* <span data-ttu-id="4c0d8-784">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-784">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4c0d8-785">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-785">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="4c0d8-786">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-786">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="4c0d8-787">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-787">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4c0d8-788">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-788">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4c0d8-789">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-789">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4c0d8-790">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-790">August 15, 2017</span></span>

<span data-ttu-id="4c0d8-791">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4c0d8-791">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-792">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-792">ACS</span></span>

* <span data-ttu-id="4c0d8-793">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-793">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-794">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-794">Appservice</span></span>

* <span data-ttu-id="4c0d8-795">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-795">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4c0d8-796">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4c0d8-796">Event Grid</span></span>

* <span data-ttu-id="4c0d8-797">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-797">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4c0d8-798">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-798">August 11, 2017</span></span>

<span data-ttu-id="4c0d8-799">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4c0d8-799">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-800">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-800">ACS</span></span>

* <span data-ttu-id="4c0d8-801">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-801">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4c0d8-802">Batch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-802">Batch</span></span>

* <span data-ttu-id="4c0d8-803">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-803">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4c0d8-804">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-804">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4c0d8-805">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-805">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4c0d8-806">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-806">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4c0d8-807">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-807">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4c0d8-808">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-808">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4c0d8-809">Componente</span><span class="sxs-lookup"><span data-stu-id="4c0d8-809">Component</span></span>

* <span data-ttu-id="4c0d8-810">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-810">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4c0d8-811">Contenedor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-811">Container</span></span>

* <span data-ttu-id="4c0d8-812">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-812">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4c0d8-813">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="4c0d8-813">Data Lake Store</span></span>

* <span data-ttu-id="4c0d8-814">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-814">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4c0d8-815">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4c0d8-815">Event Grid</span></span>

* <span data-ttu-id="4c0d8-816">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-816">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-817">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-817">Network</span></span>

* <span data-ttu-id="4c0d8-818">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-818">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4c0d8-819">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-819">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4c0d8-820">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-820">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4c0d8-821">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-821">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-822">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-822">Profile</span></span>

* <span data-ttu-id="4c0d8-823">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-823">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-824">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-824">Storage</span></span>

* <span data-ttu-id="4c0d8-825">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-825">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-826">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-826">VM</span></span>

* <span data-ttu-id="4c0d8-827">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-827">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4c0d8-828">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-828">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4c0d8-829">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-829">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4c0d8-830">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-830">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4c0d8-831">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-831">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4c0d8-832">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-832">July 28, 2017</span></span>

<span data-ttu-id="4c0d8-833">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4c0d8-833">Version 2.0.12</span></span>

* <span data-ttu-id="4c0d8-834">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-834">Added container commands</span></span>
* <span data-ttu-id="4c0d8-835">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-835">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4c0d8-836">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-836">Core</span></span>

* <span data-ttu-id="4c0d8-837">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-837">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4c0d8-838">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-838">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4c0d8-839">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-839">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4c0d8-840">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-840">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4c0d8-841">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-841">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4c0d8-842">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-842">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4c0d8-843">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-843">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4c0d8-844">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-844">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4c0d8-845">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-845">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4c0d8-846">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-846">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4c0d8-847">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-847">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4c0d8-848">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-848">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4c0d8-849">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-849">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4c0d8-850">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-850">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4c0d8-851">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-851">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4c0d8-852">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-852">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4c0d8-853">ACR</span><span class="sxs-lookup"><span data-stu-id="4c0d8-853">ACR</span></span>

* <span data-ttu-id="4c0d8-854">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-854">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4c0d8-855">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-855">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4c0d8-856">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-856">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4c0d8-857">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-857">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4c0d8-858">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-858">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4c0d8-859">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-859">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-860">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-860">ACS</span></span>

* <span data-ttu-id="4c0d8-861">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-861">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-862">Appservice</span><span class="sxs-lookup"><span data-stu-id="4c0d8-862">Appservice</span></span>

* <span data-ttu-id="4c0d8-863">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-863">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4c0d8-864">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-864">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4c0d8-865">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-865">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4c0d8-866">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-866">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4c0d8-867">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-867">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4c0d8-868">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-868">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4c0d8-869">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-869">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4c0d8-870">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-870">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4c0d8-871">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-871">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4c0d8-872">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-872">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4c0d8-873">Batch</span><span class="sxs-lookup"><span data-stu-id="4c0d8-873">Batch</span></span>

* <span data-ttu-id="4c0d8-874">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-874">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4c0d8-875">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-875">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4c0d8-876">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-876">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4c0d8-877">CDN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-877">CDN</span></span>

* <span data-ttu-id="4c0d8-878">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="4c0d8-878">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="4c0d8-879">Nube</span><span class="sxs-lookup"><span data-stu-id="4c0d8-879">Cloud</span></span>

* <span data-ttu-id="4c0d8-880">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-880">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4c0d8-881">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-881">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4c0d8-882">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-882">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4c0d8-883">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-883">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4c0d8-884">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-884">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4c0d8-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-885">CosmosDB</span></span>

* <span data-ttu-id="4c0d8-886">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-886">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4c0d8-887">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="4c0d8-887">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4c0d8-888">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4c0d8-888">Data Lake Analytics</span></span>

* <span data-ttu-id="4c0d8-889">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-889">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4c0d8-890">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-890">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4c0d8-891">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-891">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4c0d8-892">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="4c0d8-892">Data Lake Store</span></span>

* <span data-ttu-id="4c0d8-893">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-893">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4c0d8-894">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-894">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4c0d8-895">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-895">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4c0d8-896">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-896">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4c0d8-897">Interactive</span><span class="sxs-lookup"><span data-stu-id="4c0d8-897">Interactive</span></span>

* <span data-ttu-id="4c0d8-898">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-898">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4c0d8-899">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-899">Increased test coverage</span></span>
* <span data-ttu-id="4c0d8-900">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-900">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4c0d8-901">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-901">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4c0d8-902">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-902">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4c0d8-903">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-903">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4c0d8-904">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-904">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4c0d8-905">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-905">Added `--progress` flag</span></span>
* <span data-ttu-id="4c0d8-906">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-906">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4c0d8-907">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-907">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4c0d8-908">IoT</span><span class="sxs-lookup"><span data-stu-id="4c0d8-908">IoT</span></span>

* <span data-ttu-id="4c0d8-909">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-909">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4c0d8-910">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-910">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4c0d8-911">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="4c0d8-911">Key vault</span></span>

* <span data-ttu-id="4c0d8-912">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-912">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4c0d8-913">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-913">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4c0d8-914">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-914">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4c0d8-915">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-915">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4c0d8-916">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-916">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4c0d8-917">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-917">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4c0d8-918">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="4c0d8-918">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4c0d8-919">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-919">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4c0d8-920">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-920">Lab</span></span>

* <span data-ttu-id="4c0d8-921">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-921">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4c0d8-922">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-922">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-923">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-923">Monitor</span></span>

* <span data-ttu-id="4c0d8-924">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-924">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4c0d8-925">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-925">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4c0d8-926">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-926">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4c0d8-927">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-927">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4c0d8-928">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-928">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4c0d8-929">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-929">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4c0d8-930">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-930">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4c0d8-931">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-931">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4c0d8-932">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-932">`location` no longer required</span></span>
  * <span data-ttu-id="4c0d8-933">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-933">Add name and ID support for target</span></span>
  * <span data-ttu-id="4c0d8-934">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-934">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4c0d8-935">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-935">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4c0d8-936">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-936">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4c0d8-937">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-937">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4c0d8-938">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-938">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4c0d8-939">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-939">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-940">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-940">Network</span></span>

* <span data-ttu-id="4c0d8-941">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-941">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4c0d8-942">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-942">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4c0d8-943">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-943">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4c0d8-944">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-944">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4c0d8-945">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-945">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4c0d8-946">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-946">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4c0d8-947">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-947">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4c0d8-948">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-948">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4c0d8-949">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-949">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4c0d8-950">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-950">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4c0d8-951">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-951">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4c0d8-952">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-952">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4c0d8-953">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-953">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4c0d8-954">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-954">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4c0d8-955">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-955">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4c0d8-956">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-956">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4c0d8-957">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-957">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4c0d8-958">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-958">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4c0d8-959">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-959">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4c0d8-960">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-960">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4c0d8-961">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-961">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4c0d8-962">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-962">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4c0d8-963">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-963">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4c0d8-964">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-964">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4c0d8-965">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-965">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4c0d8-966">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-966">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4c0d8-967">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-967">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-968">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-968">Profile</span></span>

* <span data-ttu-id="4c0d8-969">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-969">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4c0d8-970">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-970">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4c0d8-971">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="4c0d8-971">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4c0d8-972">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-972">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4c0d8-973">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-973">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4c0d8-974">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-974">RDBMS</span></span>

* <span data-ttu-id="4c0d8-975">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-975">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4c0d8-976">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-976">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4c0d8-977">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-977">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4c0d8-978">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-978">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-979">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-979">Resource</span></span>

* <span data-ttu-id="4c0d8-980">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-980">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4c0d8-981">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-981">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4c0d8-982">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-982">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4c0d8-983">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-983">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4c0d8-984">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-984">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4c0d8-985">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-985">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4c0d8-986">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-986">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4c0d8-987">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-987">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4c0d8-988">Rol</span><span class="sxs-lookup"><span data-stu-id="4c0d8-988">Role</span></span>

* <span data-ttu-id="4c0d8-989">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-989">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4c0d8-990">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-990">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4c0d8-991">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-991">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4c0d8-992">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-992">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4c0d8-993">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-993">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4c0d8-994">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4c0d8-994">Service Fabric</span></span>
* <span data-ttu-id="4c0d8-995">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-995">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4c0d8-996">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-996">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4c0d8-997">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-997">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-998">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-998">SQL</span></span>

* <span data-ttu-id="4c0d8-999">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-999">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4c0d8-1000">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1000">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4c0d8-1001">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1001">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-1002">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1002">Storage</span></span>

* <span data-ttu-id="4c0d8-1003">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1003">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4c0d8-1004">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1004">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4c0d8-1005">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1005">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4c0d8-1006">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1006">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="4c0d8-1007">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1007">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="4c0d8-1008">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1008">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-1009">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1009">VM</span></span>

* <span data-ttu-id="4c0d8-1010">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1010">Support configuring nsg</span></span>
* <span data-ttu-id="4c0d8-1011">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1011">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4c0d8-1012">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1012">Support managed service identities</span></span>
* <span data-ttu-id="4c0d8-1013">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1013">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="4c0d8-1014">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1014">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4c0d8-1015">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1015">May 10, 2017</span></span>

<span data-ttu-id="4c0d8-1016">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1016">Version 2.0.6</span></span>

* <span data-ttu-id="4c0d8-1017">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1017">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4c0d8-1018">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1018">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4c0d8-1019">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1019">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="4c0d8-1020">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1020">Include Cognitive Services module</span></span>
* <span data-ttu-id="4c0d8-1021">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1021">Include Service Fabric module</span></span>
* <span data-ttu-id="4c0d8-1022">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1022">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="4c0d8-1023">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1023">Add support for CDN commands</span></span>
* <span data-ttu-id="4c0d8-1024">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1024">Remove Container module</span></span>
* <span data-ttu-id="4c0d8-1025">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1025">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4c0d8-1026">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1026">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4c0d8-1027">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1027">Core</span></span>

* <span data-ttu-id="4c0d8-1028">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1028">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="4c0d8-1029">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1029">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4c0d8-1030">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1030">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4c0d8-1031">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1031">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4c0d8-1032">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1032">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4c0d8-1033">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1033">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4c0d8-1034">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1034">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4c0d8-1035">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1035">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4c0d8-1036">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1036">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4c0d8-1037">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1037">core: Improved performance</span></span>
* <span data-ttu-id="4c0d8-1038">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1038">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4c0d8-1039">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1039">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-1040">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1040">ACS</span></span>

* <span data-ttu-id="4c0d8-1041">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1041">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4c0d8-1042">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1042">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4c0d8-1043">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1043">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4c0d8-1044">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1044">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-1045">AppService</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1045">AppService</span></span>

* <span data-ttu-id="4c0d8-1046">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1046">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4c0d8-1047">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1047">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4c0d8-1048">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1048">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4c0d8-1049">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1049">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4c0d8-1050">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1050">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4c0d8-1051">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1051">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4c0d8-1052">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1052">support slot swap with preview</span></span>
* <span data-ttu-id="4c0d8-1053">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1053">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4c0d8-1054">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1054">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4c0d8-1055">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1055">CosmosDB</span></span>

* <span data-ttu-id="4c0d8-1056">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1056">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="4c0d8-1057">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1057">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4c0d8-1058">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1058">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4c0d8-1059">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1059">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4c0d8-1060">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1060">Data Lake Analytics</span></span>

* <span data-ttu-id="4c0d8-1061">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1061">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="4c0d8-1062">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1062">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4c0d8-1063">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1063">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4c0d8-1064">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1064">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4c0d8-1065">Tabla</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1065">Table</span></span>
  * <span data-ttu-id="4c0d8-1066">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1066">Table valued function</span></span>
  * <span data-ttu-id="4c0d8-1067">Ver</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1067">View</span></span>
  * <span data-ttu-id="4c0d8-1068">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1068">Table Statistics.</span></span> <span data-ttu-id="4c0d8-1069">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1069">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4c0d8-1070">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1070">Data Lake Store</span></span>

* <span data-ttu-id="4c0d8-1071">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1071">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="4c0d8-1072">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1072">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4c0d8-1073">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1073">missed help for access show.</span></span> <span data-ttu-id="4c0d8-1074">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1074">adding it.</span></span> <span data-ttu-id="4c0d8-1075">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1075">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4c0d8-1076">Buscar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1076">Find</span></span>

* <span data-ttu-id="4c0d8-1077">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1077">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4c0d8-1078">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1078">KeyVault</span></span>

* <span data-ttu-id="4c0d8-1079">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1079">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4c0d8-1080">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1080">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="4c0d8-1081">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1081">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4c0d8-1082">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1082">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="4c0d8-1083">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1083">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4c0d8-1084">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1084">Lab</span></span>

* <span data-ttu-id="4c0d8-1085">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1085">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="4c0d8-1086">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1086">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="4c0d8-1087">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1087">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="4c0d8-1088">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1088">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="4c0d8-1089">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1089">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="4c0d8-1090">Supervisión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1090">Monitor</span></span>

* <span data-ttu-id="4c0d8-1091">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1091">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4c0d8-1092">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1092">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4c0d8-1093">Red</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1093">Network</span></span>

* <span data-ttu-id="4c0d8-1094">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1094">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="4c0d8-1095">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1095">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="4c0d8-1096">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1096">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="4c0d8-1097">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1097">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="4c0d8-1098">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1098">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="4c0d8-1099">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1099">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="4c0d8-1100">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1100">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="4c0d8-1101">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1101">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="4c0d8-1102">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1102">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="4c0d8-1103">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1103">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4c0d8-1104">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1104">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="4c0d8-1105">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1105">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="4c0d8-1106">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1106">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="4c0d8-1107">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1107">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="4c0d8-1108">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1108">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="4c0d8-1109">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1109">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="4c0d8-1110">Perfil</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1110">Profile</span></span>

* <span data-ttu-id="4c0d8-1111">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1111">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4c0d8-1112">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1112">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4c0d8-1113">Redis</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1113">Redis</span></span>

* <span data-ttu-id="4c0d8-1114">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1114">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4c0d8-1115">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1115">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="4c0d8-1116">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1116">Resource</span></span>

* <span data-ttu-id="4c0d8-1117">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1117">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4c0d8-1118">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1118">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4c0d8-1119">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1119">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4c0d8-1120">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1120">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4c0d8-1121">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1121">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4c0d8-1122">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1122">Add docs for az lock update.</span></span> <span data-ttu-id="4c0d8-1123">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1123">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4c0d8-1124">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1124">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4c0d8-1125">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1125">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4c0d8-1126">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1126">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4c0d8-1127">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1127">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4c0d8-1128">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1128">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4c0d8-1129">Rol</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1129">Role</span></span>

* <span data-ttu-id="4c0d8-1130">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1130">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4c0d8-1131">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1131">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4c0d8-1132">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1132">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4c0d8-1133">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1133">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4c0d8-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1134">SQL</span></span>

* <span data-ttu-id="4c0d8-1135">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1135">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="4c0d8-1136">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1136">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4c0d8-1137">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1137">Storage</span></span>

* <span data-ttu-id="4c0d8-1138">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1138">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="4c0d8-1139">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1139">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4c0d8-1140">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1140">Add support for large block blob upload</span></span>
* <span data-ttu-id="4c0d8-1141">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1141">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-1142">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1142">VM</span></span>

* <span data-ttu-id="4c0d8-1143">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1143">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4c0d8-1144">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1144">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4c0d8-1145">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1145">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4c0d8-1146">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1146">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4c0d8-1147">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1147">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4c0d8-1148">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1148">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4c0d8-1149">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1149">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4c0d8-1150">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1150">April 3, 2017</span></span>

<span data-ttu-id="4c0d8-1151">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1151">Version 2.0.2</span></span>

<span data-ttu-id="4c0d8-1152">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1152">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="4c0d8-1153">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1153">Core</span></span>

* <span data-ttu-id="4c0d8-1154">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1154">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="4c0d8-1155">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1155">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4c0d8-1156">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1156">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4c0d8-1157">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1157">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4c0d8-1158">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1158">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4c0d8-1159">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1159">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4c0d8-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4c0d8-1161">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1161">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4c0d8-1162">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1162">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="4c0d8-1163">ACS</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1163">ACS</span></span>

* <span data-ttu-id="4c0d8-1164">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1164">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4c0d8-1165">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1165">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4c0d8-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4c0d8-1167">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1167">Add support for windows clusters.</span></span> <span data-ttu-id="4c0d8-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4c0d8-1169">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1169">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4c0d8-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="4c0d8-1171">AppService</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1171">AppService</span></span>

* <span data-ttu-id="4c0d8-1172">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1172">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4c0d8-1173">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1173">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4c0d8-1174">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1174">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4c0d8-1175">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1175">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="4c0d8-1176">DataLake</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1176">DataLake</span></span>

* <span data-ttu-id="4c0d8-1177">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1177">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="4c0d8-1178">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1178">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="4c0d8-1179">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1179">DocuemntDB</span></span>

* <span data-ttu-id="4c0d8-1180">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1180">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4c0d8-1181">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1181">VM</span></span>

* <span data-ttu-id="4c0d8-1182">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1182">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4c0d8-1183">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1183">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4c0d8-1184">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1184">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4c0d8-1185">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1185">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4c0d8-1186">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1186">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4c0d8-1187">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1187">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="4c0d8-1188">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1188">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4c0d8-1189">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1189">February 27, 2017</span></span>

<span data-ttu-id="4c0d8-1190">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1190">Version 2.0.0</span></span>

<span data-ttu-id="4c0d8-1191">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1191">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="4c0d8-1192">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1192">Container Service (acs)</span></span>
- <span data-ttu-id="4c0d8-1193">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1193">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4c0d8-1194">Redes</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1194">Networking</span></span>
- <span data-ttu-id="4c0d8-1195">Storage</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1195">Storage</span></span>

<span data-ttu-id="4c0d8-1196">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1196">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="4c0d8-1197">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1197">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="4c0d8-1198">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1198">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="4c0d8-1199">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1199">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="4c0d8-1200">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1200">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="4c0d8-1201">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1201">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4c0d8-1202">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1202">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4c0d8-1203">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1203">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="4c0d8-1204">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="4c0d8-1204">Provide feedback from the command line with the `az feedback` command</span></span>

