---
title: Notas de la versión de la CLI de Azure 2.0
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 254c7b306440d921cef6b611268839150fdf3196
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="98354-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="98354-103">Azure CLI 2.0 release notes</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="98354-104">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-104">May 7, 2018</span></span>

<span data-ttu-id="98354-105">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="98354-105">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="98354-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-106">Core</span></span>

* <span data-ttu-id="98354-107">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="98354-107">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="98354-108">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="98354-108">Added limited support for positional arguments</span></span>
* <span data-ttu-id="98354-109">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="98354-109">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="98354-110">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="98354-110">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="98354-111">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="98354-111">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="98354-112">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="98354-112">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="98354-113">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="98354-113">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="98354-114">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="98354-114">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="98354-115">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="98354-115">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="98354-116">ACR</span><span class="sxs-lookup"><span data-stu-id="98354-116">ACR</span></span>

* <span data-ttu-id="98354-117">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="98354-117">Added ACR Build commands</span></span>
* <span data-ttu-id="98354-118">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="98354-118">Improved resource not found error messages</span></span>
* <span data-ttu-id="98354-119">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="98354-119">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="98354-120">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="98354-120">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="98354-121">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="98354-121">Improved repository commands error messages</span></span>
* <span data-ttu-id="98354-122">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="98354-122">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="98354-123">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-123">ACS</span></span>

* <span data-ttu-id="98354-124">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="98354-124">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="98354-125">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="98354-125">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="98354-126">AMS</span><span class="sxs-lookup"><span data-stu-id="98354-126">AMS</span></span>

* <span data-ttu-id="98354-127">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="98354-127">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-128">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-128">Appservice</span></span>

* <span data-ttu-id="98354-129">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="98354-129">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="98354-130">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="98354-130">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="98354-131">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="98354-131">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="98354-132">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="98354-132">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="98354-133">Batch AI</span><span class="sxs-lookup"><span data-stu-id="98354-133">Batch AI</span></span>

* <span data-ttu-id="98354-134">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="98354-134">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="98354-135">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="98354-135">Cognitive Services</span></span>

* <span data-ttu-id="98354-136">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="98354-136">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="98354-137">Consumo</span><span class="sxs-lookup"><span data-stu-id="98354-137">Consumption</span></span>

* <span data-ttu-id="98354-138">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="98354-138">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="98354-139">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-139">Container</span></span>

* <span data-ttu-id="98354-140">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="98354-140">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="98354-141">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="98354-141">Cosmos DB</span></span>

* <span data-ttu-id="98354-142">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="98354-142">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="98354-143">DMS</span><span class="sxs-lookup"><span data-stu-id="98354-143">DMS</span></span>

* <span data-ttu-id="98354-144">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="98354-144">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="98354-145">Extensión</span><span class="sxs-lookup"><span data-stu-id="98354-145">Extension</span></span>

* <span data-ttu-id="98354-146">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="98354-146">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-147">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-147">Interactive</span></span>

* <span data-ttu-id="98354-148">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="98354-148">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="98354-149">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="98354-149">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="98354-150">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="98354-150">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="98354-151">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="98354-151">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="98354-152">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-152">Lab</span></span>

* <span data-ttu-id="98354-153">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="98354-153">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="98354-154">Red</span><span class="sxs-lookup"><span data-stu-id="98354-154">Network</span></span>

* <span data-ttu-id="98354-155">[[CAMBIO IMPORTANTE]] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="98354-155">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="98354-156">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-156">Profile</span></span>

* <span data-ttu-id="98354-157">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="98354-157">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="98354-158">[[CAMBIO IMPORTANTE]] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="98354-158">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="98354-159">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="98354-159">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="98354-160">Redis</span><span class="sxs-lookup"><span data-stu-id="98354-160">Redis</span></span>

* <span data-ttu-id="98354-161">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="98354-161">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="98354-162">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="98354-162">Deprecated `redis list-all`.</span></span> <span data-ttu-id="98354-163">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="98354-163">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="98354-164">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="98354-164">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="98354-165">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="98354-165">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="98354-166">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-166">Role</span></span>

* <span data-ttu-id="98354-167">[[CAMBIO IMPORTANTE]] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="98354-167">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="98354-168">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-168">Storage</span></span>

* <span data-ttu-id="98354-169">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="98354-169">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="98354-170">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="98354-170">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="98354-171">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="98354-171">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="98354-172">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="98354-172">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="98354-173">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="98354-173">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="98354-174">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-174">VM</span></span>

* <span data-ttu-id="98354-175">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="98354-175">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="98354-176">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="98354-176">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="98354-177">[[CAMBIO IMPORTANTE]] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="98354-177">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="98354-178">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="98354-178">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="98354-179">[[CAMBIO IMPORTANTE]] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="98354-179">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="98354-180">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="98354-180">Added write accelerator support</span></span> 
* <span data-ttu-id="98354-181">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="98354-181">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="98354-182">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="98354-182">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="98354-183">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="98354-183">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="98354-184">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-184">April 10, 2018</span></span>

<span data-ttu-id="98354-185">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="98354-185">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="98354-186">ACR</span><span class="sxs-lookup"><span data-stu-id="98354-186">ACR</span></span>

* <span data-ttu-id="98354-187">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="98354-187">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="98354-188">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-188">ACS</span></span>

* <span data-ttu-id="98354-189">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="98354-189">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-190">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-190">Appservice</span></span>

* <span data-ttu-id="98354-191">[[CAMBIO IMPORTANTE]]: Removed `assign-identity`</span><span class="sxs-lookup"><span data-stu-id="98354-191">[BREAKING CHANGE]: Removed `assign-identity`</span></span>
* <span data-ttu-id="98354-192">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="98354-192">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="98354-193">BatchAI</span><span class="sxs-lookup"><span data-stu-id="98354-193">BatchAI</span></span>

* <span data-ttu-id="98354-194">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="98354-194">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="98354-195">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="98354-195">Job level mounting</span></span>
 - <span data-ttu-id="98354-196">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="98354-196">Environment variables with secret values</span></span>
 - <span data-ttu-id="98354-197">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="98354-197">Performance counters settings</span></span>
 - <span data-ttu-id="98354-198">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="98354-198">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="98354-199">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="98354-199">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="98354-200">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="98354-200">Usage and limits reporting</span></span>
 - <span data-ttu-id="98354-201">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="98354-201">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="98354-202">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="98354-202">Support for custom images</span></span>
 - <span data-ttu-id="98354-203">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="98354-203">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="98354-204">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="98354-204">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="98354-205">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="98354-205">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="98354-206">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="98354-206">National clouds are supported</span></span>
* <span data-ttu-id="98354-207">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="98354-207">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="98354-208">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="98354-208">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="98354-209">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="98354-209">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="98354-210">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="98354-210">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="98354-211">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="98354-211">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="98354-212">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="98354-212">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="98354-213">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="98354-213">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="98354-214">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="98354-214">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="98354-215">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="98354-215">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="98354-216">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="98354-216">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="98354-217">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="98354-217">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="98354-218">[[CAMBIO IMPORTANTE]] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="98354-218">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="98354-219">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="98354-219">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="98354-220">Facturación</span><span class="sxs-lookup"><span data-stu-id="98354-220">Billing</span></span>

* <span data-ttu-id="98354-221">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="98354-221">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="98354-222">Consumo</span><span class="sxs-lookup"><span data-stu-id="98354-222">Consumption</span></span>

* <span data-ttu-id="98354-223">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="98354-223">Added `marketplace` commands</span></span>
* <span data-ttu-id="98354-224">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="98354-224">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="98354-225">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="98354-225">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="98354-226">[[CAMBIO IMPORTANTE]] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="98354-226">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="98354-227">[[CAMBIO IMPORTANTE]] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="98354-227">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="98354-228">[[CAMBIO IMPORTANTE]] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="98354-228">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="98354-229">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-229">Container</span></span>

* <span data-ttu-id="98354-230">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="98354-230">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="98354-231">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="98354-231">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="98354-232">Extensión</span><span class="sxs-lookup"><span data-stu-id="98354-232">Extension</span></span>

* <span data-ttu-id="98354-233">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="98354-233">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-234">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-234">Interactive</span></span>

* <span data-ttu-id="98354-235">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="98354-235">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="98354-236">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="98354-236">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="98354-237">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="98354-237">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="98354-238">Red</span><span class="sxs-lookup"><span data-stu-id="98354-238">Network</span></span>

* <span data-ttu-id="98354-239">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="98354-239">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="98354-240">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="98354-240">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="98354-241">4910</span><span class="sxs-lookup"><span data-stu-id="98354-241">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="98354-242">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="98354-242">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="98354-243">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="98354-243">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="98354-244">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-244">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="98354-245">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-245">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="98354-246">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="98354-246">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="98354-247">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-247">Profile</span></span>

* <span data-ttu-id="98354-248">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="98354-248">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="98354-249">[[CAMBIO IMPORTANTE]] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="98354-249">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="98354-250">RDBMS</span><span class="sxs-lookup"><span data-stu-id="98354-250">RDBMS</span></span>

* <span data-ttu-id="98354-251">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="98354-251">Added `georestore` command</span></span>
* <span data-ttu-id="98354-252">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="98354-252">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="98354-253">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-253">Resource</span></span>

* <span data-ttu-id="98354-254">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="98354-254">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="98354-255">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="98354-255">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="98354-256">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-256">SQL</span></span>

* <span data-ttu-id="98354-257">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="98354-257">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="98354-258">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-258">Storage</span></span>

* <span data-ttu-id="98354-259">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="98354-259">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="98354-260">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-260">VM</span></span>

* <span data-ttu-id="98354-261">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="98354-261">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="98354-262">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="98354-262">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="98354-264">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="98354-264">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="98354-265">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="98354-265">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="98354-266">5718</span><span class="sxs-lookup"><span data-stu-id="98354-266">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="98354-267">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="98354-267">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="98354-268">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-268">March 27, 2018</span></span>

<span data-ttu-id="98354-269">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="98354-269">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="98354-270">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-270">Core</span></span>

* <span data-ttu-id="98354-271">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="98354-271">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="98354-272">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-272">ACS</span></span>

* <span data-ttu-id="98354-273">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="98354-273">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-274">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-274">Appservice</span></span>

* <span data-ttu-id="98354-275">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="98354-275">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="98354-276">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="98354-276">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="98354-277">Backup</span><span class="sxs-lookup"><span data-stu-id="98354-277">Backup</span></span>

* <span data-ttu-id="98354-278">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="98354-278">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="98354-279">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-279">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="98354-280">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="98354-280">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="98354-281">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="98354-281">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="98354-282">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-282">Container</span></span>

* <span data-ttu-id="98354-283">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="98354-283">Added `container exec` command.</span></span> <span data-ttu-id="98354-284">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="98354-284">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="98354-285">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="98354-285">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="98354-286">Extensión</span><span class="sxs-lookup"><span data-stu-id="98354-286">Extension</span></span>

* <span data-ttu-id="98354-287">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="98354-287">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="98354-288">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="98354-288">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="98354-289">[[CAMBIO IMPORTANTE]] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="98354-289">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-290">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-290">Interactive</span></span>

* <span data-ttu-id="98354-291">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="98354-291">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="98354-292">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="98354-292">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="98354-293">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="98354-293">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="98354-294">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="98354-294">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="98354-295">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-295">Lab</span></span>

* <span data-ttu-id="98354-296">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="98354-296">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-297">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-297">Monitor</span></span>

* <span data-ttu-id="98354-298">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="98354-298">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="98354-299">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="98354-299">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="98354-300">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="98354-300">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="98354-301">Red</span><span class="sxs-lookup"><span data-stu-id="98354-301">Network</span></span>

* <span data-ttu-id="98354-302">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="98354-302">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="98354-303">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-303">Profile</span></span>

* <span data-ttu-id="98354-304">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="98354-304">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="98354-305">RDBMS</span><span class="sxs-lookup"><span data-stu-id="98354-305">RDBMS</span></span>

* <span data-ttu-id="98354-306">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="98354-306">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="98354-307">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-307">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="98354-309">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-309">Role</span></span>

* <span data-ttu-id="98354-310">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="98354-310">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="98354-311">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="98354-311">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="98354-312">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="98354-312">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="98354-313">[[CAMBIO IMPORTANTE]] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="98354-313">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="98354-314">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="98354-314">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="98354-315">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-315">Storage</span></span>

* <span data-ttu-id="98354-316">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="98354-316">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="98354-317">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="98354-317">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="98354-318">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-318">VM</span></span>

* <span data-ttu-id="98354-319">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="98354-319">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="98354-320">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="98354-320">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="98354-321">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="98354-321">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="98354-322">[[CAMBIO IMPORTANTE]] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="98354-322">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="98354-323">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-323">March 13, 2018</span></span>

<span data-ttu-id="98354-324">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="98354-324">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="98354-325">ACR</span><span class="sxs-lookup"><span data-stu-id="98354-325">ACR</span></span>

* <span data-ttu-id="98354-326">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="98354-326">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="98354-327">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="98354-327">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="98354-328">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="98354-328">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="98354-329">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-329">ACS</span></span>

* <span data-ttu-id="98354-330">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="98354-330">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="98354-331">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="98354-331">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="98354-332">Advisor</span><span class="sxs-lookup"><span data-stu-id="98354-332">Advisor</span></span>

* <span data-ttu-id="98354-333">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="98354-333">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="98354-334">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="98354-334">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="98354-335">[[CAMBIO IMPORTANTE]] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="98354-335">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="98354-336">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="98354-336">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="98354-337">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="98354-337">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-338">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-338">Appservice</span></span>

* <span data-ttu-id="98354-339">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="98354-339">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="98354-340">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="98354-340">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="98354-341">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="98354-341">Eventhubs</span></span>

* <span data-ttu-id="98354-342">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="98354-342">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="98354-343">Extensión</span><span class="sxs-lookup"><span data-stu-id="98354-343">Extension</span></span>

* <span data-ttu-id="98354-344">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="98354-344">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-345">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-345">Interactive</span></span>

* <span data-ttu-id="98354-346">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="98354-346">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="98354-347">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="98354-347">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="98354-348">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="98354-348">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="98354-349">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="98354-349">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-350">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-350">Monitor</span></span>

* <span data-ttu-id="98354-351">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="98354-351">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="98354-352">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="98354-352">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="98354-353">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="98354-353">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="98354-354">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="98354-354">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="98354-355">Red</span><span class="sxs-lookup"><span data-stu-id="98354-355">Network</span></span>

* <span data-ttu-id="98354-356">[[CAMBIO IMPORTANTE]] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="98354-356">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="98354-357">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="98354-357">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="98354-358">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="98354-358">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="98354-359">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="98354-359">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="98354-360">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-360">Profile</span></span>

* <span data-ttu-id="98354-361">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="98354-361">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="98354-362">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="98354-362">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="98354-363">RDBMS</span><span class="sxs-lookup"><span data-stu-id="98354-363">RDBMS</span></span>

* <span data-ttu-id="98354-364">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="98354-364">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="98354-365">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="98354-365">Service Bus</span></span>

* <span data-ttu-id="98354-366">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="98354-366">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="98354-367">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-367">Storage</span></span>

* <span data-ttu-id="98354-368">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="98354-368">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="98354-369">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="98354-369">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="98354-370">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-370">VM</span></span>

* <span data-ttu-id="98354-371">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="98354-371">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="98354-372">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="98354-372">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="98354-373">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="98354-373">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="98354-374">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="98354-374">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="98354-375">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-375">February 27, 2018</span></span>

<span data-ttu-id="98354-376">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="98354-376">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="98354-377">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-377">Core</span></span>

* <span data-ttu-id="98354-378">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="98354-378">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="98354-379">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="98354-379">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="98354-380">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="98354-380">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="98354-381">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-381">ACS</span></span>

* <span data-ttu-id="98354-382">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="98354-382">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="98354-383">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="98354-383">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="98354-384">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="98354-384">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="98354-385">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="98354-385">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-386">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-386">Appservice</span></span>

* <span data-ttu-id="98354-387">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="98354-387">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="98354-388">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="98354-388">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="98354-389">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="98354-389">Cognitive Services</span></span>

* <span data-ttu-id="98354-390">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="98354-390">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="98354-391">Consumo</span><span class="sxs-lookup"><span data-stu-id="98354-391">Consumption</span></span>

* <span data-ttu-id="98354-392">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="98354-392">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="98354-393">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="98354-393">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="98354-394">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-394">Container</span></span>

* <span data-ttu-id="98354-395">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="98354-395">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="98354-396">Red</span><span class="sxs-lookup"><span data-stu-id="98354-396">Network</span></span>

* <span data-ttu-id="98354-397">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="98354-397">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="98354-398">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-398">Resource</span></span>

* <span data-ttu-id="98354-399">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="98354-399">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="98354-400">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-400">Role</span></span>

* <span data-ttu-id="98354-401">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="98354-401">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="98354-402">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-402">SQL</span></span>

* <span data-ttu-id="98354-403">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="98354-403">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="98354-404">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-404">Storage</span></span>

* <span data-ttu-id="98354-405">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="98354-405">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="98354-406">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-406">VM</span></span>

* <span data-ttu-id="98354-407">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="98354-407">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="98354-408">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-408">February 13, 2018</span></span>

<span data-ttu-id="98354-409">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="98354-409">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="98354-410">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-410">Core</span></span>

* <span data-ttu-id="98354-411">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="98354-411">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="98354-412">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-412">ACS</span></span>

* <span data-ttu-id="98354-413">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="98354-413">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="98354-414">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="98354-414">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="98354-415">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="98354-415">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="98354-416">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="98354-416">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="98354-417">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="98354-417">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="98354-418">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="98354-418">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="98354-419">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="98354-419">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="98354-420">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="98354-420">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-421">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-421">Appservice</span></span>

* <span data-ttu-id="98354-422">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="98354-422">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="98354-423">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="98354-423">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="98354-424">CDN</span><span class="sxs-lookup"><span data-stu-id="98354-424">CDN</span></span>

* <span data-ttu-id="98354-425">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="98354-425">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="98354-426">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-426">Container</span></span>

* <span data-ttu-id="98354-427">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="98354-427">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="98354-428">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="98354-428">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="98354-429">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="98354-429">CosmosDB</span></span>

* <span data-ttu-id="98354-430">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="98354-430">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="98354-431">Extensión</span><span class="sxs-lookup"><span data-stu-id="98354-431">Extension</span></span>

* <span data-ttu-id="98354-432">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-432">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="98354-433">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-433">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="98354-434">Comentarios</span><span class="sxs-lookup"><span data-stu-id="98354-434">Feedback</span></span>

* <span data-ttu-id="98354-435">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="98354-435">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-436">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-436">Interactive</span></span>

* <span data-ttu-id="98354-437">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="98354-437">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="98354-438">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="98354-438">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="98354-439">IoT</span><span class="sxs-lookup"><span data-stu-id="98354-439">IoT</span></span>

* <span data-ttu-id="98354-440">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="98354-440">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="98354-441">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="98354-441">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="98354-442">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-442">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="98354-443">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="98354-443">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-444">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-444">Monitor</span></span>

* <span data-ttu-id="98354-445">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="98354-445">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="98354-446">Red</span><span class="sxs-lookup"><span data-stu-id="98354-446">Network</span></span>

* <span data-ttu-id="98354-447">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="98354-447">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="98354-448">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-448">Profile</span></span>

* <span data-ttu-id="98354-449">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="98354-449">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="98354-450">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-450">Resource</span></span>

* <span data-ttu-id="98354-451">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="98354-451">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="98354-452">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-452">Role</span></span>

* <span data-ttu-id="98354-453">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="98354-453">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="98354-454">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-454">SQL</span></span>

* <span data-ttu-id="98354-455">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="98354-455">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="98354-456">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="98354-456">Added `sql db rename`</span></span>
* <span data-ttu-id="98354-457">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="98354-457">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="98354-458">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-458">Storage</span></span>

* <span data-ttu-id="98354-459">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="98354-459">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="98354-460">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-460">VM</span></span>

* <span data-ttu-id="98354-461">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="98354-461">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="98354-462">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="98354-462">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="98354-463">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="98354-463">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="98354-464">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-464">January 31, 2018</span></span>

<span data-ttu-id="98354-465">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="98354-465">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="98354-466">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-466">Core</span></span>

* <span data-ttu-id="98354-467">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="98354-467">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="98354-468">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="98354-468">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="98354-469">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="98354-469">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="98354-470">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="98354-470">Use `--verbose` to see</span></span>
* <span data-ttu-id="98354-471">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="98354-471">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="98354-472">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-472">ACS</span></span>

* <span data-ttu-id="98354-473">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="98354-473">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="98354-474">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="98354-474">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-475">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-475">Appservice</span></span>

* <span data-ttu-id="98354-476">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="98354-476">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="98354-477">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="98354-477">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="98354-478">CDN</span><span class="sxs-lookup"><span data-stu-id="98354-478">CDN</span></span>

* <span data-ttu-id="98354-479">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="98354-479">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="98354-480">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="98354-480">CosmosDB</span></span>

* <span data-ttu-id="98354-481">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="98354-481">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-482">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-482">Interactive</span></span>

* <span data-ttu-id="98354-483">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="98354-483">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="98354-484">Red</span><span class="sxs-lookup"><span data-stu-id="98354-484">Network</span></span>

* <span data-ttu-id="98354-485">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="98354-485">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="98354-486">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="98354-486">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="98354-487">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="98354-487">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="98354-488">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="98354-488">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="98354-489">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="98354-489">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="98354-490">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="98354-490">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="98354-491">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="98354-491">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="98354-492">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="98354-492">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="98354-493">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="98354-493">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="98354-494">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="98354-494">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="98354-495">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-495">Profile</span></span>

* <span data-ttu-id="98354-496">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="98354-496">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="98354-497">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-497">Resource</span></span>

* <span data-ttu-id="98354-498">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="98354-498">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="98354-499">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-499">Storage</span></span>

* <span data-ttu-id="98354-500">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="98354-500">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="98354-501">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="98354-501">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="98354-502">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="98354-502">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="98354-503">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="98354-503">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="98354-504">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="98354-504">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="98354-505">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-505">VM</span></span>

* <span data-ttu-id="98354-506">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="98354-506">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="98354-507">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="98354-507">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="98354-508">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="98354-508">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="98354-509">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="98354-509">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="98354-510">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="98354-510">January 17, 2018</span></span>

<span data-ttu-id="98354-511">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="98354-511">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="98354-512">ACR</span><span class="sxs-lookup"><span data-stu-id="98354-512">ACR</span></span>

* <span data-ttu-id="98354-513">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="98354-513">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="98354-514">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="98354-514">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="98354-515">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-515">ACS</span></span>

* <span data-ttu-id="98354-516">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="98354-516">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="98354-517">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="98354-517">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-518">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-518">Appservice</span></span>

* <span data-ttu-id="98354-519">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="98354-519">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="98354-520">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="98354-520">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="98354-521">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="98354-521">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="98354-522">Backup</span><span class="sxs-lookup"><span data-stu-id="98354-522">Backup</span></span>

* <span data-ttu-id="98354-523">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="98354-523">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="98354-524">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="98354-524">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="98354-525">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="98354-525">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="98354-526">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="98354-526">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="98354-527">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="98354-527">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="98354-528">Batch</span><span class="sxs-lookup"><span data-stu-id="98354-528">Batch</span></span>

* <span data-ttu-id="98354-529">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="98354-529">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="98354-530">Nube</span><span class="sxs-lookup"><span data-stu-id="98354-530">Cloud</span></span>

* <span data-ttu-id="98354-531">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="98354-531">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="98354-532">Consumo</span><span class="sxs-lookup"><span data-stu-id="98354-532">Consumption</span></span>

* <span data-ttu-id="98354-533">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="98354-533">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="98354-534">Event Grid</span><span class="sxs-lookup"><span data-stu-id="98354-534">Event Grid</span></span>

* <span data-ttu-id="98354-535">[[CAMBIO IMPORTANTE]] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="98354-535">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="98354-536">[[CAMBIO IMPORTANTE]] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="98354-536">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="98354-537">[[CAMBIO IMPORTANTE]] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="98354-537">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="98354-538">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="98354-538">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="98354-539">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="98354-539">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="98354-540">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="98354-540">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="98354-541">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="98354-541">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="98354-542">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="98354-542">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-543">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-543">Interactive</span></span>

* <span data-ttu-id="98354-544">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="98354-544">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="98354-545">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="98354-545">Fixed errors on startup</span></span>
* <span data-ttu-id="98354-546">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="98354-546">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="98354-547">IoT</span><span class="sxs-lookup"><span data-stu-id="98354-547">IoT</span></span>

* <span data-ttu-id="98354-548">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="98354-548">Added support for device provisioning service</span></span>
* <span data-ttu-id="98354-549">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="98354-549">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="98354-550">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="98354-550">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-551">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-551">Monitor</span></span>

* <span data-ttu-id="98354-552">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="98354-552">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="98354-553">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="98354-553">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="98354-554">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="98354-554">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="98354-555">Red</span><span class="sxs-lookup"><span data-stu-id="98354-555">Network</span></span>

* <span data-ttu-id="98354-556">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="98354-556">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="98354-557">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-557">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="98354-558">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-558">Profile</span></span>

* <span data-ttu-id="98354-559">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="98354-559">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="98354-560">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-560">Role</span></span>

* <span data-ttu-id="98354-561">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="98354-561">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="98354-562">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="98354-562">Service Fabric</span></span>

* <span data-ttu-id="98354-563">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="98354-563">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="98354-564">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="98354-564">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="98354-565">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-565">VM</span></span>

* <span data-ttu-id="98354-566">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="98354-566">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="98354-567">[[CAMBIO IMPORTANTE]] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="98354-567">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="98354-568">[[CAMBIO IMPORTANTE]] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="98354-568">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="98354-569">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="98354-569">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="98354-570">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="98354-570">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="98354-571">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="98354-571">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="98354-572">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="98354-572">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="98354-573">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="98354-573">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="98354-574">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-574">December 19, 2017</span></span>

<span data-ttu-id="98354-575">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="98354-575">Version 2.0.23</span></span>

* <span data-ttu-id="98354-576">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="98354-576">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="98354-577">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-577">Container</span></span>

* <span data-ttu-id="98354-578">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-578">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="98354-579">Red</span><span class="sxs-lookup"><span data-stu-id="98354-579">Network</span></span>

* <span data-ttu-id="98354-580">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-580">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="98354-581">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-581">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="98354-582">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-582">Storage</span></span>

* <span data-ttu-id="98354-583">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="98354-583">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="98354-584">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-584">VM</span></span>

* <span data-ttu-id="98354-585">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="98354-585">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="98354-586">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-586">December 5, 2017</span></span>

<span data-ttu-id="98354-587">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="98354-587">Version 2.0.22</span></span>

* <span data-ttu-id="98354-588">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="98354-588">Removed `az component` commands.</span></span> <span data-ttu-id="98354-589">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="98354-589">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="98354-590">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-590">Core</span></span>
* <span data-ttu-id="98354-591">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="98354-591">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="98354-592">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="98354-592">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="98354-593">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-593">ACS</span></span>

* <span data-ttu-id="98354-594">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="98354-594">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="98354-595">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="98354-595">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="98354-596">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="98354-596">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="98354-597">Advisor</span><span class="sxs-lookup"><span data-stu-id="98354-597">Advisor</span></span>

* <span data-ttu-id="98354-598">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="98354-598">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-599">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-599">Appservice</span></span>

* <span data-ttu-id="98354-600">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="98354-600">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="98354-601">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="98354-601">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="98354-602">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="98354-602">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="98354-603">Consumo</span><span class="sxs-lookup"><span data-stu-id="98354-603">Consumption</span></span>

* <span data-ttu-id="98354-604">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="98354-604">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="98354-605">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-605">Container</span></span>

* <span data-ttu-id="98354-606">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="98354-606">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-607">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-607">Monitor</span></span>

* <span data-ttu-id="98354-608">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="98354-608">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="98354-609">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-609">Resource</span></span>

* <span data-ttu-id="98354-610">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="98354-610">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="98354-611">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-611">Role</span></span>

* <span data-ttu-id="98354-612">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="98354-612">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="98354-613">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="98354-613">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="98354-614">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="98354-614">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="98354-615">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-615">SQL</span></span>

* <span data-ttu-id="98354-616">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="98354-616">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="98354-617">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="98354-617">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="98354-618">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-618">VM</span></span>

* <span data-ttu-id="98354-619">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="98354-619">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="98354-620">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-620">November 14, 2017</span></span>

<span data-ttu-id="98354-621">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="98354-621">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="98354-622">ACR</span><span class="sxs-lookup"><span data-stu-id="98354-622">ACR</span></span>

* <span data-ttu-id="98354-623">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="98354-623">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="98354-624">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-624">ACS</span></span>

* <span data-ttu-id="98354-625">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="98354-625">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="98354-626">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="98354-626">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="98354-627">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="98354-627">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="98354-628">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="98354-628">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="98354-629">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="98354-629">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-630">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-630">Appservice</span></span>

* <span data-ttu-id="98354-631">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="98354-631">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="98354-632">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="98354-632">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="98354-633">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="98354-633">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="98354-634">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="98354-634">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="98354-635">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="98354-635">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="98354-636">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="98354-636">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="98354-637">Batch</span><span class="sxs-lookup"><span data-stu-id="98354-637">Batch</span></span>

* <span data-ttu-id="98354-638">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="98354-638">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="98354-639">Batchai</span><span class="sxs-lookup"><span data-stu-id="98354-639">Batchai</span></span>

* <span data-ttu-id="98354-640">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="98354-640">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="98354-641">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="98354-641">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="98354-642">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="98354-642">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="98354-643">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="98354-643">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="98354-644">Nube</span><span class="sxs-lookup"><span data-stu-id="98354-644">Cloud</span></span>

* <span data-ttu-id="98354-645">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="98354-645">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="98354-646">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-646">Container</span></span>

* <span data-ttu-id="98354-647">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="98354-647">Added support to open multiple ports</span></span>
* <span data-ttu-id="98354-648">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="98354-648">Added container group restart policy</span></span>
* <span data-ttu-id="98354-649">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="98354-649">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="98354-650">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="98354-650">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="98354-651">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="98354-651">Data Lake Analytics</span></span>

* <span data-ttu-id="98354-652">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="98354-652">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="98354-653">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="98354-653">Data Lake Store</span></span>

* <span data-ttu-id="98354-654">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="98354-654">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="98354-655">Extensión</span><span class="sxs-lookup"><span data-stu-id="98354-655">Extension</span></span>

* <span data-ttu-id="98354-656">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="98354-656">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="98354-657">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="98354-657">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="98354-658">IoT</span><span class="sxs-lookup"><span data-stu-id="98354-658">IoT</span></span>

* <span data-ttu-id="98354-659">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="98354-659">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-660">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-660">Monitor</span></span>

* <span data-ttu-id="98354-661">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="98354-661">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="98354-662">Red</span><span class="sxs-lookup"><span data-stu-id="98354-662">Network</span></span>

* <span data-ttu-id="98354-663">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="98354-663">Added support for CAA DNS records</span></span>
* <span data-ttu-id="98354-664">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="98354-664">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="98354-665">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="98354-665">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="98354-666">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="98354-666">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="98354-667">Reservations</span><span class="sxs-lookup"><span data-stu-id="98354-667">Reservations</span></span>

* <span data-ttu-id="98354-668">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="98354-668">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="98354-669">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-669">Resource</span></span>

* <span data-ttu-id="98354-670">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="98354-670">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="98354-671">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-671">SQL</span></span>

* <span data-ttu-id="98354-672">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-672">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="98354-673">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-673">Storage</span></span>

* <span data-ttu-id="98354-674">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="98354-674">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="98354-675">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="98354-675">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="98354-676">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="98354-676">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="98354-677">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="98354-677">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="98354-678">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="98354-678">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="98354-679">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="98354-679">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="98354-680">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="98354-680">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="98354-681">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-681">VM</span></span>

* <span data-ttu-id="98354-682">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="98354-682">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="98354-683">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="98354-683">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="98354-684">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="98354-684">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="98354-685">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="98354-685">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="98354-686">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="98354-686">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="98354-687">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-687">October 24, 2017</span></span>

<span data-ttu-id="98354-688">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="98354-688">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="98354-689">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-689">Core</span></span>

* <span data-ttu-id="98354-690">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="98354-690">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="98354-691">ACR</span><span class="sxs-lookup"><span data-stu-id="98354-691">ACR</span></span>

* <span data-ttu-id="98354-692">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="98354-692">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="98354-693">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="98354-693">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="98354-694">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="98354-694">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="98354-695">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-695">ACS</span></span>

* <span data-ttu-id="98354-696">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="98354-696">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="98354-697">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="98354-697">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-698">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-698">Appservice</span></span>

* <span data-ttu-id="98354-699">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="98354-699">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="98354-700">Componente</span><span class="sxs-lookup"><span data-stu-id="98354-700">Component</span></span>

* <span data-ttu-id="98354-701">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="98354-701">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-702">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-702">Monitor</span></span>

* <span data-ttu-id="98354-703">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="98354-703">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="98354-704">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-704">Resource</span></span>

* <span data-ttu-id="98354-705">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="98354-705">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="98354-706">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="98354-706">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="98354-707">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-707">VM</span></span>

* <span data-ttu-id="98354-708">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="98354-708">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="98354-709">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-709">October 9, 2017</span></span>

<span data-ttu-id="98354-710">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="98354-710">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="98354-711">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-711">Core</span></span>

* <span data-ttu-id="98354-712">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="98354-712">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-713">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-713">Appservice</span></span>

* <span data-ttu-id="98354-714">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="98354-714">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="98354-715">Batch</span><span class="sxs-lookup"><span data-stu-id="98354-715">Batch</span></span>

* <span data-ttu-id="98354-716">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="98354-716">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="98354-717">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="98354-717">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="98354-718">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="98354-718">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="98354-719">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="98354-719">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="98354-720">Batchai</span><span class="sxs-lookup"><span data-stu-id="98354-720">Batchai</span></span>

* <span data-ttu-id="98354-721">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="98354-721">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="98354-722">Keyvault</span><span class="sxs-lookup"><span data-stu-id="98354-722">Keyvault</span></span>

* <span data-ttu-id="98354-723">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="98354-723">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="98354-724">(#4448)</span><span class="sxs-lookup"><span data-stu-id="98354-724">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="98354-725">Red</span><span class="sxs-lookup"><span data-stu-id="98354-725">Network</span></span>

* <span data-ttu-id="98354-726">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="98354-726">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="98354-727">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="98354-727">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="98354-728">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-728">Resource</span></span>

* <span data-ttu-id="98354-729">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="98354-729">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="98354-730">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="98354-730">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="98354-731">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="98354-731">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="98354-732">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="98354-732">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="98354-733">Sql</span><span class="sxs-lookup"><span data-stu-id="98354-733">Sql</span></span>

* <span data-ttu-id="98354-734">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="98354-734">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="98354-735">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="98354-735">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="98354-736">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="98354-736">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="98354-737">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-737">Storage</span></span>

* <span data-ttu-id="98354-738">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="98354-738">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="98354-739">Vm</span><span class="sxs-lookup"><span data-stu-id="98354-739">Vm</span></span>

* <span data-ttu-id="98354-740">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="98354-740">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="98354-741">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="98354-741">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="98354-742">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="98354-742">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="98354-743">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="98354-743">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="98354-744">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="98354-744">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="98354-745">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-745">September 22, 2017</span></span>

<span data-ttu-id="98354-746">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="98354-746">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="98354-747">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-747">Resource</span></span>

* <span data-ttu-id="98354-748">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="98354-748">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="98354-749">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="98354-749">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="98354-750">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="98354-750">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="98354-751">[[CAMBIO IMPORTANTE]] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="98354-751">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="98354-752">Red</span><span class="sxs-lookup"><span data-stu-id="98354-752">Network</span></span>

* <span data-ttu-id="98354-753">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="98354-753">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="98354-754">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="98354-754">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="98354-755">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="98354-755">Added `asg` application security group commands</span></span>
* <span data-ttu-id="98354-756">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="98354-756">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="98354-757">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-757">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="98354-758">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-758">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="98354-759">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="98354-759">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="98354-760">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-760">Storage</span></span>

* <span data-ttu-id="98354-761">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="98354-761">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="98354-762">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="98354-762">Eventgrid</span></span>

* <span data-ttu-id="98354-763">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="98354-763">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="98354-764">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-764">SQL</span></span>

* <span data-ttu-id="98354-765">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="98354-765">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="98354-766">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="98354-766">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="98354-767">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-767">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="98354-768">Keyvault</span><span class="sxs-lookup"><span data-stu-id="98354-768">Keyvault</span></span>

* <span data-ttu-id="98354-769">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="98354-769">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="98354-770">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-770">VM</span></span>

* <span data-ttu-id="98354-771">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="98354-771">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="98354-772">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="98354-772">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="98354-773">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="98354-773">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="98354-774">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="98354-774">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="98354-775">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="98354-775">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="98354-776">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="98354-776">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="98354-777">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-777">ACS</span></span>

* <span data-ttu-id="98354-778">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="98354-778">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-779">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-779">Appservice</span></span>

* <span data-ttu-id="98354-780">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="98354-780">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="98354-781">Backup</span><span class="sxs-lookup"><span data-stu-id="98354-781">Backup</span></span>

* <span data-ttu-id="98354-782">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="98354-782">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="98354-783">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-783">September 11, 2017</span></span>

<span data-ttu-id="98354-784">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="98354-784">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="98354-785">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-785">Core</span></span>

* <span data-ttu-id="98354-786">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="98354-786">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="98354-787">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="98354-787">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="98354-788">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-788">Acs</span></span>

* <span data-ttu-id="98354-789">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="98354-789">Added `acs list-locations` command</span></span>
* <span data-ttu-id="98354-790">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="98354-790">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-791">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-791">Appservice</span></span>

* <span data-ttu-id="98354-792">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="98354-792">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="98354-793">CDN</span><span class="sxs-lookup"><span data-stu-id="98354-793">CDN</span></span>

* <span data-ttu-id="98354-794">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="98354-794">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="98354-795">Extensión</span><span class="sxs-lookup"><span data-stu-id="98354-795">Extension</span></span>

* <span data-ttu-id="98354-796">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="98354-796">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="98354-797">Keyvault</span><span class="sxs-lookup"><span data-stu-id="98354-797">Keyvault</span></span>

* <span data-ttu-id="98354-798">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="98354-798">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="98354-799">Red</span><span class="sxs-lookup"><span data-stu-id="98354-799">Network</span></span>

* <span data-ttu-id="98354-800">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="98354-800">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="98354-801">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="98354-801">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="98354-802">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="98354-802">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="98354-803">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="98354-803">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="98354-804">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="98354-804">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="98354-805">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-805">Resource</span></span>

* <span data-ttu-id="98354-806">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="98354-806">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="98354-807">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="98354-807">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="98354-808">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="98354-808">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="98354-809">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="98354-809">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="98354-810">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-810">SQL</span></span>

* <span data-ttu-id="98354-811">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="98354-811">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="98354-812">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-812">VM</span></span>

* <span data-ttu-id="98354-813">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="98354-813">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="98354-814">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="98354-814">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="98354-815">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="98354-815">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="98354-816">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="98354-816">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="98354-817">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="98354-817">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="98354-818">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-818">August 31, 2017</span></span>

<span data-ttu-id="98354-819">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="98354-819">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="98354-820">Keyvault</span><span class="sxs-lookup"><span data-stu-id="98354-820">Keyvault</span></span>

* <span data-ttu-id="98354-821">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="98354-821">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="98354-822">Sf</span><span class="sxs-lookup"><span data-stu-id="98354-822">Sf</span></span>

* <span data-ttu-id="98354-823">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="98354-823">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="98354-824">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-824">Storage</span></span>

* <span data-ttu-id="98354-825">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="98354-825">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="98354-826">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="98354-826">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="98354-827">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-827">August 28, 2017</span></span>

<span data-ttu-id="98354-828">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="98354-828">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="98354-829">CLI</span><span class="sxs-lookup"><span data-stu-id="98354-829">CLI</span></span>

* <span data-ttu-id="98354-830">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="98354-830">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="98354-831">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-831">ACS</span></span>

* <span data-ttu-id="98354-832">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="98354-832">Corrected preview regions</span></span>
* <span data-ttu-id="98354-833">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="98354-833">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="98354-834">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="98354-834">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-835">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-835">Appservice</span></span>

* <span data-ttu-id="98354-836">[[CAMBIO IMPORTANTE]] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="98354-836">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="98354-837">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="98354-837">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="98354-838">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="98354-838">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="98354-839">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="98354-839">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="98354-840">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="98354-840">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="98354-841">IoT</span><span class="sxs-lookup"><span data-stu-id="98354-841">IoT</span></span>

* <span data-ttu-id="98354-842">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="98354-842">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="98354-843">Red</span><span class="sxs-lookup"><span data-stu-id="98354-843">Network</span></span>

* <span data-ttu-id="98354-844">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="98354-844">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="98354-845">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="98354-845">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="98354-846">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="98354-846">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="98354-847">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="98354-847">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="98354-848">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="98354-848">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="98354-849">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-849">Profile</span></span>

* <span data-ttu-id="98354-850">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="98354-850">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="98354-851">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="98354-851">Service Fabric</span></span>

* <span data-ttu-id="98354-852">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="98354-852">Preview release</span></span>
* <span data-ttu-id="98354-853">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="98354-853">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="98354-854">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="98354-854">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="98354-855">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="98354-855">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="98354-856">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-856">Storage</span></span>

* <span data-ttu-id="98354-857">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="98354-857">Enabled setting blob tier</span></span>
* <span data-ttu-id="98354-858">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="98354-858">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="98354-859">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="98354-859">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="98354-860">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="98354-860">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="98354-861">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="98354-861">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="98354-862">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="98354-862">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="98354-863">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-863">VM</span></span>

* <span data-ttu-id="98354-864">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="98354-864">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="98354-865">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="98354-865">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="98354-866">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="98354-866">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="98354-867">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="98354-867">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="98354-868">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="98354-868">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="98354-869">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="98354-869">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="98354-870">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-870">August 15, 2017</span></span>

<span data-ttu-id="98354-871">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="98354-871">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="98354-872">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-872">ACS</span></span>

* <span data-ttu-id="98354-873">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="98354-873">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-874">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-874">Appservice</span></span>

* <span data-ttu-id="98354-875">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="98354-875">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="98354-876">Event Grid</span><span class="sxs-lookup"><span data-stu-id="98354-876">Event Grid</span></span>

* <span data-ttu-id="98354-877">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="98354-877">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="98354-878">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-878">August 11, 2017</span></span>

<span data-ttu-id="98354-879">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="98354-879">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="98354-880">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-880">ACS</span></span>

* <span data-ttu-id="98354-881">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="98354-881">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="98354-882">Batch</span><span class="sxs-lookup"><span data-stu-id="98354-882">Batch</span></span>

* <span data-ttu-id="98354-883">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="98354-883">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="98354-884">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="98354-884">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="98354-885">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="98354-885">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="98354-886">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="98354-886">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="98354-887">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="98354-887">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="98354-888">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="98354-888">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="98354-889">Componente</span><span class="sxs-lookup"><span data-stu-id="98354-889">Component</span></span>

* <span data-ttu-id="98354-890">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="98354-890">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="98354-891">Contenedor</span><span class="sxs-lookup"><span data-stu-id="98354-891">Container</span></span>

* <span data-ttu-id="98354-892">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="98354-892">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="98354-893">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="98354-893">Data Lake Store</span></span>

* <span data-ttu-id="98354-894">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="98354-894">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="98354-895">Event Grid</span><span class="sxs-lookup"><span data-stu-id="98354-895">Event Grid</span></span>

* <span data-ttu-id="98354-896">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="98354-896">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="98354-897">Red</span><span class="sxs-lookup"><span data-stu-id="98354-897">Network</span></span>

* <span data-ttu-id="98354-898">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="98354-898">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="98354-899">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="98354-899">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="98354-900">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="98354-900">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="98354-901">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="98354-901">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="98354-902">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-902">Profile</span></span>

* <span data-ttu-id="98354-903">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="98354-903">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="98354-904">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-904">Storage</span></span>

* <span data-ttu-id="98354-905">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="98354-905">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="98354-906">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-906">VM</span></span>

* <span data-ttu-id="98354-907">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="98354-907">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="98354-908">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="98354-908">Exposed `list-skus` command</span></span>
* <span data-ttu-id="98354-909">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="98354-909">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="98354-910">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="98354-910">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="98354-911">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="98354-911">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="98354-912">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-912">July 28, 2017</span></span>

<span data-ttu-id="98354-913">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="98354-913">Version 2.0.12</span></span>

* <span data-ttu-id="98354-914">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="98354-914">Added container commands</span></span>
* <span data-ttu-id="98354-915">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="98354-915">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="98354-916">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-916">Core</span></span>

* <span data-ttu-id="98354-917">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="98354-917">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="98354-918">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="98354-918">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="98354-919">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="98354-919">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="98354-920">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="98354-920">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="98354-921">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="98354-921">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="98354-922">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="98354-922">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="98354-923">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="98354-923">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="98354-924">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="98354-924">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="98354-925">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="98354-925">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="98354-926">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="98354-926">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="98354-927">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="98354-927">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="98354-928">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="98354-928">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="98354-929">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="98354-929">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="98354-930">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="98354-930">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="98354-931">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="98354-931">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="98354-932">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="98354-932">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="98354-933">ACR</span><span class="sxs-lookup"><span data-stu-id="98354-933">ACR</span></span>

* <span data-ttu-id="98354-934">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="98354-934">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="98354-935">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="98354-935">Support SKU update for managed registries</span></span>
* <span data-ttu-id="98354-936">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="98354-936">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="98354-937">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="98354-937">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="98354-938">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="98354-938">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="98354-939">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="98354-939">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="98354-940">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-940">ACS</span></span>

* <span data-ttu-id="98354-941">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="98354-941">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-942">Appservice</span><span class="sxs-lookup"><span data-stu-id="98354-942">Appservice</span></span>

* <span data-ttu-id="98354-943">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="98354-943">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="98354-944">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="98354-944">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="98354-945">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="98354-945">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="98354-946">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="98354-946">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="98354-947">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="98354-947">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="98354-948">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="98354-948">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="98354-949">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="98354-949">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="98354-950">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="98354-950">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="98354-951">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="98354-951">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="98354-952">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="98354-952">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="98354-953">Batch</span><span class="sxs-lookup"><span data-stu-id="98354-953">Batch</span></span>

* <span data-ttu-id="98354-954">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="98354-954">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="98354-955">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="98354-955">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="98354-956">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="98354-956">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="98354-957">CDN</span><span class="sxs-lookup"><span data-stu-id="98354-957">CDN</span></span>

* <span data-ttu-id="98354-958">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="98354-958">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="98354-959">Nube</span><span class="sxs-lookup"><span data-stu-id="98354-959">Cloud</span></span>

* <span data-ttu-id="98354-960">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="98354-960">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="98354-961">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="98354-961">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="98354-962">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="98354-962">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="98354-963">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="98354-963">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="98354-964">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="98354-964">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="98354-965">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="98354-965">CosmosDB</span></span>

* <span data-ttu-id="98354-966">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="98354-966">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="98354-967">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="98354-967">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="98354-968">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="98354-968">Data Lake Analytics</span></span>

* <span data-ttu-id="98354-969">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="98354-969">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="98354-970">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="98354-970">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="98354-971">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="98354-971">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="98354-972">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="98354-972">Data Lake Store</span></span>

* <span data-ttu-id="98354-973">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="98354-973">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="98354-974">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="98354-974">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="98354-975">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="98354-975">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="98354-976">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="98354-976">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="98354-977">Interactive</span><span class="sxs-lookup"><span data-stu-id="98354-977">Interactive</span></span>

* <span data-ttu-id="98354-978">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="98354-978">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="98354-979">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="98354-979">Increased test coverage</span></span>
* <span data-ttu-id="98354-980">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="98354-980">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="98354-981">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="98354-981">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="98354-982">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="98354-982">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="98354-983">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="98354-983">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="98354-984">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="98354-984">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="98354-985">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="98354-985">Added `--progress` flag</span></span>
* <span data-ttu-id="98354-986">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="98354-986">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="98354-987">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="98354-987">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="98354-988">IoT</span><span class="sxs-lookup"><span data-stu-id="98354-988">IoT</span></span>

* <span data-ttu-id="98354-989">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="98354-989">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="98354-990">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="98354-990">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="98354-991">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="98354-991">Key vault</span></span>

* <span data-ttu-id="98354-992">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="98354-992">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="98354-993">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="98354-993">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="98354-994">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="98354-994">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="98354-995">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="98354-995">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="98354-996">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="98354-996">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="98354-997">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="98354-997">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="98354-998">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="98354-998">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="98354-999">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="98354-999">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="98354-1000">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-1000">Lab</span></span>

* <span data-ttu-id="98354-1001">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="98354-1001">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="98354-1002">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="98354-1002">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-1003">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-1003">Monitor</span></span>

* <span data-ttu-id="98354-1004">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="98354-1004">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="98354-1005">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="98354-1005">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="98354-1006">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="98354-1006">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="98354-1007">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="98354-1007">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="98354-1008">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="98354-1008">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="98354-1009">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="98354-1009">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="98354-1010">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="98354-1010">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="98354-1011">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="98354-1011">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="98354-1012">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="98354-1012">`location` no longer required</span></span>
  * <span data-ttu-id="98354-1013">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="98354-1013">Add name and ID support for target</span></span>
  * <span data-ttu-id="98354-1014">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="98354-1014">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="98354-1015">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="98354-1015">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="98354-1016">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="98354-1016">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="98354-1017">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="98354-1017">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="98354-1018">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="98354-1018">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="98354-1019">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="98354-1019">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="98354-1020">Red</span><span class="sxs-lookup"><span data-stu-id="98354-1020">Network</span></span>

* <span data-ttu-id="98354-1021">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="98354-1021">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="98354-1022">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="98354-1022">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="98354-1023">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="98354-1023">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="98354-1024">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="98354-1024">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="98354-1025">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="98354-1025">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="98354-1026">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="98354-1026">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="98354-1027">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="98354-1027">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="98354-1028">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="98354-1028">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="98354-1029">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="98354-1029">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="98354-1030">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="98354-1030">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="98354-1031">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="98354-1031">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="98354-1032">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="98354-1032">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="98354-1033">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="98354-1033">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="98354-1034">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="98354-1034">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="98354-1035">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="98354-1035">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="98354-1036">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="98354-1036">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="98354-1037">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="98354-1037">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="98354-1038">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="98354-1038">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="98354-1039">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="98354-1039">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="98354-1040">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="98354-1040">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="98354-1041">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="98354-1041">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="98354-1042">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="98354-1042">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="98354-1043">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="98354-1043">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="98354-1044">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="98354-1044">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="98354-1045">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="98354-1045">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="98354-1046">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="98354-1046">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="98354-1047">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="98354-1047">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="98354-1048">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-1048">Profile</span></span>

* <span data-ttu-id="98354-1049">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="98354-1049">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="98354-1050">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="98354-1050">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="98354-1051">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="98354-1051">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="98354-1052">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="98354-1052">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="98354-1053">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="98354-1053">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="98354-1054">RDBMS</span><span class="sxs-lookup"><span data-stu-id="98354-1054">RDBMS</span></span>

* <span data-ttu-id="98354-1055">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="98354-1055">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="98354-1056">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="98354-1056">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="98354-1057">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="98354-1057">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="98354-1058">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="98354-1058">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="98354-1059">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-1059">Resource</span></span>

* <span data-ttu-id="98354-1060">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="98354-1060">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="98354-1061">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="98354-1061">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="98354-1062">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="98354-1062">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="98354-1063">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="98354-1063">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="98354-1064">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="98354-1064">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="98354-1065">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="98354-1065">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="98354-1066">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="98354-1066">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="98354-1067">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="98354-1067">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="98354-1068">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-1068">Role</span></span>

* <span data-ttu-id="98354-1069">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="98354-1069">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="98354-1070">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="98354-1070">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="98354-1071">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="98354-1071">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="98354-1072">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="98354-1072">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="98354-1073">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="98354-1073">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="98354-1074">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="98354-1074">Service Fabric</span></span>
* <span data-ttu-id="98354-1075">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="98354-1075">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="98354-1076">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="98354-1076">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="98354-1077">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="98354-1077">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="98354-1078">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-1078">SQL</span></span>

* <span data-ttu-id="98354-1079">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="98354-1079">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="98354-1080">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="98354-1080">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="98354-1081">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="98354-1081">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="98354-1082">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-1082">Storage</span></span>

* <span data-ttu-id="98354-1083">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="98354-1083">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="98354-1084">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="98354-1084">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="98354-1085">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="98354-1085">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="98354-1086">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="98354-1086">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="98354-1087">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="98354-1087">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="98354-1088">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="98354-1088">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="98354-1089">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-1089">VM</span></span>

* <span data-ttu-id="98354-1090">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="98354-1090">Support configuring nsg</span></span>
* <span data-ttu-id="98354-1091">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="98354-1091">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="98354-1092">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="98354-1092">Support managed service identities</span></span>
* <span data-ttu-id="98354-1093">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="98354-1093">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="98354-1094">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="98354-1094">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="98354-1095">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-1095">May 10, 2017</span></span>

<span data-ttu-id="98354-1096">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="98354-1096">Version 2.0.6</span></span>

* <span data-ttu-id="98354-1097">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="98354-1097">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="98354-1098">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="98354-1098">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="98354-1099">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="98354-1099">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="98354-1100">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="98354-1100">Include Cognitive Services module</span></span>
* <span data-ttu-id="98354-1101">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="98354-1101">Include Service Fabric module</span></span>
* <span data-ttu-id="98354-1102">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="98354-1102">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="98354-1103">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="98354-1103">Add support for CDN commands</span></span>
* <span data-ttu-id="98354-1104">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="98354-1104">Remove Container module</span></span>
* <span data-ttu-id="98354-1105">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="98354-1105">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="98354-1106">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="98354-1106">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="98354-1107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-1107">Core</span></span>

* <span data-ttu-id="98354-1108">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="98354-1108">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="98354-1109">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="98354-1109">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="98354-1110">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="98354-1110">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="98354-1111">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="98354-1111">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="98354-1112">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="98354-1112">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="98354-1113">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="98354-1113">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="98354-1114">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="98354-1114">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="98354-1115">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="98354-1115">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="98354-1116">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="98354-1116">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="98354-1117">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="98354-1117">core: Improved performance</span></span>
* <span data-ttu-id="98354-1118">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="98354-1118">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="98354-1119">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="98354-1119">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="98354-1120">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-1120">ACS</span></span>

* <span data-ttu-id="98354-1121">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="98354-1121">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="98354-1122">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="98354-1122">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="98354-1123">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="98354-1123">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="98354-1124">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="98354-1124">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-1125">AppService</span><span class="sxs-lookup"><span data-stu-id="98354-1125">AppService</span></span>

* <span data-ttu-id="98354-1126">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="98354-1126">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="98354-1127">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="98354-1127">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="98354-1128">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="98354-1128">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="98354-1129">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="98354-1129">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="98354-1130">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="98354-1130">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="98354-1131">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="98354-1131">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="98354-1132">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="98354-1132">support slot swap with preview</span></span>
* <span data-ttu-id="98354-1133">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="98354-1133">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="98354-1134">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="98354-1134">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="98354-1135">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="98354-1135">CosmosDB</span></span>

* <span data-ttu-id="98354-1136">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="98354-1136">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="98354-1137">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="98354-1137">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="98354-1138">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="98354-1138">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="98354-1139">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="98354-1139">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="98354-1140">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="98354-1140">Data Lake Analytics</span></span>

* <span data-ttu-id="98354-1141">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="98354-1141">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="98354-1142">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="98354-1142">Add support for new catalog item type: package.</span></span> <span data-ttu-id="98354-1143">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="98354-1143">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="98354-1144">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="98354-1144">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="98354-1145">Tabla</span><span class="sxs-lookup"><span data-stu-id="98354-1145">Table</span></span>
  * <span data-ttu-id="98354-1146">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="98354-1146">Table valued function</span></span>
  * <span data-ttu-id="98354-1147">Ver</span><span class="sxs-lookup"><span data-stu-id="98354-1147">View</span></span>
  * <span data-ttu-id="98354-1148">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="98354-1148">Table Statistics.</span></span> <span data-ttu-id="98354-1149">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="98354-1149">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="98354-1150">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="98354-1150">Data Lake Store</span></span>

* <span data-ttu-id="98354-1151">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="98354-1151">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="98354-1152">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="98354-1152">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="98354-1153">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="98354-1153">missed help for access show.</span></span> <span data-ttu-id="98354-1154">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="98354-1154">adding it.</span></span> <span data-ttu-id="98354-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="98354-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="98354-1156">Buscar</span><span class="sxs-lookup"><span data-stu-id="98354-1156">Find</span></span>

* <span data-ttu-id="98354-1157">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="98354-1157">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="98354-1158">KeyVault</span><span class="sxs-lookup"><span data-stu-id="98354-1158">KeyVault</span></span>

* <span data-ttu-id="98354-1159">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="98354-1159">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="98354-1160">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="98354-1160">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="98354-1161">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="98354-1161">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="98354-1162">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="98354-1162">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="98354-1163">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="98354-1163">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="98354-1164">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-1164">Lab</span></span>

* <span data-ttu-id="98354-1165">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-1165">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="98354-1166">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-1166">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="98354-1167">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-1167">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="98354-1168">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-1168">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="98354-1169">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="98354-1169">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="98354-1170">Supervisión</span><span class="sxs-lookup"><span data-stu-id="98354-1170">Monitor</span></span>

* <span data-ttu-id="98354-1171">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="98354-1171">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="98354-1172">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="98354-1172">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="98354-1173">Red</span><span class="sxs-lookup"><span data-stu-id="98354-1173">Network</span></span>

* <span data-ttu-id="98354-1174">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="98354-1174">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="98354-1175">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="98354-1175">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="98354-1176">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="98354-1176">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="98354-1177">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="98354-1177">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="98354-1178">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="98354-1178">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="98354-1179">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="98354-1179">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="98354-1180">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="98354-1180">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="98354-1181">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="98354-1181">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="98354-1182">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="98354-1182">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="98354-1183">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="98354-1183">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="98354-1184">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="98354-1184">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="98354-1185">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="98354-1185">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="98354-1186">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="98354-1186">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="98354-1187">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="98354-1187">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="98354-1188">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="98354-1188">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="98354-1189">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="98354-1189">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="98354-1190">Perfil</span><span class="sxs-lookup"><span data-stu-id="98354-1190">Profile</span></span>

* <span data-ttu-id="98354-1191">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="98354-1191">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="98354-1192">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="98354-1192">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="98354-1193">Redis</span><span class="sxs-lookup"><span data-stu-id="98354-1193">Redis</span></span>

* <span data-ttu-id="98354-1194">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="98354-1194">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="98354-1195">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="98354-1195">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="98354-1196">Recurso</span><span class="sxs-lookup"><span data-stu-id="98354-1196">Resource</span></span>

* <span data-ttu-id="98354-1197">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="98354-1197">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="98354-1198">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="98354-1198">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="98354-1199">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="98354-1199">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="98354-1200">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="98354-1200">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="98354-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="98354-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="98354-1202">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="98354-1202">Add docs for az lock update.</span></span> <span data-ttu-id="98354-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="98354-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="98354-1204">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="98354-1204">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="98354-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="98354-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="98354-1206">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="98354-1206">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="98354-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="98354-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="98354-1208">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="98354-1208">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="98354-1209">Rol</span><span class="sxs-lookup"><span data-stu-id="98354-1209">Role</span></span>

* <span data-ttu-id="98354-1210">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="98354-1210">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="98354-1211">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="98354-1211">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="98354-1212">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="98354-1212">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="98354-1213">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="98354-1213">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="98354-1214">SQL</span><span class="sxs-lookup"><span data-stu-id="98354-1214">SQL</span></span>

* <span data-ttu-id="98354-1215">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="98354-1215">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="98354-1216">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="98354-1216">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="98354-1217">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-1217">Storage</span></span>

* <span data-ttu-id="98354-1218">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="98354-1218">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="98354-1219">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="98354-1219">Add support for incremental blob copy</span></span>
* <span data-ttu-id="98354-1220">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="98354-1220">Add support for large block blob upload</span></span>
* <span data-ttu-id="98354-1221">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="98354-1221">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="98354-1222">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-1222">VM</span></span>

* <span data-ttu-id="98354-1223">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="98354-1223">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="98354-1224">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="98354-1224">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="98354-1225">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="98354-1225">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="98354-1226">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="98354-1226">az vm/vmss disk</span></span>
  3. <span data-ttu-id="98354-1227">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="98354-1227">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="98354-1228">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="98354-1228">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="98354-1229">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="98354-1229">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="98354-1230">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-1230">April 3, 2017</span></span>

<span data-ttu-id="98354-1231">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="98354-1231">Version 2.0.2</span></span>

<span data-ttu-id="98354-1232">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="98354-1232">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="98354-1233">Núcleo</span><span class="sxs-lookup"><span data-stu-id="98354-1233">Core</span></span>

* <span data-ttu-id="98354-1234">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="98354-1234">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="98354-1235">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="98354-1235">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="98354-1236">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="98354-1236">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="98354-1237">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="98354-1237">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="98354-1238">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="98354-1238">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="98354-1239">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="98354-1239">Add prompting for missing template parameters.</span></span> <span data-ttu-id="98354-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="98354-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="98354-1241">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="98354-1241">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="98354-1242">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="98354-1242">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="98354-1243">ACS</span><span class="sxs-lookup"><span data-stu-id="98354-1243">ACS</span></span>

* <span data-ttu-id="98354-1244">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="98354-1244">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="98354-1245">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="98354-1245">Add support for ssh key password prompting.</span></span> <span data-ttu-id="98354-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="98354-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="98354-1247">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="98354-1247">Add support for windows clusters.</span></span> <span data-ttu-id="98354-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="98354-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="98354-1249">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="98354-1249">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="98354-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="98354-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="98354-1251">AppService</span><span class="sxs-lookup"><span data-stu-id="98354-1251">AppService</span></span>

* <span data-ttu-id="98354-1252">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="98354-1252">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="98354-1253">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="98354-1253">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="98354-1254">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="98354-1254">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="98354-1255">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="98354-1255">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="98354-1256">DataLake</span><span class="sxs-lookup"><span data-stu-id="98354-1256">DataLake</span></span>

* <span data-ttu-id="98354-1257">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="98354-1257">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="98354-1258">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="98354-1258">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="98354-1259">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="98354-1259">DocuemntDB</span></span>

* <span data-ttu-id="98354-1260">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="98354-1260">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="98354-1261">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="98354-1261">VM</span></span>

* <span data-ttu-id="98354-1262">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="98354-1262">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="98354-1263">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="98354-1263">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="98354-1264">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="98354-1264">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="98354-1265">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="98354-1265">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="98354-1266">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="98354-1266">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="98354-1267">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="98354-1267">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="98354-1268">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="98354-1268">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="98354-1269">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="98354-1269">February 27, 2017</span></span>

<span data-ttu-id="98354-1270">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="98354-1270">Version 2.0.0</span></span>

<span data-ttu-id="98354-1271">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="98354-1271">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="98354-1272">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="98354-1272">Container Service (acs)</span></span>
- <span data-ttu-id="98354-1273">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="98354-1273">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="98354-1274">Redes</span><span class="sxs-lookup"><span data-stu-id="98354-1274">Networking</span></span>
- <span data-ttu-id="98354-1275">Storage</span><span class="sxs-lookup"><span data-stu-id="98354-1275">Storage</span></span>

<span data-ttu-id="98354-1276">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="98354-1276">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="98354-1277">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="98354-1277">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="98354-1278">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="98354-1278">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="98354-1279">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="98354-1279">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="98354-1280">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="98354-1280">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="98354-1281">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="98354-1281">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="98354-1282">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="98354-1282">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="98354-1283">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="98354-1283">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="98354-1284">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="98354-1284">Provide feedback from the command line with the `az feedback` command</span></span>

