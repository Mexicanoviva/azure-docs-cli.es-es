---
title: "Notas de la versión de la CLI de Azure 2.0"
description: "Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0"
keywords: "CLI de Azure 2.0, notas de la versión"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 3bd4b9c059da3b841fc0757a11bc7ce78ec64b08
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.contentlocale: es-ES
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="8ded2-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="8ded2-104">Azure CLI 2.0 release notes</span></span>

## <a name="may-10-2017"></a><span data-ttu-id="8ded2-105">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="8ded2-105">May 10, 2017</span></span>

<span data-ttu-id="8ded2-106">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="8ded2-106">Version 2.0.6</span></span>

* <span data-ttu-id="8ded2-107">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="8ded2-107">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="8ded2-108">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="8ded2-108">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="8ded2-109">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8ded2-109">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="8ded2-110">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="8ded2-110">Include Cognitive Services module.</span></span>
* <span data-ttu-id="8ded2-111">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="8ded2-111">Include Service Fabric module.</span></span>
* <span data-ttu-id="8ded2-112">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="8ded2-112">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="8ded2-113">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="8ded2-113">Add support for CDN commands.</span></span>
* <span data-ttu-id="8ded2-114">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="8ded2-114">Remove Container module.</span></span>
* <span data-ttu-id="8ded2-115">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="8ded2-115">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="8ded2-116">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="8ded2-116">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="8ded2-117">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8ded2-117">Core</span></span>

* <span data-ttu-id="8ded2-118">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="8ded2-118">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="8ded2-119">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="8ded2-119">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="8ded2-120">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="8ded2-120">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="8ded2-121">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="8ded2-121">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="8ded2-122">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="8ded2-122">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="8ded2-123">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="8ded2-123">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="8ded2-124">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="8ded2-124">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="8ded2-125">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="8ded2-125">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="8ded2-126">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="8ded2-126">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="8ded2-127">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="8ded2-127">core: Improved performance</span></span>
* <span data-ttu-id="8ded2-128">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="8ded2-128">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="8ded2-129">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="8ded2-129">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="8ded2-130">ACS</span><span class="sxs-lookup"><span data-stu-id="8ded2-130">ACS</span></span>

* <span data-ttu-id="8ded2-131">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="8ded2-131">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="8ded2-132">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="8ded2-132">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="8ded2-133">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="8ded2-133">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="8ded2-134">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="8ded2-134">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="8ded2-135">AppService</span><span class="sxs-lookup"><span data-stu-id="8ded2-135">AppService</span></span>

* <span data-ttu-id="8ded2-136">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="8ded2-136">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="8ded2-137">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="8ded2-137">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="8ded2-138">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="8ded2-138">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="8ded2-139">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="8ded2-139">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="8ded2-140">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="8ded2-140">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="8ded2-141">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="8ded2-141">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="8ded2-142">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="8ded2-142">support slot swap with preview</span></span>
* <span data-ttu-id="8ded2-143">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="8ded2-143">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="8ded2-144">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="8ded2-144">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ded2-145">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ded2-145">CosmosDB</span></span>

* <span data-ttu-id="8ded2-146">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ded2-146">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="8ded2-147">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="8ded2-147">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="8ded2-148">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="8ded2-148">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="8ded2-149">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="8ded2-149">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8ded2-150">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8ded2-150">Data Lake Analytics</span></span>

* <span data-ttu-id="8ded2-151">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="8ded2-151">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="8ded2-152">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="8ded2-152">Add support for new catalog item type: package.</span></span> <span data-ttu-id="8ded2-153">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="8ded2-153">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="8ded2-154">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="8ded2-154">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="8ded2-155">Tabla</span><span class="sxs-lookup"><span data-stu-id="8ded2-155">Table</span></span>
  * <span data-ttu-id="8ded2-156">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="8ded2-156">Table valued function</span></span>
  * <span data-ttu-id="8ded2-157">Ver</span><span class="sxs-lookup"><span data-stu-id="8ded2-157">View</span></span>
  * <span data-ttu-id="8ded2-158">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="8ded2-158">Table Statistics.</span></span> <span data-ttu-id="8ded2-159">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="8ded2-159">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8ded2-160">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ded2-160">Data Lake Store</span></span>

* <span data-ttu-id="8ded2-161">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="8ded2-161">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="8ded2-162">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="8ded2-162">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="8ded2-163">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="8ded2-163">missed help for access show.</span></span> <span data-ttu-id="8ded2-164">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="8ded2-164">adding it.</span></span> <span data-ttu-id="8ded2-165">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="8ded2-165">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="8ded2-166">Buscar</span><span class="sxs-lookup"><span data-stu-id="8ded2-166">Find</span></span>

* <span data-ttu-id="8ded2-167">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="8ded2-167">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ded2-168">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ded2-168">KeyVault</span></span>

* <span data-ttu-id="8ded2-169">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="8ded2-169">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="8ded2-170">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="8ded2-170">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="8ded2-171">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="8ded2-171">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="8ded2-172">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="8ded2-172">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="8ded2-173">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="8ded2-173">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="8ded2-174">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="8ded2-174">Lab</span></span>

* <span data-ttu-id="8ded2-175">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="8ded2-175">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="8ded2-176">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="8ded2-176">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="8ded2-177">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="8ded2-177">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="8ded2-178">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="8ded2-178">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="8ded2-179">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="8ded2-179">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="8ded2-180">Supervisión</span><span class="sxs-lookup"><span data-stu-id="8ded2-180">Monitor</span></span>

* <span data-ttu-id="8ded2-181">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="8ded2-181">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="8ded2-182">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="8ded2-182">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="8ded2-183">Red</span><span class="sxs-lookup"><span data-stu-id="8ded2-183">Network</span></span>

* <span data-ttu-id="8ded2-184">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="8ded2-184">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="8ded2-185">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="8ded2-185">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="8ded2-186">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="8ded2-186">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="8ded2-187">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="8ded2-187">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="8ded2-188">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="8ded2-188">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="8ded2-189">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8ded2-189">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="8ded2-190">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="8ded2-190">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="8ded2-191">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="8ded2-191">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="8ded2-192">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="8ded2-192">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="8ded2-193">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="8ded2-193">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="8ded2-194">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="8ded2-194">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="8ded2-195">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="8ded2-195">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="8ded2-196">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="8ded2-196">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="8ded2-197">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="8ded2-197">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="8ded2-198">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="8ded2-198">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="8ded2-199">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="8ded2-199">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="8ded2-200">Perfil</span><span class="sxs-lookup"><span data-stu-id="8ded2-200">Profile</span></span>

* <span data-ttu-id="8ded2-201">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="8ded2-201">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="8ded2-202">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="8ded2-202">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="8ded2-203">Redis</span><span class="sxs-lookup"><span data-stu-id="8ded2-203">Redis</span></span>

* <span data-ttu-id="8ded2-204">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="8ded2-204">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="8ded2-205">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="8ded2-205">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="8ded2-206">Recurso</span><span class="sxs-lookup"><span data-stu-id="8ded2-206">Resource</span></span>

* <span data-ttu-id="8ded2-207">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="8ded2-207">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="8ded2-208">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="8ded2-208">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="8ded2-209">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="8ded2-209">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="8ded2-210">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="8ded2-210">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="8ded2-211">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="8ded2-211">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="8ded2-212">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="8ded2-212">Add docs for az lock update.</span></span> <span data-ttu-id="8ded2-213">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="8ded2-213">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="8ded2-214">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="8ded2-214">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="8ded2-215">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="8ded2-215">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="8ded2-216">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="8ded2-216">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="8ded2-217">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="8ded2-217">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="8ded2-218">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="8ded2-218">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="8ded2-219">Rol</span><span class="sxs-lookup"><span data-stu-id="8ded2-219">Role</span></span>

* <span data-ttu-id="8ded2-220">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="8ded2-220">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="8ded2-221">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="8ded2-221">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="8ded2-222">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="8ded2-222">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="8ded2-223">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="8ded2-223">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="8ded2-224">SQL</span><span class="sxs-lookup"><span data-stu-id="8ded2-224">SQL</span></span>

* <span data-ttu-id="8ded2-225">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="8ded2-225">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="8ded2-226">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="8ded2-226">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="8ded2-227">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="8ded2-227">Storage</span></span>

* <span data-ttu-id="8ded2-228">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="8ded2-228">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="8ded2-229">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="8ded2-229">Add support for incremental blob copy</span></span>
* <span data-ttu-id="8ded2-230">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="8ded2-230">Add support for large block blob upload</span></span>
* <span data-ttu-id="8ded2-231">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="8ded2-231">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="8ded2-232">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="8ded2-232">VM</span></span>

* <span data-ttu-id="8ded2-233">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="8ded2-233">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="8ded2-234">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="8ded2-234">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="8ded2-235">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="8ded2-235">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="8ded2-236">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="8ded2-236">az vm/vmss disk</span></span>
  3. <span data-ttu-id="8ded2-237">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="8ded2-237">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="8ded2-238">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="8ded2-238">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="8ded2-239">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="8ded2-239">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="8ded2-240">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="8ded2-240">April 3, 2017</span></span>

<span data-ttu-id="8ded2-241">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="8ded2-241">Version 2.0.2</span></span>

<span data-ttu-id="8ded2-242">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="8ded2-242">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="8ded2-243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8ded2-243">Core</span></span>

* <span data-ttu-id="8ded2-244">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="8ded2-244">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="8ded2-245">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="8ded2-245">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="8ded2-246">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="8ded2-246">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="8ded2-247">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="8ded2-247">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8ded2-248">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="8ded2-248">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="8ded2-249">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="8ded2-249">Add prompting for missing template parameters.</span></span> <span data-ttu-id="8ded2-250">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="8ded2-250">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="8ded2-251">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="8ded2-251">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="8ded2-252">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="8ded2-252">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="8ded2-253">ACS</span><span class="sxs-lookup"><span data-stu-id="8ded2-253">ACS</span></span>

* [<span data-ttu-id="8ded2-254">ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554</span><span class="sxs-lookup"><span data-stu-id="8ded2-254">ACS] Adding support for configuring a default ACS cluster ([#2554</span></span>](https://github.com/Azure/azure-cli/pull/2554))
* <span data-ttu-id="8ded2-255">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="8ded2-255">Add support for ssh key password prompting.</span></span> <span data-ttu-id="8ded2-256">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="8ded2-256">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="8ded2-257">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="8ded2-257">Add support for windows clusters.</span></span> <span data-ttu-id="8ded2-258">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="8ded2-258">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="8ded2-259">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="8ded2-259">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="8ded2-260">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="8ded2-260">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="8ded2-261">AppService</span><span class="sxs-lookup"><span data-stu-id="8ded2-261">AppService</span></span>

* <span data-ttu-id="8ded2-262">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="8ded2-262">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="8ded2-263">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="8ded2-263">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="8ded2-264">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="8ded2-264">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="8ded2-265">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="8ded2-265">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="8ded2-266">DataLake</span><span class="sxs-lookup"><span data-stu-id="8ded2-266">DataLake</span></span>

* <span data-ttu-id="8ded2-267">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="8ded2-267">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="8ded2-268">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8ded2-268">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="8ded2-269">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="8ded2-269">DocuemntDB</span></span>

* <span data-ttu-id="8ded2-270">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="8ded2-270">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="8ded2-271">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="8ded2-271">VM</span></span>

* [<span data-ttu-id="8ded2-272">Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570</span><span class="sxs-lookup"><span data-stu-id="8ded2-272">Compute] Add AppGateway support to virtual machine scale set create ([#2570</span></span>](https://github.com/Azure/azure-cli/pull/2570))
* [<span data-ttu-id="8ded2-273">VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522</span><span class="sxs-lookup"><span data-stu-id="8ded2-273">VM/VMSS] Improved disk caching support ([#2522</span></span>](https://github.com/Azure/azure-cli/pull/2522))
* <span data-ttu-id="8ded2-274">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="8ded2-274">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="8ded2-275">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="8ded2-275">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8ded2-276">Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="8ded2-276">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="8ded2-277">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="8ded2-277">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="8ded2-278">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="8ded2-278">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="8ded2-279">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="8ded2-279">February 27, 2017</span></span>

<span data-ttu-id="8ded2-280">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="8ded2-280">Version 2.0.0</span></span>

<span data-ttu-id="8ded2-281">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="8ded2-281">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="8ded2-282">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="8ded2-282">General availability applies to these command modules:</span></span>
- <span data-ttu-id="8ded2-283">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="8ded2-283">Container Service (acs)</span></span>
- <span data-ttu-id="8ded2-284">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="8ded2-284">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="8ded2-285">Redes</span><span class="sxs-lookup"><span data-stu-id="8ded2-285">Networking</span></span>
- <span data-ttu-id="8ded2-286">Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="8ded2-286">Storage</span></span>

<span data-ttu-id="8ded2-287">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8ded2-287">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="8ded2-288">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="8ded2-288">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="8ded2-289">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="8ded2-289">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
<span data-ttu-id="8ded2-290">Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8ded2-290">You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="8ded2-291">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="8ded2-291">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="8ded2-292">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="8ded2-292">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="8ded2-293">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="8ded2-293">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="8ded2-294">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="8ded2-294">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="8ded2-295">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="8ded2-295">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="8ded2-296">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="8ded2-296">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="8ded2-297">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="8ded2-297">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="8ded2-298">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="8ded2-298">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="8ded2-299">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="8ded2-299">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="8ded2-300">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="8ded2-300">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="8ded2-301">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8ded2-301">Provide feedback from the command line with the `az feedback` command.</span></span>

