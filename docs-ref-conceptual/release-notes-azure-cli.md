---
title: Notas de la versión de la CLI de Azure 2.0
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/01/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 57f13c7d17e2d248132e2e9c49bb0b4994f041f5
ms.sourcegitcommit: 80189ff103c91f8c47ab8ebf586df815fff5dd5d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2018
ms.locfileid: "34799267"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="614a8-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="614a8-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="614a8-104">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-104">June 5, 2018</span></span>

<span data-ttu-id="614a8-105">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="614a8-105">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="614a8-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-106">Core</span></span>

* <span data-ttu-id="614a8-107">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="614a8-107">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="614a8-108">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="614a8-108">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-109">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-109">ACR</span></span>

* <span data-ttu-id="614a8-110">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="614a8-110">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="614a8-111">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="614a8-111">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="614a8-112">AKS</span><span class="sxs-lookup"><span data-stu-id="614a8-112">AKS</span></span>

* <span data-ttu-id="614a8-113">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="614a8-113">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="614a8-114">Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-114">Batch</span></span>

* <span data-ttu-id="614a8-115">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="614a8-115">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="614a8-116">IoT</span><span class="sxs-lookup"><span data-stu-id="614a8-116">IOT</span></span>

* <span data-ttu-id="614a8-117">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="614a8-117">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="614a8-118">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-118">Network</span></span>

* <span data-ttu-id="614a8-119">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="614a8-119">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="614a8-120">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="614a8-120">Policy Insights</span></span>

* <span data-ttu-id="614a8-121">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="614a8-121">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="614a8-122">ARM</span><span class="sxs-lookup"><span data-stu-id="614a8-122">ARM</span></span>

* <span data-ttu-id="614a8-123">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="614a8-123">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-124">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-124">SQL</span></span>

* <span data-ttu-id="614a8-125">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="614a8-125">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="614a8-126">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="614a8-126">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="614a8-127">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-127">Storage</span></span>

* <span data-ttu-id="614a8-128">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="614a8-128">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-129">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-129">VM</span></span>

* <span data-ttu-id="614a8-130">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="614a8-130">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="614a8-131">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="614a8-131">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="614a8-132">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="614a8-132">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="614a8-133">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-133">May 22, 2018</span></span>

<span data-ttu-id="614a8-134">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="614a8-134">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="614a8-135">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-135">Core</span></span>

* <span data-ttu-id="614a8-136">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="614a8-136">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-137">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-137">ACS</span></span>

* <span data-ttu-id="614a8-138">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="614a8-138">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="614a8-139">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="614a8-139">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-140">AppService</span><span class="sxs-lookup"><span data-stu-id="614a8-140">AppService</span></span>

* <span data-ttu-id="614a8-141">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="614a8-141">Improved generic update commands</span></span>
* <span data-ttu-id="614a8-142">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="614a8-142">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="614a8-143">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-143">Container</span></span>

* <span data-ttu-id="614a8-144">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="614a8-144">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="614a8-145">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="614a8-145">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-146">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-146">Extension</span></span>

* <span data-ttu-id="614a8-147">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="614a8-147">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-148">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-148">Interactive</span></span>

* <span data-ttu-id="614a8-149">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="614a8-149">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="614a8-150">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="614a8-150">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="614a8-151">KeyVault</span><span class="sxs-lookup"><span data-stu-id="614a8-151">KeyVault</span></span>

* <span data-ttu-id="614a8-152">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="614a8-152">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="614a8-153">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-153">Network</span></span>

* <span data-ttu-id="614a8-154">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="614a8-154">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="614a8-155">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="614a8-155">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-156">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-156">SQL</span></span>

* <span data-ttu-id="614a8-157">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="614a8-157">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="614a8-158">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="614a8-158">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="614a8-159">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="614a8-159">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="614a8-160">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="614a8-160">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="614a8-161">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="614a8-161">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="614a8-162">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="614a8-162">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="614a8-163">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="614a8-163">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="614a8-164">`edition`.</span><span class="sxs-lookup"><span data-stu-id="614a8-164">`edition`.</span></span> <span data-ttu-id="614a8-165">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="614a8-165">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="614a8-166">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="614a8-166">`elasticPoolName`.</span></span> <span data-ttu-id="614a8-167">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="614a8-167">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="614a8-168">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="614a8-168">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="614a8-169">`edition`.</span><span class="sxs-lookup"><span data-stu-id="614a8-169">`edition`.</span></span> <span data-ttu-id="614a8-170">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="614a8-170">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="614a8-171">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="614a8-171">`dtu`.</span></span> <span data-ttu-id="614a8-172">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="614a8-172">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="614a8-173">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="614a8-173">`databaseDtuMin`.</span></span> <span data-ttu-id="614a8-174">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="614a8-174">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="614a8-175">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="614a8-175">`databaseDtuMax`.</span></span> <span data-ttu-id="614a8-176">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="614a8-176">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="614a8-177">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="614a8-177">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="614a8-178">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="614a8-178">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-179">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-179">Storage</span></span>

* <span data-ttu-id="614a8-180">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="614a8-180">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="614a8-181">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="614a8-181">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-182">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-182">VM</span></span>

* <span data-ttu-id="614a8-183">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-183">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="614a8-184">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="614a8-184">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="614a8-185">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="614a8-185">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="614a8-186">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="614a8-186">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="614a8-187">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="614a8-187">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="614a8-188">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-188">May 7, 2018</span></span>

<span data-ttu-id="614a8-189">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="614a8-189">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="614a8-190">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-190">Core</span></span>

* <span data-ttu-id="614a8-191">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="614a8-191">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="614a8-192">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="614a8-192">Added limited support for positional arguments</span></span>
* <span data-ttu-id="614a8-193">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="614a8-193">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="614a8-194">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="614a8-194">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="614a8-195">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="614a8-195">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="614a8-196">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="614a8-196">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="614a8-197">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-197">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="614a8-198">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="614a8-198">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="614a8-199">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-199">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-200">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-200">ACR</span></span>

* <span data-ttu-id="614a8-201">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="614a8-201">Added ACR Build commands</span></span>
* <span data-ttu-id="614a8-202">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="614a8-202">Improved resource not found error messages</span></span>
* <span data-ttu-id="614a8-203">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="614a8-203">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="614a8-204">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="614a8-204">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="614a8-205">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="614a8-205">Improved repository commands error messages</span></span>
* <span data-ttu-id="614a8-206">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="614a8-206">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-207">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-207">ACS</span></span>

* <span data-ttu-id="614a8-208">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="614a8-208">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="614a8-209">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="614a8-209">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="614a8-210">AMS</span><span class="sxs-lookup"><span data-stu-id="614a8-210">AMS</span></span>

* <span data-ttu-id="614a8-211">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="614a8-211">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-212">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-212">Appservice</span></span>

* <span data-ttu-id="614a8-213">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="614a8-213">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="614a8-214">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="614a8-214">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="614a8-215">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="614a8-215">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="614a8-216">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="614a8-216">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="614a8-217">Batch AI</span><span class="sxs-lookup"><span data-stu-id="614a8-217">Batch AI</span></span>

* <span data-ttu-id="614a8-218">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="614a8-218">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="614a8-219">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="614a8-219">Cognitive Services</span></span>

* <span data-ttu-id="614a8-220">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="614a8-220">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="614a8-221">Consumo</span><span class="sxs-lookup"><span data-stu-id="614a8-221">Consumption</span></span>

* <span data-ttu-id="614a8-222">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="614a8-222">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="614a8-223">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-223">Container</span></span>

* <span data-ttu-id="614a8-224">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="614a8-224">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="614a8-225">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="614a8-225">Cosmos DB</span></span>

* <span data-ttu-id="614a8-226">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="614a8-226">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="614a8-227">DMS</span><span class="sxs-lookup"><span data-stu-id="614a8-227">DMS</span></span>

* <span data-ttu-id="614a8-228">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-228">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-229">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-229">Extension</span></span>

* <span data-ttu-id="614a8-230">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="614a8-230">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-231">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-231">Interactive</span></span>

* <span data-ttu-id="614a8-232">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="614a8-232">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="614a8-233">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="614a8-233">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="614a8-234">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="614a8-234">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="614a8-235">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-235">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="614a8-236">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-236">Lab</span></span>

* <span data-ttu-id="614a8-237">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="614a8-237">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="614a8-238">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-238">Network</span></span>

* <span data-ttu-id="614a8-239">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="614a8-239">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="614a8-240">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-240">Profile</span></span>

* <span data-ttu-id="614a8-241">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="614a8-241">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="614a8-242">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="614a8-242">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="614a8-243">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="614a8-243">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="614a8-244">Redis</span><span class="sxs-lookup"><span data-stu-id="614a8-244">Redis</span></span>

* <span data-ttu-id="614a8-245">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="614a8-245">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="614a8-246">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="614a8-246">Deprecated `redis list-all`.</span></span> <span data-ttu-id="614a8-247">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="614a8-247">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="614a8-248">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="614a8-248">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="614a8-249">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-249">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="614a8-250">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-250">Role</span></span>

* <span data-ttu-id="614a8-251">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="614a8-251">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-252">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-252">Storage</span></span>

* <span data-ttu-id="614a8-253">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="614a8-253">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="614a8-254">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="614a8-254">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="614a8-255">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="614a8-255">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="614a8-256">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="614a8-256">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="614a8-257">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="614a8-257">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-258">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-258">VM</span></span>

* <span data-ttu-id="614a8-259">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="614a8-259">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="614a8-260">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="614a8-260">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="614a8-261">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="614a8-261">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="614a8-262">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="614a8-262">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="614a8-263">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="614a8-263">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="614a8-264">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="614a8-264">Added write accelerator support</span></span> 
* <span data-ttu-id="614a8-265">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="614a8-265">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="614a8-266">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="614a8-266">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="614a8-267">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="614a8-267">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="614a8-268">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-268">April 10, 2018</span></span>

<span data-ttu-id="614a8-269">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="614a8-269">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-270">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-270">ACR</span></span>

* <span data-ttu-id="614a8-271">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="614a8-271">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-272">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-272">ACS</span></span>

* <span data-ttu-id="614a8-273">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="614a8-273">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-274">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-274">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="614a8-276">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="614a8-276">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="614a8-277">BatchAI</span><span class="sxs-lookup"><span data-stu-id="614a8-277">BatchAI</span></span>

* <span data-ttu-id="614a8-278">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="614a8-278">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="614a8-279">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="614a8-279">Job level mounting</span></span>
 - <span data-ttu-id="614a8-280">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="614a8-280">Environment variables with secret values</span></span>
 - <span data-ttu-id="614a8-281">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="614a8-281">Performance counters settings</span></span>
 - <span data-ttu-id="614a8-282">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="614a8-282">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="614a8-283">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="614a8-283">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="614a8-284">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="614a8-284">Usage and limits reporting</span></span>
 - <span data-ttu-id="614a8-285">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="614a8-285">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="614a8-286">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="614a8-286">Support for custom images</span></span>
 - <span data-ttu-id="614a8-287">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="614a8-287">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="614a8-288">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="614a8-288">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="614a8-289">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="614a8-289">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="614a8-290">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="614a8-290">National clouds are supported</span></span>
* <span data-ttu-id="614a8-291">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="614a8-291">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="614a8-292">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="614a8-292">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="614a8-293">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="614a8-293">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="614a8-294">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="614a8-294">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="614a8-295">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="614a8-295">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="614a8-296">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="614a8-296">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="614a8-297">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="614a8-297">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="614a8-298">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="614a8-298">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="614a8-299">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="614a8-299">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="614a8-300">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="614a8-300">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="614a8-301">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-301">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="614a8-302">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="614a8-302">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="614a8-303">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="614a8-303">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="614a8-304">Facturación</span><span class="sxs-lookup"><span data-stu-id="614a8-304">Billing</span></span>

* <span data-ttu-id="614a8-305">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="614a8-305">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="614a8-306">Consumo</span><span class="sxs-lookup"><span data-stu-id="614a8-306">Consumption</span></span>

* <span data-ttu-id="614a8-307">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="614a8-307">Added `marketplace` commands</span></span>
* <span data-ttu-id="614a8-308">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="614a8-308">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="614a8-309">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="614a8-309">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="614a8-310">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="614a8-310">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="614a8-311">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="614a8-311">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="614a8-312">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="614a8-312">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="614a8-313">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-313">Container</span></span>

* <span data-ttu-id="614a8-314">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="614a8-314">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="614a8-315">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="614a8-315">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-316">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-316">Extension</span></span>

* <span data-ttu-id="614a8-317">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="614a8-317">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-318">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-318">Interactive</span></span>

* <span data-ttu-id="614a8-319">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="614a8-319">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="614a8-320">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-320">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="614a8-321">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="614a8-321">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="614a8-322">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-322">Network</span></span>

* <span data-ttu-id="614a8-323">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="614a8-323">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="614a8-324">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="614a8-324">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="614a8-325">4910</span><span class="sxs-lookup"><span data-stu-id="614a8-325">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="614a8-326">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="614a8-326">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="614a8-327">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="614a8-327">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="614a8-328">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-328">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="614a8-329">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-329">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="614a8-330">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="614a8-330">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-331">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-331">Profile</span></span>

* <span data-ttu-id="614a8-332">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="614a8-332">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="614a8-333">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="614a8-333">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="614a8-334">RDBMS</span><span class="sxs-lookup"><span data-stu-id="614a8-334">RDBMS</span></span>

* <span data-ttu-id="614a8-335">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="614a8-335">Added `georestore` command</span></span>
* <span data-ttu-id="614a8-336">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="614a8-336">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-337">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-337">Resource</span></span>

* <span data-ttu-id="614a8-338">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-338">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="614a8-339">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="614a8-339">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-340">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-340">SQL</span></span>

* <span data-ttu-id="614a8-341">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="614a8-341">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-342">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-342">Storage</span></span>

* <span data-ttu-id="614a8-343">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="614a8-343">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-344">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-344">VM</span></span>

* <span data-ttu-id="614a8-345">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="614a8-345">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="614a8-346">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="614a8-346">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="614a8-348">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="614a8-348">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="614a8-349">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="614a8-349">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="614a8-350">5718</span><span class="sxs-lookup"><span data-stu-id="614a8-350">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="614a8-351">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="614a8-351">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="614a8-352">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-352">March 27, 2018</span></span>

<span data-ttu-id="614a8-353">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="614a8-353">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="614a8-354">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-354">Core</span></span>

* <span data-ttu-id="614a8-355">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="614a8-355">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-356">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-356">ACS</span></span>

* <span data-ttu-id="614a8-357">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="614a8-357">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-358">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-358">Appservice</span></span>

* <span data-ttu-id="614a8-359">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="614a8-359">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="614a8-360">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="614a8-360">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="614a8-361">Backup</span><span class="sxs-lookup"><span data-stu-id="614a8-361">Backup</span></span>

* <span data-ttu-id="614a8-362">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="614a8-362">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="614a8-363">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-363">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="614a8-364">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="614a8-364">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="614a8-365">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="614a8-365">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="614a8-366">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-366">Container</span></span>

* <span data-ttu-id="614a8-367">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="614a8-367">Added `container exec` command.</span></span> <span data-ttu-id="614a8-368">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="614a8-368">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="614a8-369">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="614a8-369">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-370">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-370">Extension</span></span>

* <span data-ttu-id="614a8-371">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="614a8-371">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="614a8-372">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="614a8-372">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="614a8-373">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="614a8-373">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-374">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-374">Interactive</span></span>

* <span data-ttu-id="614a8-375">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-375">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="614a8-376">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="614a8-376">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="614a8-377">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-377">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="614a8-378">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="614a8-378">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="614a8-379">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-379">Lab</span></span>

* <span data-ttu-id="614a8-380">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="614a8-380">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-381">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-381">Monitor</span></span>

* <span data-ttu-id="614a8-382">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="614a8-382">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="614a8-383">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="614a8-383">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="614a8-384">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="614a8-384">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="614a8-385">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-385">Network</span></span>

* <span data-ttu-id="614a8-386">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="614a8-386">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-387">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-387">Profile</span></span>

* <span data-ttu-id="614a8-388">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="614a8-388">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="614a8-389">RDBMS</span><span class="sxs-lookup"><span data-stu-id="614a8-389">RDBMS</span></span>

* <span data-ttu-id="614a8-390">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="614a8-390">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-391">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-391">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="614a8-393">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-393">Role</span></span>

* <span data-ttu-id="614a8-394">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="614a8-394">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="614a8-395">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="614a8-395">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="614a8-396">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="614a8-396">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="614a8-397">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="614a8-397">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="614a8-398">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="614a8-398">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-399">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-399">Storage</span></span>

* <span data-ttu-id="614a8-400">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="614a8-400">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="614a8-401">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="614a8-401">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-402">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-402">VM</span></span>

* <span data-ttu-id="614a8-403">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="614a8-403">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="614a8-404">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="614a8-404">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="614a8-405">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="614a8-405">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="614a8-406">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="614a8-406">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="614a8-407">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-407">March 13, 2018</span></span>

<span data-ttu-id="614a8-408">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="614a8-408">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-409">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-409">ACR</span></span>

* <span data-ttu-id="614a8-410">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="614a8-410">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="614a8-411">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="614a8-411">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="614a8-412">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="614a8-412">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-413">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-413">ACS</span></span>

* <span data-ttu-id="614a8-414">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="614a8-414">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="614a8-415">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="614a8-415">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="614a8-416">Advisor</span><span class="sxs-lookup"><span data-stu-id="614a8-416">Advisor</span></span>

* <span data-ttu-id="614a8-417">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="614a8-417">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="614a8-418">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="614a8-418">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="614a8-419">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="614a8-419">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="614a8-420">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="614a8-420">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="614a8-421">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="614a8-421">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-422">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-422">Appservice</span></span>

* <span data-ttu-id="614a8-423">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="614a8-423">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="614a8-424">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="614a8-424">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="614a8-425">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="614a8-425">Eventhubs</span></span>

* <span data-ttu-id="614a8-426">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="614a8-426">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-427">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-427">Extension</span></span>

* <span data-ttu-id="614a8-428">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="614a8-428">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-429">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-429">Interactive</span></span>

* <span data-ttu-id="614a8-430">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="614a8-430">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="614a8-431">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="614a8-431">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="614a8-432">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="614a8-432">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="614a8-433">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="614a8-433">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-434">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-434">Monitor</span></span>

* <span data-ttu-id="614a8-435">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="614a8-435">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="614a8-436">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="614a8-436">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="614a8-437">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="614a8-437">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="614a8-438">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="614a8-438">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="614a8-439">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-439">Network</span></span>

* <span data-ttu-id="614a8-440">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="614a8-440">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="614a8-441">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="614a8-441">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="614a8-442">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="614a8-442">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="614a8-443">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="614a8-443">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-444">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-444">Profile</span></span>

* <span data-ttu-id="614a8-445">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="614a8-445">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="614a8-446">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="614a8-446">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="614a8-447">RDBMS</span><span class="sxs-lookup"><span data-stu-id="614a8-447">RDBMS</span></span>

* <span data-ttu-id="614a8-448">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="614a8-448">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="614a8-449">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="614a8-449">Service Bus</span></span>

* <span data-ttu-id="614a8-450">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="614a8-450">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-451">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-451">Storage</span></span>

* <span data-ttu-id="614a8-452">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="614a8-452">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="614a8-453">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="614a8-453">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-454">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-454">VM</span></span>

* <span data-ttu-id="614a8-455">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="614a8-455">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="614a8-456">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="614a8-456">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="614a8-457">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="614a8-457">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="614a8-458">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="614a8-458">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="614a8-459">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-459">February 27, 2018</span></span>

<span data-ttu-id="614a8-460">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="614a8-460">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="614a8-461">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-461">Core</span></span>

* <span data-ttu-id="614a8-462">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="614a8-462">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="614a8-463">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="614a8-463">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="614a8-464">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="614a8-464">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-465">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-465">ACS</span></span>

* <span data-ttu-id="614a8-466">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="614a8-466">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="614a8-467">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="614a8-467">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="614a8-468">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="614a8-468">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="614a8-469">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="614a8-469">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-470">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-470">Appservice</span></span>

* <span data-ttu-id="614a8-471">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="614a8-471">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="614a8-472">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="614a8-472">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="614a8-473">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="614a8-473">Cognitive Services</span></span>

* <span data-ttu-id="614a8-474">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="614a8-474">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="614a8-475">Consumo</span><span class="sxs-lookup"><span data-stu-id="614a8-475">Consumption</span></span>

* <span data-ttu-id="614a8-476">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="614a8-476">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="614a8-477">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="614a8-477">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="614a8-478">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-478">Container</span></span>

* <span data-ttu-id="614a8-479">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="614a8-479">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="614a8-480">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-480">Network</span></span>

* <span data-ttu-id="614a8-481">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="614a8-481">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-482">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-482">Resource</span></span>

* <span data-ttu-id="614a8-483">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="614a8-483">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="614a8-484">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-484">Role</span></span>

* <span data-ttu-id="614a8-485">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="614a8-485">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-486">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-486">SQL</span></span>

* <span data-ttu-id="614a8-487">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="614a8-487">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-488">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-488">Storage</span></span>

* <span data-ttu-id="614a8-489">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="614a8-489">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-490">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-490">VM</span></span>

* <span data-ttu-id="614a8-491">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="614a8-491">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="614a8-492">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-492">February 13, 2018</span></span>

<span data-ttu-id="614a8-493">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="614a8-493">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="614a8-494">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-494">Core</span></span>

* <span data-ttu-id="614a8-495">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="614a8-495">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-496">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-496">ACS</span></span>

* <span data-ttu-id="614a8-497">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="614a8-497">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="614a8-498">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="614a8-498">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="614a8-499">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="614a8-499">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="614a8-500">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="614a8-500">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="614a8-501">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="614a8-501">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="614a8-502">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="614a8-502">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="614a8-503">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="614a8-503">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="614a8-504">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="614a8-504">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-505">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-505">Appservice</span></span>

* <span data-ttu-id="614a8-506">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="614a8-506">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="614a8-507">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="614a8-507">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="614a8-508">CDN</span><span class="sxs-lookup"><span data-stu-id="614a8-508">CDN</span></span>

* <span data-ttu-id="614a8-509">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="614a8-509">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="614a8-510">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-510">Container</span></span>

* <span data-ttu-id="614a8-511">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="614a8-511">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="614a8-512">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="614a8-512">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="614a8-513">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="614a8-513">CosmosDB</span></span>

* <span data-ttu-id="614a8-514">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="614a8-514">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-515">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-515">Extension</span></span>

* <span data-ttu-id="614a8-516">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-516">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="614a8-517">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-517">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="614a8-518">Comentarios</span><span class="sxs-lookup"><span data-stu-id="614a8-518">Feedback</span></span>

* <span data-ttu-id="614a8-519">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="614a8-519">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-520">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-520">Interactive</span></span>

* <span data-ttu-id="614a8-521">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="614a8-521">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="614a8-522">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="614a8-522">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="614a8-523">IoT</span><span class="sxs-lookup"><span data-stu-id="614a8-523">IoT</span></span>

* <span data-ttu-id="614a8-524">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="614a8-524">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="614a8-525">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="614a8-525">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="614a8-526">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-526">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="614a8-527">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="614a8-527">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-528">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-528">Monitor</span></span>

* <span data-ttu-id="614a8-529">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="614a8-529">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="614a8-530">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-530">Network</span></span>

* <span data-ttu-id="614a8-531">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="614a8-531">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="614a8-532">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-532">Profile</span></span>

* <span data-ttu-id="614a8-533">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="614a8-533">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-534">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-534">Resource</span></span>

* <span data-ttu-id="614a8-535">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="614a8-535">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="614a8-536">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-536">Role</span></span>

* <span data-ttu-id="614a8-537">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="614a8-537">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-538">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-538">SQL</span></span>

* <span data-ttu-id="614a8-539">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="614a8-539">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="614a8-540">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="614a8-540">Added `sql db rename`</span></span>
* <span data-ttu-id="614a8-541">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="614a8-541">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-542">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-542">Storage</span></span>

* <span data-ttu-id="614a8-543">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="614a8-543">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-544">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-544">VM</span></span>

* <span data-ttu-id="614a8-545">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="614a8-545">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="614a8-546">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="614a8-546">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="614a8-547">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="614a8-547">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="614a8-548">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-548">January 31, 2018</span></span>

<span data-ttu-id="614a8-549">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="614a8-549">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="614a8-550">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-550">Core</span></span>

* <span data-ttu-id="614a8-551">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="614a8-551">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="614a8-552">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="614a8-552">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="614a8-553">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="614a8-553">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="614a8-554">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="614a8-554">Use `--verbose` to see</span></span>
* <span data-ttu-id="614a8-555">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="614a8-555">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-556">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-556">ACS</span></span>

* <span data-ttu-id="614a8-557">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="614a8-557">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="614a8-558">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="614a8-558">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-559">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-559">Appservice</span></span>

* <span data-ttu-id="614a8-560">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="614a8-560">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="614a8-561">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="614a8-561">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="614a8-562">CDN</span><span class="sxs-lookup"><span data-stu-id="614a8-562">CDN</span></span>

* <span data-ttu-id="614a8-563">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="614a8-563">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="614a8-564">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="614a8-564">CosmosDB</span></span>

* <span data-ttu-id="614a8-565">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="614a8-565">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-566">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-566">Interactive</span></span>

* <span data-ttu-id="614a8-567">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="614a8-567">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="614a8-568">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-568">Network</span></span>

* <span data-ttu-id="614a8-569">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="614a8-569">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="614a8-570">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="614a8-570">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="614a8-571">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="614a8-571">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="614a8-572">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="614a8-572">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="614a8-573">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="614a8-573">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="614a8-574">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="614a8-574">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="614a8-575">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="614a8-575">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="614a8-576">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="614a8-576">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="614a8-577">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="614a8-577">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="614a8-578">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="614a8-578">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-579">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-579">Profile</span></span>

* <span data-ttu-id="614a8-580">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="614a8-580">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-581">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-581">Resource</span></span>

* <span data-ttu-id="614a8-582">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="614a8-582">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-583">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-583">Storage</span></span>

* <span data-ttu-id="614a8-584">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="614a8-584">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="614a8-585">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="614a8-585">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="614a8-586">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="614a8-586">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="614a8-587">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="614a8-587">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="614a8-588">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="614a8-588">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-589">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-589">VM</span></span>

* <span data-ttu-id="614a8-590">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="614a8-590">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="614a8-591">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="614a8-591">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="614a8-592">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="614a8-592">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="614a8-593">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="614a8-593">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="614a8-594">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="614a8-594">January 17, 2018</span></span>

<span data-ttu-id="614a8-595">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="614a8-595">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-596">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-596">ACR</span></span>

* <span data-ttu-id="614a8-597">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="614a8-597">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="614a8-598">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="614a8-598">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-599">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-599">ACS</span></span>

* <span data-ttu-id="614a8-600">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="614a8-600">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="614a8-601">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="614a8-601">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-602">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-602">Appservice</span></span>

* <span data-ttu-id="614a8-603">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="614a8-603">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="614a8-604">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="614a8-604">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="614a8-605">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="614a8-605">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="614a8-606">Backup</span><span class="sxs-lookup"><span data-stu-id="614a8-606">Backup</span></span>

* <span data-ttu-id="614a8-607">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="614a8-607">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="614a8-608">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="614a8-608">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="614a8-609">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="614a8-609">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="614a8-610">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="614a8-610">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="614a8-611">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="614a8-611">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="614a8-612">Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-612">Batch</span></span>

* <span data-ttu-id="614a8-613">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="614a8-613">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="614a8-614">Nube</span><span class="sxs-lookup"><span data-stu-id="614a8-614">Cloud</span></span>

* <span data-ttu-id="614a8-615">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="614a8-615">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="614a8-616">Consumo</span><span class="sxs-lookup"><span data-stu-id="614a8-616">Consumption</span></span>

* <span data-ttu-id="614a8-617">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="614a8-617">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="614a8-618">Event Grid</span><span class="sxs-lookup"><span data-stu-id="614a8-618">Event Grid</span></span>

* <span data-ttu-id="614a8-619">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="614a8-619">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="614a8-620">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="614a8-620">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="614a8-621">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="614a8-621">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="614a8-622">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="614a8-622">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="614a8-623">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="614a8-623">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="614a8-624">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="614a8-624">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="614a8-625">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="614a8-625">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="614a8-626">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="614a8-626">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-627">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-627">Interactive</span></span>

* <span data-ttu-id="614a8-628">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="614a8-628">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="614a8-629">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="614a8-629">Fixed errors on startup</span></span>
* <span data-ttu-id="614a8-630">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="614a8-630">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="614a8-631">IoT</span><span class="sxs-lookup"><span data-stu-id="614a8-631">IoT</span></span>

* <span data-ttu-id="614a8-632">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="614a8-632">Added support for device provisioning service</span></span>
* <span data-ttu-id="614a8-633">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-633">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="614a8-634">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="614a8-634">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-635">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-635">Monitor</span></span>

* <span data-ttu-id="614a8-636">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="614a8-636">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="614a8-637">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="614a8-637">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="614a8-638">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="614a8-638">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="614a8-639">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-639">Network</span></span>

* <span data-ttu-id="614a8-640">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="614a8-640">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="614a8-641">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-641">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-642">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-642">Profile</span></span>

* <span data-ttu-id="614a8-643">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="614a8-643">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="614a8-644">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-644">Role</span></span>

* <span data-ttu-id="614a8-645">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="614a8-645">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="614a8-646">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="614a8-646">Service Fabric</span></span>

* <span data-ttu-id="614a8-647">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="614a8-647">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="614a8-648">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="614a8-648">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-649">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-649">VM</span></span>

* <span data-ttu-id="614a8-650">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="614a8-650">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="614a8-651">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="614a8-651">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="614a8-652">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="614a8-652">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="614a8-653">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="614a8-653">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="614a8-654">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="614a8-654">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="614a8-655">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="614a8-655">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="614a8-656">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="614a8-656">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="614a8-657">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="614a8-657">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="614a8-658">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-658">December 19, 2017</span></span>

<span data-ttu-id="614a8-659">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="614a8-659">Version 2.0.23</span></span>

* <span data-ttu-id="614a8-660">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="614a8-660">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="614a8-661">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-661">Container</span></span>

* <span data-ttu-id="614a8-662">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-662">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="614a8-663">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-663">Network</span></span>

* <span data-ttu-id="614a8-664">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-664">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="614a8-665">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-665">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-666">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-666">Storage</span></span>

* <span data-ttu-id="614a8-667">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="614a8-667">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-668">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-668">VM</span></span>

* <span data-ttu-id="614a8-669">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="614a8-669">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="614a8-670">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-670">December 5, 2017</span></span>

<span data-ttu-id="614a8-671">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="614a8-671">Version 2.0.22</span></span>

* <span data-ttu-id="614a8-672">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="614a8-672">Removed `az component` commands.</span></span> <span data-ttu-id="614a8-673">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="614a8-673">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="614a8-674">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-674">Core</span></span>
* <span data-ttu-id="614a8-675">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="614a8-675">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="614a8-676">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="614a8-676">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-677">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-677">ACS</span></span>

* <span data-ttu-id="614a8-678">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="614a8-678">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="614a8-679">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="614a8-679">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="614a8-680">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="614a8-680">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="614a8-681">Advisor</span><span class="sxs-lookup"><span data-stu-id="614a8-681">Advisor</span></span>

* <span data-ttu-id="614a8-682">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="614a8-682">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-683">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-683">Appservice</span></span>

* <span data-ttu-id="614a8-684">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="614a8-684">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="614a8-685">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="614a8-685">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="614a8-686">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="614a8-686">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="614a8-687">Consumo</span><span class="sxs-lookup"><span data-stu-id="614a8-687">Consumption</span></span>

* <span data-ttu-id="614a8-688">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="614a8-688">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="614a8-689">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-689">Container</span></span>

* <span data-ttu-id="614a8-690">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="614a8-690">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-691">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-691">Monitor</span></span>

* <span data-ttu-id="614a8-692">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="614a8-692">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-693">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-693">Resource</span></span>

* <span data-ttu-id="614a8-694">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="614a8-694">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="614a8-695">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-695">Role</span></span>

* <span data-ttu-id="614a8-696">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="614a8-696">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="614a8-697">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="614a8-697">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="614a8-698">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="614a8-698">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-699">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-699">SQL</span></span>

* <span data-ttu-id="614a8-700">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="614a8-700">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="614a8-701">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="614a8-701">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-702">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-702">VM</span></span>

* <span data-ttu-id="614a8-703">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="614a8-703">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="614a8-704">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-704">November 14, 2017</span></span>

<span data-ttu-id="614a8-705">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="614a8-705">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-706">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-706">ACR</span></span>

* <span data-ttu-id="614a8-707">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="614a8-707">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="614a8-708">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-708">ACS</span></span>

* <span data-ttu-id="614a8-709">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="614a8-709">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="614a8-710">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="614a8-710">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="614a8-711">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="614a8-711">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="614a8-712">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="614a8-712">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="614a8-713">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="614a8-713">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-714">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-714">Appservice</span></span>

* <span data-ttu-id="614a8-715">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="614a8-715">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="614a8-716">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="614a8-716">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="614a8-717">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="614a8-717">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="614a8-718">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="614a8-718">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="614a8-719">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="614a8-719">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="614a8-720">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="614a8-720">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="614a8-721">Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-721">Batch</span></span>

* <span data-ttu-id="614a8-722">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="614a8-722">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="614a8-723">Batchai</span><span class="sxs-lookup"><span data-stu-id="614a8-723">Batchai</span></span>

* <span data-ttu-id="614a8-724">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="614a8-724">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="614a8-725">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="614a8-725">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="614a8-726">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="614a8-726">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="614a8-727">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="614a8-727">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="614a8-728">Nube</span><span class="sxs-lookup"><span data-stu-id="614a8-728">Cloud</span></span>

* <span data-ttu-id="614a8-729">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="614a8-729">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="614a8-730">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-730">Container</span></span>

* <span data-ttu-id="614a8-731">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="614a8-731">Added support to open multiple ports</span></span>
* <span data-ttu-id="614a8-732">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="614a8-732">Added container group restart policy</span></span>
* <span data-ttu-id="614a8-733">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="614a8-733">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="614a8-734">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="614a8-734">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="614a8-735">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="614a8-735">Data Lake Analytics</span></span>

* <span data-ttu-id="614a8-736">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="614a8-736">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="614a8-737">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="614a8-737">Data Lake Store</span></span>

* <span data-ttu-id="614a8-738">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="614a8-738">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-739">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-739">Extension</span></span>

* <span data-ttu-id="614a8-740">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="614a8-740">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="614a8-741">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="614a8-741">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="614a8-742">IoT</span><span class="sxs-lookup"><span data-stu-id="614a8-742">IoT</span></span>

* <span data-ttu-id="614a8-743">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="614a8-743">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-744">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-744">Monitor</span></span>

* <span data-ttu-id="614a8-745">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="614a8-745">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="614a8-746">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-746">Network</span></span>

* <span data-ttu-id="614a8-747">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="614a8-747">Added support for CAA DNS records</span></span>
* <span data-ttu-id="614a8-748">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="614a8-748">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="614a8-749">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-749">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="614a8-750">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="614a8-750">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="614a8-751">Reservations</span><span class="sxs-lookup"><span data-stu-id="614a8-751">Reservations</span></span>

* <span data-ttu-id="614a8-752">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="614a8-752">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-753">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-753">Resource</span></span>

* <span data-ttu-id="614a8-754">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-754">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-755">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-755">SQL</span></span>

* <span data-ttu-id="614a8-756">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-756">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-757">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-757">Storage</span></span>

* <span data-ttu-id="614a8-758">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="614a8-758">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="614a8-759">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="614a8-759">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="614a8-760">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="614a8-760">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="614a8-761">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="614a8-761">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="614a8-762">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="614a8-762">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="614a8-763">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="614a8-763">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="614a8-764">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="614a8-764">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-765">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-765">VM</span></span>

* <span data-ttu-id="614a8-766">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="614a8-766">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="614a8-767">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="614a8-767">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="614a8-768">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="614a8-768">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="614a8-769">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="614a8-769">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="614a8-770">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="614a8-770">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="614a8-771">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-771">October 24, 2017</span></span>

<span data-ttu-id="614a8-772">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="614a8-772">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="614a8-773">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-773">Core</span></span>

* <span data-ttu-id="614a8-774">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="614a8-774">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-775">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-775">ACR</span></span>

* <span data-ttu-id="614a8-776">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="614a8-776">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="614a8-777">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="614a8-777">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="614a8-778">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="614a8-778">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-779">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-779">ACS</span></span>

* <span data-ttu-id="614a8-780">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="614a8-780">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="614a8-781">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="614a8-781">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-782">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-782">Appservice</span></span>

* <span data-ttu-id="614a8-783">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="614a8-783">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="614a8-784">Componente</span><span class="sxs-lookup"><span data-stu-id="614a8-784">Component</span></span>

* <span data-ttu-id="614a8-785">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="614a8-785">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-786">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-786">Monitor</span></span>

* <span data-ttu-id="614a8-787">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="614a8-787">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-788">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-788">Resource</span></span>

* <span data-ttu-id="614a8-789">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="614a8-789">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="614a8-790">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="614a8-790">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-791">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-791">VM</span></span>

* <span data-ttu-id="614a8-792">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="614a8-792">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="614a8-793">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-793">October 9, 2017</span></span>

<span data-ttu-id="614a8-794">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="614a8-794">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="614a8-795">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-795">Core</span></span>

* <span data-ttu-id="614a8-796">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="614a8-796">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-797">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-797">Appservice</span></span>

* <span data-ttu-id="614a8-798">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="614a8-798">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="614a8-799">Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-799">Batch</span></span>

* <span data-ttu-id="614a8-800">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="614a8-800">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="614a8-801">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="614a8-801">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="614a8-802">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-802">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="614a8-803">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="614a8-803">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="614a8-804">Batchai</span><span class="sxs-lookup"><span data-stu-id="614a8-804">Batchai</span></span>

* <span data-ttu-id="614a8-805">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-805">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="614a8-806">Keyvault</span><span class="sxs-lookup"><span data-stu-id="614a8-806">Keyvault</span></span>

* <span data-ttu-id="614a8-807">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="614a8-807">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="614a8-808">(#4448)</span><span class="sxs-lookup"><span data-stu-id="614a8-808">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="614a8-809">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-809">Network</span></span>

* <span data-ttu-id="614a8-810">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="614a8-810">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="614a8-811">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="614a8-811">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-812">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-812">Resource</span></span>

* <span data-ttu-id="614a8-813">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-813">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="614a8-814">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="614a8-814">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="614a8-815">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="614a8-815">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="614a8-816">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-816">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-817">Sql</span><span class="sxs-lookup"><span data-stu-id="614a8-817">Sql</span></span>

* <span data-ttu-id="614a8-818">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="614a8-818">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="614a8-819">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="614a8-819">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="614a8-820">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="614a8-820">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-821">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-821">Storage</span></span>

* <span data-ttu-id="614a8-822">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="614a8-822">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-823">Vm</span><span class="sxs-lookup"><span data-stu-id="614a8-823">Vm</span></span>

* <span data-ttu-id="614a8-824">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="614a8-824">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="614a8-825">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="614a8-825">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="614a8-826">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="614a8-826">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="614a8-827">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="614a8-827">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="614a8-828">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="614a8-828">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="614a8-829">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-829">September 22, 2017</span></span>

<span data-ttu-id="614a8-830">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="614a8-830">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-831">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-831">Resource</span></span>

* <span data-ttu-id="614a8-832">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="614a8-832">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="614a8-833">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="614a8-833">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="614a8-834">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="614a8-834">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="614a8-835">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="614a8-835">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="614a8-836">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-836">Network</span></span>

* <span data-ttu-id="614a8-837">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="614a8-837">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="614a8-838">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="614a8-838">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="614a8-839">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="614a8-839">Added `asg` application security group commands</span></span>
* <span data-ttu-id="614a8-840">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-840">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="614a8-841">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-841">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="614a8-842">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-842">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="614a8-843">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="614a8-843">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-844">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-844">Storage</span></span>

* <span data-ttu-id="614a8-845">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="614a8-845">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="614a8-846">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="614a8-846">Eventgrid</span></span>

* <span data-ttu-id="614a8-847">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="614a8-847">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-848">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-848">SQL</span></span>

* <span data-ttu-id="614a8-849">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="614a8-849">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="614a8-850">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="614a8-850">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="614a8-851">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-851">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="614a8-852">Keyvault</span><span class="sxs-lookup"><span data-stu-id="614a8-852">Keyvault</span></span>

* <span data-ttu-id="614a8-853">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="614a8-853">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-854">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-854">VM</span></span>

* <span data-ttu-id="614a8-855">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="614a8-855">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="614a8-856">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="614a8-856">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="614a8-857">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="614a8-857">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="614a8-858">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="614a8-858">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="614a8-859">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="614a8-859">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="614a8-860">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="614a8-860">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-861">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-861">ACS</span></span>

* <span data-ttu-id="614a8-862">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-862">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-863">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-863">Appservice</span></span>

* <span data-ttu-id="614a8-864">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="614a8-864">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="614a8-865">Backup</span><span class="sxs-lookup"><span data-stu-id="614a8-865">Backup</span></span>

* <span data-ttu-id="614a8-866">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="614a8-866">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="614a8-867">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-867">September 11, 2017</span></span>

<span data-ttu-id="614a8-868">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="614a8-868">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="614a8-869">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-869">Core</span></span>

* <span data-ttu-id="614a8-870">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="614a8-870">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="614a8-871">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="614a8-871">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-872">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-872">Acs</span></span>

* <span data-ttu-id="614a8-873">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="614a8-873">Added `acs list-locations` command</span></span>
* <span data-ttu-id="614a8-874">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="614a8-874">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-875">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-875">Appservice</span></span>

* <span data-ttu-id="614a8-876">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="614a8-876">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="614a8-877">CDN</span><span class="sxs-lookup"><span data-stu-id="614a8-877">CDN</span></span>

* <span data-ttu-id="614a8-878">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="614a8-878">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="614a8-879">Extensión</span><span class="sxs-lookup"><span data-stu-id="614a8-879">Extension</span></span>

* <span data-ttu-id="614a8-880">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="614a8-880">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="614a8-881">Keyvault</span><span class="sxs-lookup"><span data-stu-id="614a8-881">Keyvault</span></span>

* <span data-ttu-id="614a8-882">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="614a8-882">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="614a8-883">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-883">Network</span></span>

* <span data-ttu-id="614a8-884">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="614a8-884">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="614a8-885">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-885">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="614a8-886">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-886">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="614a8-887">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-887">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="614a8-888">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-888">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-889">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-889">Resource</span></span>

* <span data-ttu-id="614a8-890">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-890">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="614a8-891">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-891">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="614a8-892">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="614a8-892">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="614a8-893">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="614a8-893">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-894">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-894">SQL</span></span>

* <span data-ttu-id="614a8-895">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="614a8-895">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-896">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-896">VM</span></span>

* <span data-ttu-id="614a8-897">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="614a8-897">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="614a8-898">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="614a8-898">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="614a8-899">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-899">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="614a8-900">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="614a8-900">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="614a8-901">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="614a8-901">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="614a8-902">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-902">August 31, 2017</span></span>

<span data-ttu-id="614a8-903">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="614a8-903">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="614a8-904">Keyvault</span><span class="sxs-lookup"><span data-stu-id="614a8-904">Keyvault</span></span>

* <span data-ttu-id="614a8-905">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="614a8-905">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="614a8-906">Sf</span><span class="sxs-lookup"><span data-stu-id="614a8-906">Sf</span></span>

* <span data-ttu-id="614a8-907">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="614a8-907">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-908">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-908">Storage</span></span>

* <span data-ttu-id="614a8-909">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="614a8-909">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="614a8-910">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="614a8-910">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="614a8-911">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-911">August 28, 2017</span></span>

<span data-ttu-id="614a8-912">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="614a8-912">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="614a8-913">CLI</span><span class="sxs-lookup"><span data-stu-id="614a8-913">CLI</span></span>

* <span data-ttu-id="614a8-914">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="614a8-914">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-915">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-915">ACS</span></span>

* <span data-ttu-id="614a8-916">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="614a8-916">Corrected preview regions</span></span>
* <span data-ttu-id="614a8-917">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="614a8-917">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="614a8-918">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="614a8-918">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-919">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-919">Appservice</span></span>

* <span data-ttu-id="614a8-920">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="614a8-920">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="614a8-921">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="614a8-921">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="614a8-922">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="614a8-922">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="614a8-923">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="614a8-923">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="614a8-924">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="614a8-924">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="614a8-925">IoT</span><span class="sxs-lookup"><span data-stu-id="614a8-925">IoT</span></span>

* <span data-ttu-id="614a8-926">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="614a8-926">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="614a8-927">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-927">Network</span></span>

* <span data-ttu-id="614a8-928">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="614a8-928">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="614a8-929">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="614a8-929">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="614a8-930">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="614a8-930">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="614a8-931">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-931">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="614a8-932">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-932">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-933">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-933">Profile</span></span>

* <span data-ttu-id="614a8-934">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="614a8-934">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="614a8-935">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="614a8-935">Service Fabric</span></span>

* <span data-ttu-id="614a8-936">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="614a8-936">Preview release</span></span>
* <span data-ttu-id="614a8-937">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="614a8-937">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="614a8-938">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="614a8-938">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="614a8-939">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="614a8-939">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-940">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-940">Storage</span></span>

* <span data-ttu-id="614a8-941">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="614a8-941">Enabled setting blob tier</span></span>
* <span data-ttu-id="614a8-942">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="614a8-942">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="614a8-943">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="614a8-943">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="614a8-944">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="614a8-944">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="614a8-945">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="614a8-945">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="614a8-946">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="614a8-946">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-947">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-947">VM</span></span>

* <span data-ttu-id="614a8-948">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="614a8-948">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="614a8-949">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-949">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="614a8-950">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-950">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="614a8-951">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="614a8-951">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="614a8-952">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="614a8-952">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="614a8-953">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-953">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="614a8-954">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-954">August 15, 2017</span></span>

<span data-ttu-id="614a8-955">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="614a8-955">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-956">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-956">ACS</span></span>

* <span data-ttu-id="614a8-957">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="614a8-957">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-958">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-958">Appservice</span></span>

* <span data-ttu-id="614a8-959">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="614a8-959">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="614a8-960">Event Grid</span><span class="sxs-lookup"><span data-stu-id="614a8-960">Event Grid</span></span>

* <span data-ttu-id="614a8-961">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="614a8-961">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="614a8-962">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-962">August 11, 2017</span></span>

<span data-ttu-id="614a8-963">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="614a8-963">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-964">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-964">ACS</span></span>

* <span data-ttu-id="614a8-965">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="614a8-965">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="614a8-966">Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-966">Batch</span></span>

* <span data-ttu-id="614a8-967">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="614a8-967">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="614a8-968">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="614a8-968">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="614a8-969">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="614a8-969">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="614a8-970">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="614a8-970">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="614a8-971">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="614a8-971">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="614a8-972">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="614a8-972">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="614a8-973">Componente</span><span class="sxs-lookup"><span data-stu-id="614a8-973">Component</span></span>

* <span data-ttu-id="614a8-974">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="614a8-974">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="614a8-975">Contenedor</span><span class="sxs-lookup"><span data-stu-id="614a8-975">Container</span></span>

* <span data-ttu-id="614a8-976">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="614a8-976">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="614a8-977">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="614a8-977">Data Lake Store</span></span>

* <span data-ttu-id="614a8-978">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="614a8-978">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="614a8-979">Event Grid</span><span class="sxs-lookup"><span data-stu-id="614a8-979">Event Grid</span></span>

* <span data-ttu-id="614a8-980">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="614a8-980">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="614a8-981">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-981">Network</span></span>

* <span data-ttu-id="614a8-982">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="614a8-982">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="614a8-983">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="614a8-983">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="614a8-984">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="614a8-984">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="614a8-985">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="614a8-985">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-986">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-986">Profile</span></span>

* <span data-ttu-id="614a8-987">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="614a8-987">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-988">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-988">Storage</span></span>

* <span data-ttu-id="614a8-989">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="614a8-989">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-990">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-990">VM</span></span>

* <span data-ttu-id="614a8-991">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="614a8-991">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="614a8-992">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="614a8-992">Exposed `list-skus` command</span></span>
* <span data-ttu-id="614a8-993">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="614a8-993">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="614a8-994">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="614a8-994">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="614a8-995">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="614a8-995">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="614a8-996">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-996">July 28, 2017</span></span>

<span data-ttu-id="614a8-997">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="614a8-997">Version 2.0.12</span></span>

* <span data-ttu-id="614a8-998">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="614a8-998">Added container commands</span></span>
* <span data-ttu-id="614a8-999">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="614a8-999">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="614a8-1000">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-1000">Core</span></span>

* <span data-ttu-id="614a8-1001">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="614a8-1001">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="614a8-1002">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="614a8-1002">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="614a8-1003">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="614a8-1003">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="614a8-1004">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="614a8-1004">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="614a8-1005">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="614a8-1005">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="614a8-1006">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="614a8-1006">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="614a8-1007">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="614a8-1007">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="614a8-1008">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="614a8-1008">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="614a8-1009">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="614a8-1009">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="614a8-1010">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="614a8-1010">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="614a8-1011">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="614a8-1011">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="614a8-1012">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="614a8-1012">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="614a8-1013">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="614a8-1013">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="614a8-1014">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="614a8-1014">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="614a8-1015">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="614a8-1015">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="614a8-1016">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="614a8-1016">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="614a8-1017">ACR</span><span class="sxs-lookup"><span data-stu-id="614a8-1017">ACR</span></span>

* <span data-ttu-id="614a8-1018">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="614a8-1018">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="614a8-1019">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="614a8-1019">Support SKU update for managed registries</span></span>
* <span data-ttu-id="614a8-1020">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="614a8-1020">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="614a8-1021">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="614a8-1021">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="614a8-1022">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="614a8-1022">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="614a8-1023">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="614a8-1023">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-1024">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-1024">ACS</span></span>

* <span data-ttu-id="614a8-1025">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="614a8-1025">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-1026">Appservice</span><span class="sxs-lookup"><span data-stu-id="614a8-1026">Appservice</span></span>

* <span data-ttu-id="614a8-1027">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="614a8-1027">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="614a8-1028">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="614a8-1028">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="614a8-1029">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1029">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="614a8-1030">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="614a8-1030">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="614a8-1031">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="614a8-1031">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="614a8-1032">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="614a8-1032">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="614a8-1033">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="614a8-1033">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="614a8-1034">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="614a8-1034">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="614a8-1035">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="614a8-1035">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="614a8-1036">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="614a8-1036">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="614a8-1037">Batch</span><span class="sxs-lookup"><span data-stu-id="614a8-1037">Batch</span></span>

* <span data-ttu-id="614a8-1038">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="614a8-1038">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="614a8-1039">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1039">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="614a8-1040">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1040">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="614a8-1041">CDN</span><span class="sxs-lookup"><span data-stu-id="614a8-1041">CDN</span></span>

* <span data-ttu-id="614a8-1042">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="614a8-1042">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="614a8-1043">Nube</span><span class="sxs-lookup"><span data-stu-id="614a8-1043">Cloud</span></span>

* <span data-ttu-id="614a8-1044">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="614a8-1044">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="614a8-1045">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="614a8-1045">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="614a8-1046">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="614a8-1046">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="614a8-1047">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="614a8-1047">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="614a8-1048">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1048">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="614a8-1049">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="614a8-1049">CosmosDB</span></span>

* <span data-ttu-id="614a8-1050">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="614a8-1050">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="614a8-1051">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="614a8-1051">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="614a8-1052">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="614a8-1052">Data Lake Analytics</span></span>

* <span data-ttu-id="614a8-1053">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1053">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="614a8-1054">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1054">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="614a8-1055">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1055">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="614a8-1056">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="614a8-1056">Data Lake Store</span></span>

* <span data-ttu-id="614a8-1057">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1057">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="614a8-1058">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="614a8-1058">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="614a8-1059">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1059">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="614a8-1060">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="614a8-1060">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="614a8-1061">Interactive</span><span class="sxs-lookup"><span data-stu-id="614a8-1061">Interactive</span></span>

* <span data-ttu-id="614a8-1062">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="614a8-1062">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="614a8-1063">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="614a8-1063">Increased test coverage</span></span>
* <span data-ttu-id="614a8-1064">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="614a8-1064">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="614a8-1065">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="614a8-1065">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="614a8-1066">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="614a8-1066">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="614a8-1067">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="614a8-1067">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="614a8-1068">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="614a8-1068">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="614a8-1069">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1069">Added `--progress` flag</span></span>
* <span data-ttu-id="614a8-1070">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="614a8-1070">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="614a8-1071">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="614a8-1071">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="614a8-1072">IoT</span><span class="sxs-lookup"><span data-stu-id="614a8-1072">IoT</span></span>

* <span data-ttu-id="614a8-1073">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="614a8-1073">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="614a8-1074">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="614a8-1074">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="614a8-1075">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="614a8-1075">Key vault</span></span>

* <span data-ttu-id="614a8-1076">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="614a8-1076">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="614a8-1077">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="614a8-1077">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="614a8-1078">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="614a8-1078">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="614a8-1079">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="614a8-1079">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="614a8-1080">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="614a8-1080">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="614a8-1081">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="614a8-1081">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="614a8-1082">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="614a8-1082">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="614a8-1083">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="614a8-1083">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="614a8-1084">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-1084">Lab</span></span>

* <span data-ttu-id="614a8-1085">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1085">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="614a8-1086">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1086">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-1087">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-1087">Monitor</span></span>

* <span data-ttu-id="614a8-1088">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="614a8-1088">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="614a8-1089">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1089">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="614a8-1090">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1090">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="614a8-1091">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1091">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="614a8-1092">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1092">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="614a8-1093">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="614a8-1093">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="614a8-1094">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="614a8-1094">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="614a8-1095">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="614a8-1095">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="614a8-1096">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="614a8-1096">`location` no longer required</span></span>
  * <span data-ttu-id="614a8-1097">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="614a8-1097">Add name and ID support for target</span></span>
  * <span data-ttu-id="614a8-1098">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1098">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="614a8-1099">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="614a8-1099">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="614a8-1100">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="614a8-1100">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="614a8-1101">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="614a8-1101">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="614a8-1102">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1102">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="614a8-1103">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="614a8-1103">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="614a8-1104">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-1104">Network</span></span>

* <span data-ttu-id="614a8-1105">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1105">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="614a8-1106">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1106">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="614a8-1107">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="614a8-1107">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="614a8-1108">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="614a8-1108">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="614a8-1109">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1109">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="614a8-1110">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1110">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="614a8-1111">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="614a8-1111">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="614a8-1112">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="614a8-1112">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="614a8-1113">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="614a8-1113">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="614a8-1114">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="614a8-1114">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="614a8-1115">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="614a8-1115">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="614a8-1116">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1116">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="614a8-1117">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="614a8-1117">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="614a8-1118">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1118">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="614a8-1119">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1119">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="614a8-1120">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1120">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="614a8-1121">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="614a8-1121">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="614a8-1122">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1122">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="614a8-1123">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1123">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="614a8-1124">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1124">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="614a8-1125">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1125">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="614a8-1126">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1126">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="614a8-1127">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1127">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="614a8-1128">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="614a8-1128">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="614a8-1129">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="614a8-1129">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="614a8-1130">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="614a8-1130">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="614a8-1131">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="614a8-1131">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-1132">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-1132">Profile</span></span>

* <span data-ttu-id="614a8-1133">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="614a8-1133">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="614a8-1134">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="614a8-1134">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="614a8-1135">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="614a8-1135">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="614a8-1136">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="614a8-1136">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="614a8-1137">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="614a8-1137">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="614a8-1138">RDBMS</span><span class="sxs-lookup"><span data-stu-id="614a8-1138">RDBMS</span></span>

* <span data-ttu-id="614a8-1139">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="614a8-1139">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="614a8-1140">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="614a8-1140">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="614a8-1141">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="614a8-1141">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="614a8-1142">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="614a8-1142">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-1143">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-1143">Resource</span></span>

* <span data-ttu-id="614a8-1144">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1144">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="614a8-1145">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1145">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="614a8-1146">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1146">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="614a8-1147">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1147">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="614a8-1148">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="614a8-1148">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="614a8-1149">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1149">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="614a8-1150">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="614a8-1150">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="614a8-1151">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1151">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="614a8-1152">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-1152">Role</span></span>

* <span data-ttu-id="614a8-1153">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="614a8-1153">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="614a8-1154">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="614a8-1154">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="614a8-1155">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1155">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="614a8-1156">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1156">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="614a8-1157">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1157">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="614a8-1158">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="614a8-1158">Service Fabric</span></span>
* <span data-ttu-id="614a8-1159">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="614a8-1159">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="614a8-1160">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="614a8-1160">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="614a8-1161">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="614a8-1161">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-1162">SQL</span></span>

* <span data-ttu-id="614a8-1163">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="614a8-1163">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="614a8-1164">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1164">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="614a8-1165">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="614a8-1165">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-1166">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-1166">Storage</span></span>

* <span data-ttu-id="614a8-1167">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="614a8-1167">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="614a8-1168">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="614a8-1168">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="614a8-1169">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="614a8-1169">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="614a8-1170">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="614a8-1170">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="614a8-1171">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="614a8-1171">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="614a8-1172">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="614a8-1172">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-1173">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-1173">VM</span></span>

* <span data-ttu-id="614a8-1174">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="614a8-1174">Support configuring nsg</span></span>
* <span data-ttu-id="614a8-1175">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="614a8-1175">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="614a8-1176">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="614a8-1176">Support managed service identities</span></span>
* <span data-ttu-id="614a8-1177">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="614a8-1177">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="614a8-1178">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="614a8-1178">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="614a8-1179">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-1179">May 10, 2017</span></span>

<span data-ttu-id="614a8-1180">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="614a8-1180">Version 2.0.6</span></span>

* <span data-ttu-id="614a8-1181">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="614a8-1181">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="614a8-1182">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="614a8-1182">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="614a8-1183">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="614a8-1183">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="614a8-1184">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="614a8-1184">Include Cognitive Services module</span></span>
* <span data-ttu-id="614a8-1185">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="614a8-1185">Include Service Fabric module</span></span>
* <span data-ttu-id="614a8-1186">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="614a8-1186">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="614a8-1187">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="614a8-1187">Add support for CDN commands</span></span>
* <span data-ttu-id="614a8-1188">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="614a8-1188">Remove Container module</span></span>
* <span data-ttu-id="614a8-1189">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="614a8-1189">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="614a8-1190">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="614a8-1190">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="614a8-1191">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-1191">Core</span></span>

* <span data-ttu-id="614a8-1192">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="614a8-1192">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="614a8-1193">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="614a8-1193">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="614a8-1194">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="614a8-1194">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="614a8-1195">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="614a8-1195">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="614a8-1196">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="614a8-1196">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="614a8-1197">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="614a8-1197">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="614a8-1198">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="614a8-1198">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="614a8-1199">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="614a8-1199">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="614a8-1200">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="614a8-1200">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="614a8-1201">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="614a8-1201">core: Improved performance</span></span>
* <span data-ttu-id="614a8-1202">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="614a8-1202">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="614a8-1203">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="614a8-1203">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-1204">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-1204">ACS</span></span>

* <span data-ttu-id="614a8-1205">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="614a8-1205">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="614a8-1206">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="614a8-1206">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="614a8-1207">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="614a8-1207">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="614a8-1208">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="614a8-1208">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-1209">AppService</span><span class="sxs-lookup"><span data-stu-id="614a8-1209">AppService</span></span>

* <span data-ttu-id="614a8-1210">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="614a8-1210">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="614a8-1211">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="614a8-1211">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="614a8-1212">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="614a8-1212">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="614a8-1213">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="614a8-1213">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="614a8-1214">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="614a8-1214">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="614a8-1215">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="614a8-1215">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="614a8-1216">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="614a8-1216">support slot swap with preview</span></span>
* <span data-ttu-id="614a8-1217">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="614a8-1217">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="614a8-1218">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="614a8-1218">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="614a8-1219">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="614a8-1219">CosmosDB</span></span>

* <span data-ttu-id="614a8-1220">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="614a8-1220">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="614a8-1221">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="614a8-1221">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="614a8-1222">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="614a8-1222">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="614a8-1223">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="614a8-1223">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="614a8-1224">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="614a8-1224">Data Lake Analytics</span></span>

* <span data-ttu-id="614a8-1225">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="614a8-1225">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="614a8-1226">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="614a8-1226">Add support for new catalog item type: package.</span></span> <span data-ttu-id="614a8-1227">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="614a8-1227">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="614a8-1228">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="614a8-1228">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="614a8-1229">Tabla</span><span class="sxs-lookup"><span data-stu-id="614a8-1229">Table</span></span>
  * <span data-ttu-id="614a8-1230">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="614a8-1230">Table valued function</span></span>
  * <span data-ttu-id="614a8-1231">Ver</span><span class="sxs-lookup"><span data-stu-id="614a8-1231">View</span></span>
  * <span data-ttu-id="614a8-1232">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="614a8-1232">Table Statistics.</span></span> <span data-ttu-id="614a8-1233">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="614a8-1233">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="614a8-1234">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="614a8-1234">Data Lake Store</span></span>

* <span data-ttu-id="614a8-1235">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="614a8-1235">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="614a8-1236">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="614a8-1236">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="614a8-1237">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="614a8-1237">missed help for access show.</span></span> <span data-ttu-id="614a8-1238">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="614a8-1238">adding it.</span></span> <span data-ttu-id="614a8-1239">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="614a8-1239">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="614a8-1240">Buscar</span><span class="sxs-lookup"><span data-stu-id="614a8-1240">Find</span></span>

* <span data-ttu-id="614a8-1241">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="614a8-1241">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="614a8-1242">KeyVault</span><span class="sxs-lookup"><span data-stu-id="614a8-1242">KeyVault</span></span>

* <span data-ttu-id="614a8-1243">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="614a8-1243">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="614a8-1244">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="614a8-1244">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="614a8-1245">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="614a8-1245">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="614a8-1246">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="614a8-1246">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="614a8-1247">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="614a8-1247">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="614a8-1248">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-1248">Lab</span></span>

* <span data-ttu-id="614a8-1249">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-1249">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="614a8-1250">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-1250">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="614a8-1251">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-1251">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="614a8-1252">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-1252">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="614a8-1253">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="614a8-1253">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="614a8-1254">Supervisión</span><span class="sxs-lookup"><span data-stu-id="614a8-1254">Monitor</span></span>

* <span data-ttu-id="614a8-1255">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="614a8-1255">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="614a8-1256">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="614a8-1256">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="614a8-1257">Red</span><span class="sxs-lookup"><span data-stu-id="614a8-1257">Network</span></span>

* <span data-ttu-id="614a8-1258">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="614a8-1258">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="614a8-1259">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="614a8-1259">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="614a8-1260">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="614a8-1260">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="614a8-1261">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="614a8-1261">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="614a8-1262">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="614a8-1262">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="614a8-1263">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="614a8-1263">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="614a8-1264">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="614a8-1264">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="614a8-1265">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="614a8-1265">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="614a8-1266">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="614a8-1266">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="614a8-1267">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="614a8-1267">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="614a8-1268">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="614a8-1268">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="614a8-1269">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="614a8-1269">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="614a8-1270">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="614a8-1270">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="614a8-1271">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="614a8-1271">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="614a8-1272">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="614a8-1272">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="614a8-1273">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="614a8-1273">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="614a8-1274">Perfil</span><span class="sxs-lookup"><span data-stu-id="614a8-1274">Profile</span></span>

* <span data-ttu-id="614a8-1275">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="614a8-1275">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="614a8-1276">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="614a8-1276">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="614a8-1277">Redis</span><span class="sxs-lookup"><span data-stu-id="614a8-1277">Redis</span></span>

* <span data-ttu-id="614a8-1278">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="614a8-1278">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="614a8-1279">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="614a8-1279">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="614a8-1280">Recurso</span><span class="sxs-lookup"><span data-stu-id="614a8-1280">Resource</span></span>

* <span data-ttu-id="614a8-1281">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="614a8-1281">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="614a8-1282">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="614a8-1282">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="614a8-1283">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="614a8-1283">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="614a8-1284">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="614a8-1284">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="614a8-1285">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="614a8-1285">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="614a8-1286">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="614a8-1286">Add docs for az lock update.</span></span> <span data-ttu-id="614a8-1287">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="614a8-1287">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="614a8-1288">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="614a8-1288">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="614a8-1289">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="614a8-1289">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="614a8-1290">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="614a8-1290">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="614a8-1291">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="614a8-1291">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="614a8-1292">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="614a8-1292">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="614a8-1293">Rol</span><span class="sxs-lookup"><span data-stu-id="614a8-1293">Role</span></span>

* <span data-ttu-id="614a8-1294">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="614a8-1294">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="614a8-1295">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="614a8-1295">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="614a8-1296">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="614a8-1296">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="614a8-1297">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="614a8-1297">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="614a8-1298">SQL</span><span class="sxs-lookup"><span data-stu-id="614a8-1298">SQL</span></span>

* <span data-ttu-id="614a8-1299">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="614a8-1299">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="614a8-1300">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="614a8-1300">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="614a8-1301">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-1301">Storage</span></span>

* <span data-ttu-id="614a8-1302">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="614a8-1302">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="614a8-1303">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="614a8-1303">Add support for incremental blob copy</span></span>
* <span data-ttu-id="614a8-1304">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="614a8-1304">Add support for large block blob upload</span></span>
* <span data-ttu-id="614a8-1305">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="614a8-1305">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-1306">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-1306">VM</span></span>

* <span data-ttu-id="614a8-1307">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="614a8-1307">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="614a8-1308">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="614a8-1308">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="614a8-1309">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="614a8-1309">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="614a8-1310">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="614a8-1310">az vm/vmss disk</span></span>
  3. <span data-ttu-id="614a8-1311">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="614a8-1311">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="614a8-1312">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="614a8-1312">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="614a8-1313">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="614a8-1313">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="614a8-1314">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-1314">April 3, 2017</span></span>

<span data-ttu-id="614a8-1315">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="614a8-1315">Version 2.0.2</span></span>

<span data-ttu-id="614a8-1316">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="614a8-1316">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="614a8-1317">Núcleo</span><span class="sxs-lookup"><span data-stu-id="614a8-1317">Core</span></span>

* <span data-ttu-id="614a8-1318">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="614a8-1318">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="614a8-1319">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="614a8-1319">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="614a8-1320">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="614a8-1320">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="614a8-1321">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="614a8-1321">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="614a8-1322">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="614a8-1322">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="614a8-1323">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="614a8-1323">Add prompting for missing template parameters.</span></span> <span data-ttu-id="614a8-1324">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="614a8-1324">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="614a8-1325">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="614a8-1325">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="614a8-1326">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="614a8-1326">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="614a8-1327">ACS</span><span class="sxs-lookup"><span data-stu-id="614a8-1327">ACS</span></span>

* <span data-ttu-id="614a8-1328">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="614a8-1328">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="614a8-1329">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="614a8-1329">Add support for ssh key password prompting.</span></span> <span data-ttu-id="614a8-1330">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="614a8-1330">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="614a8-1331">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="614a8-1331">Add support for windows clusters.</span></span> <span data-ttu-id="614a8-1332">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="614a8-1332">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="614a8-1333">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="614a8-1333">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="614a8-1334">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="614a8-1334">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="614a8-1335">AppService</span><span class="sxs-lookup"><span data-stu-id="614a8-1335">AppService</span></span>

* <span data-ttu-id="614a8-1336">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="614a8-1336">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="614a8-1337">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="614a8-1337">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="614a8-1338">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="614a8-1338">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="614a8-1339">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="614a8-1339">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="614a8-1340">DataLake</span><span class="sxs-lookup"><span data-stu-id="614a8-1340">DataLake</span></span>

* <span data-ttu-id="614a8-1341">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="614a8-1341">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="614a8-1342">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="614a8-1342">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="614a8-1343">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="614a8-1343">DocuemntDB</span></span>

* <span data-ttu-id="614a8-1344">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="614a8-1344">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="614a8-1345">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="614a8-1345">VM</span></span>

* <span data-ttu-id="614a8-1346">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="614a8-1346">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="614a8-1347">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="614a8-1347">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="614a8-1348">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="614a8-1348">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="614a8-1349">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="614a8-1349">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="614a8-1350">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="614a8-1350">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="614a8-1351">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="614a8-1351">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="614a8-1352">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="614a8-1352">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="614a8-1353">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="614a8-1353">February 27, 2017</span></span>

<span data-ttu-id="614a8-1354">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="614a8-1354">Version 2.0.0</span></span>

<span data-ttu-id="614a8-1355">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="614a8-1355">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="614a8-1356">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="614a8-1356">Container Service (acs)</span></span>
- <span data-ttu-id="614a8-1357">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="614a8-1357">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="614a8-1358">Redes</span><span class="sxs-lookup"><span data-stu-id="614a8-1358">Networking</span></span>
- <span data-ttu-id="614a8-1359">Storage</span><span class="sxs-lookup"><span data-stu-id="614a8-1359">Storage</span></span>

<span data-ttu-id="614a8-1360">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="614a8-1360">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="614a8-1361">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="614a8-1361">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="614a8-1362">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="614a8-1362">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="614a8-1363">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="614a8-1363">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="614a8-1364">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="614a8-1364">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="614a8-1365">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="614a8-1365">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="614a8-1366">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="614a8-1366">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="614a8-1367">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="614a8-1367">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="614a8-1368">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="614a8-1368">Provide feedback from the command line with the `az feedback` command</span></span>

