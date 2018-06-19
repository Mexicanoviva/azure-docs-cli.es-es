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
ms.openlocfilehash: 72e667d74ff8d55f26ecbf3b3c8845c9c03b56be
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512910"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="d1765-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="d1765-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d1765-104">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-104">June 13, 2018</span></span>

<span data-ttu-id="d1765-105">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="d1765-105">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="d1765-106">AKS</span><span class="sxs-lookup"><span data-stu-id="d1765-106">AKS</span></span>

* <span data-ttu-id="d1765-107">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1765-107">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="d1765-108">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="d1765-108">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="d1765-109">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1765-109">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="d1765-110">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1765-110">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="d1765-111">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1765-111">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-112">AppService</span><span class="sxs-lookup"><span data-stu-id="d1765-112">AppService</span></span>

* <span data-ttu-id="d1765-113">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="d1765-113">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d1765-114">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-114">June 5, 2018</span></span>

<span data-ttu-id="d1765-115">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="d1765-115">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-116">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-116">Interactive</span></span>

* <span data-ttu-id="d1765-117">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="d1765-117">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d1765-118">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-118">June 5, 2018</span></span>

<span data-ttu-id="d1765-119">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="d1765-119">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="d1765-120">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-120">Core</span></span>

* <span data-ttu-id="d1765-121">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="d1765-121">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="d1765-122">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="d1765-122">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-123">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-123">ACR</span></span>

* <span data-ttu-id="d1765-124">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="d1765-124">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="d1765-125">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="d1765-125">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="d1765-126">AKS</span><span class="sxs-lookup"><span data-stu-id="d1765-126">AKS</span></span>

* <span data-ttu-id="d1765-127">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="d1765-127">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="d1765-128">Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-128">Batch</span></span>

* <span data-ttu-id="d1765-129">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="d1765-129">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="d1765-130">IoT</span><span class="sxs-lookup"><span data-stu-id="d1765-130">IOT</span></span>

* <span data-ttu-id="d1765-131">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="d1765-131">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="d1765-132">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-132">Network</span></span>

* <span data-ttu-id="d1765-133">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="d1765-133">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="d1765-134">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="d1765-134">Policy Insights</span></span>

* <span data-ttu-id="d1765-135">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="d1765-135">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="d1765-136">ARM</span><span class="sxs-lookup"><span data-stu-id="d1765-136">ARM</span></span>

* <span data-ttu-id="d1765-137">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="d1765-137">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-138">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-138">SQL</span></span>

* <span data-ttu-id="d1765-139">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="d1765-139">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="d1765-140">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="d1765-140">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="d1765-141">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-141">Storage</span></span>

* <span data-ttu-id="d1765-142">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="d1765-142">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-143">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-143">VM</span></span>

* <span data-ttu-id="d1765-144">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="d1765-144">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="d1765-145">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1765-145">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="d1765-146">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="d1765-146">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="d1765-147">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-147">May 22, 2018</span></span>

<span data-ttu-id="d1765-148">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="d1765-148">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="d1765-149">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-149">Core</span></span>

* <span data-ttu-id="d1765-150">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="d1765-150">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-151">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-151">ACS</span></span>

* <span data-ttu-id="d1765-152">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="d1765-152">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="d1765-153">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="d1765-153">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-154">AppService</span><span class="sxs-lookup"><span data-stu-id="d1765-154">AppService</span></span>

* <span data-ttu-id="d1765-155">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="d1765-155">Improved generic update commands</span></span>
* <span data-ttu-id="d1765-156">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="d1765-156">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="d1765-157">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-157">Container</span></span>

* <span data-ttu-id="d1765-158">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="d1765-158">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="d1765-159">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d1765-159">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-160">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-160">Extension</span></span>

* <span data-ttu-id="d1765-161">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="d1765-161">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-162">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-162">Interactive</span></span>

* <span data-ttu-id="d1765-163">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="d1765-163">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="d1765-164">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="d1765-164">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1765-165">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d1765-165">KeyVault</span></span>

* <span data-ttu-id="d1765-166">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="d1765-166">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="d1765-167">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-167">Network</span></span>

* <span data-ttu-id="d1765-168">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="d1765-168">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="d1765-169">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="d1765-169">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-170">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-170">SQL</span></span>

* <span data-ttu-id="d1765-171">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="d1765-171">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="d1765-172">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="d1765-172">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="d1765-173">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="d1765-173">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="d1765-174">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="d1765-174">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="d1765-175">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="d1765-175">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="d1765-176">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="d1765-176">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="d1765-177">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="d1765-177">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="d1765-178">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d1765-178">`edition`.</span></span> <span data-ttu-id="d1765-179">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="d1765-179">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="d1765-180">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="d1765-180">`elasticPoolName`.</span></span> <span data-ttu-id="d1765-181">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="d1765-181">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="d1765-182">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="d1765-182">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="d1765-183">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d1765-183">`edition`.</span></span> <span data-ttu-id="d1765-184">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="d1765-184">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="d1765-185">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="d1765-185">`dtu`.</span></span> <span data-ttu-id="d1765-186">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="d1765-186">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="d1765-187">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="d1765-187">`databaseDtuMin`.</span></span> <span data-ttu-id="d1765-188">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="d1765-188">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="d1765-189">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="d1765-189">`databaseDtuMax`.</span></span> <span data-ttu-id="d1765-190">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="d1765-190">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="d1765-191">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d1765-191">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="d1765-192">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d1765-192">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-193">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-193">Storage</span></span>

* <span data-ttu-id="d1765-194">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="d1765-194">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="d1765-195">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="d1765-195">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-196">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-196">VM</span></span>

* <span data-ttu-id="d1765-197">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-197">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="d1765-198">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="d1765-198">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="d1765-199">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="d1765-199">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="d1765-200">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="d1765-200">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="d1765-201">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="d1765-201">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="d1765-202">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-202">May 7, 2018</span></span>

<span data-ttu-id="d1765-203">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="d1765-203">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="d1765-204">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-204">Core</span></span>

* <span data-ttu-id="d1765-205">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="d1765-205">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="d1765-206">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="d1765-206">Added limited support for positional arguments</span></span>
* <span data-ttu-id="d1765-207">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d1765-207">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="d1765-208">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="d1765-208">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="d1765-209">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d1765-209">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="d1765-210">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="d1765-210">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="d1765-211">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-211">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="d1765-212">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="d1765-212">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="d1765-213">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-213">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-214">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-214">ACR</span></span>

* <span data-ttu-id="d1765-215">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="d1765-215">Added ACR Build commands</span></span>
* <span data-ttu-id="d1765-216">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="d1765-216">Improved resource not found error messages</span></span>
* <span data-ttu-id="d1765-217">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="d1765-217">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="d1765-218">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="d1765-218">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="d1765-219">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="d1765-219">Improved repository commands error messages</span></span>
* <span data-ttu-id="d1765-220">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="d1765-220">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-221">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-221">ACS</span></span>

* <span data-ttu-id="d1765-222">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d1765-222">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="d1765-223">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="d1765-223">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="d1765-224">AMS</span><span class="sxs-lookup"><span data-stu-id="d1765-224">AMS</span></span>

* <span data-ttu-id="d1765-225">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="d1765-225">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-226">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-226">Appservice</span></span>

* <span data-ttu-id="d1765-227">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="d1765-227">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="d1765-228">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="d1765-228">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="d1765-229">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="d1765-229">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="d1765-230">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="d1765-230">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d1765-231">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d1765-231">Batch AI</span></span>

* <span data-ttu-id="d1765-232">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="d1765-232">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d1765-233">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d1765-233">Cognitive Services</span></span>

* <span data-ttu-id="d1765-234">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="d1765-234">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="d1765-235">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1765-235">Consumption</span></span>

* <span data-ttu-id="d1765-236">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="d1765-236">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="d1765-237">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-237">Container</span></span>

* <span data-ttu-id="d1765-238">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="d1765-238">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d1765-239">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d1765-239">Cosmos DB</span></span>

* <span data-ttu-id="d1765-240">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d1765-240">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="d1765-241">DMS</span><span class="sxs-lookup"><span data-stu-id="d1765-241">DMS</span></span>

* <span data-ttu-id="d1765-242">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-242">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-243">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-243">Extension</span></span>

* <span data-ttu-id="d1765-244">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="d1765-244">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-245">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-245">Interactive</span></span>

* <span data-ttu-id="d1765-246">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="d1765-246">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="d1765-247">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="d1765-247">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="d1765-248">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="d1765-248">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="d1765-249">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-249">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="d1765-250">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-250">Lab</span></span>

* <span data-ttu-id="d1765-251">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="d1765-251">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="d1765-252">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-252">Network</span></span>

* <span data-ttu-id="d1765-253">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="d1765-253">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="d1765-254">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-254">Profile</span></span>

* <span data-ttu-id="d1765-255">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="d1765-255">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="d1765-256">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="d1765-256">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="d1765-257">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="d1765-257">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="d1765-258">Redis</span><span class="sxs-lookup"><span data-stu-id="d1765-258">Redis</span></span>

* <span data-ttu-id="d1765-259">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="d1765-259">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="d1765-260">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="d1765-260">Deprecated `redis list-all`.</span></span> <span data-ttu-id="d1765-261">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="d1765-261">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="d1765-262">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="d1765-262">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="d1765-263">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-263">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="d1765-264">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-264">Role</span></span>

* <span data-ttu-id="d1765-265">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="d1765-265">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-266">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-266">Storage</span></span>

* <span data-ttu-id="d1765-267">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="d1765-267">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="d1765-268">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="d1765-268">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="d1765-269">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="d1765-269">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="d1765-270">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="d1765-270">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="d1765-271">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="d1765-271">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-272">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-272">VM</span></span>

* <span data-ttu-id="d1765-273">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="d1765-273">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="d1765-274">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="d1765-274">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="d1765-275">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="d1765-275">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="d1765-276">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="d1765-276">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="d1765-277">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="d1765-277">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="d1765-278">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="d1765-278">Added write accelerator support</span></span> 
* <span data-ttu-id="d1765-279">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="d1765-279">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="d1765-280">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="d1765-280">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="d1765-281">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="d1765-281">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="d1765-282">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-282">April 10, 2018</span></span>

<span data-ttu-id="d1765-283">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="d1765-283">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-284">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-284">ACR</span></span>

* <span data-ttu-id="d1765-285">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="d1765-285">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-286">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-286">ACS</span></span>

* <span data-ttu-id="d1765-287">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="d1765-287">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-288">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-288">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="d1765-290">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="d1765-290">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="d1765-291">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d1765-291">BatchAI</span></span>

* <span data-ttu-id="d1765-292">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="d1765-292">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="d1765-293">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="d1765-293">Job level mounting</span></span>
 - <span data-ttu-id="d1765-294">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="d1765-294">Environment variables with secret values</span></span>
 - <span data-ttu-id="d1765-295">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="d1765-295">Performance counters settings</span></span>
 - <span data-ttu-id="d1765-296">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="d1765-296">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="d1765-297">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="d1765-297">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="d1765-298">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="d1765-298">Usage and limits reporting</span></span>
 - <span data-ttu-id="d1765-299">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="d1765-299">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="d1765-300">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="d1765-300">Support for custom images</span></span>
 - <span data-ttu-id="d1765-301">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="d1765-301">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="d1765-302">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="d1765-302">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="d1765-303">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="d1765-303">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="d1765-304">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="d1765-304">National clouds are supported</span></span>
* <span data-ttu-id="d1765-305">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="d1765-305">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="d1765-306">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="d1765-306">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="d1765-307">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="d1765-307">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="d1765-308">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="d1765-308">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="d1765-309">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="d1765-309">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="d1765-310">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="d1765-310">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="d1765-311">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="d1765-311">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="d1765-312">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="d1765-312">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="d1765-313">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="d1765-313">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="d1765-314">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d1765-314">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="d1765-315">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-315">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="d1765-316">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="d1765-316">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="d1765-317">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d1765-317">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="d1765-318">Facturación</span><span class="sxs-lookup"><span data-stu-id="d1765-318">Billing</span></span>

* <span data-ttu-id="d1765-319">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="d1765-319">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="d1765-320">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1765-320">Consumption</span></span>

* <span data-ttu-id="d1765-321">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="d1765-321">Added `marketplace` commands</span></span>
* <span data-ttu-id="d1765-322">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d1765-322">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="d1765-323">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="d1765-323">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="d1765-324">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="d1765-324">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="d1765-325">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d1765-325">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="d1765-326">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="d1765-326">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="d1765-327">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-327">Container</span></span>

* <span data-ttu-id="d1765-328">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="d1765-328">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="d1765-329">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="d1765-329">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-330">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-330">Extension</span></span>

* <span data-ttu-id="d1765-331">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="d1765-331">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-332">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-332">Interactive</span></span>

* <span data-ttu-id="d1765-333">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="d1765-333">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="d1765-334">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-334">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="d1765-335">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="d1765-335">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="d1765-336">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-336">Network</span></span>

* <span data-ttu-id="d1765-337">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d1765-337">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="d1765-338">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="d1765-338">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="d1765-339">4910</span><span class="sxs-lookup"><span data-stu-id="d1765-339">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="d1765-340">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="d1765-340">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="d1765-341">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="d1765-341">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="d1765-342">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-342">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="d1765-343">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-343">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="d1765-344">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="d1765-344">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-345">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-345">Profile</span></span>

* <span data-ttu-id="d1765-346">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="d1765-346">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="d1765-347">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="d1765-347">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1765-348">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1765-348">RDBMS</span></span>

* <span data-ttu-id="d1765-349">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="d1765-349">Added `georestore` command</span></span>
* <span data-ttu-id="d1765-350">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="d1765-350">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-351">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-351">Resource</span></span>

* <span data-ttu-id="d1765-352">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-352">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="d1765-353">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d1765-353">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-354">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-354">SQL</span></span>

* <span data-ttu-id="d1765-355">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="d1765-355">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-356">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-356">Storage</span></span>

* <span data-ttu-id="d1765-357">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="d1765-357">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-358">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-358">VM</span></span>

* <span data-ttu-id="d1765-359">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1765-359">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="d1765-360">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="d1765-360">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="d1765-362">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1765-362">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="d1765-363">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="d1765-363">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="d1765-364">5718</span><span class="sxs-lookup"><span data-stu-id="d1765-364">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="d1765-365">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="d1765-365">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="d1765-366">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-366">March 27, 2018</span></span>

<span data-ttu-id="d1765-367">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="d1765-367">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="d1765-368">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-368">Core</span></span>

* <span data-ttu-id="d1765-369">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="d1765-369">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-370">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-370">ACS</span></span>

* <span data-ttu-id="d1765-371">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d1765-371">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-372">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-372">Appservice</span></span>

* <span data-ttu-id="d1765-373">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d1765-373">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="d1765-374">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="d1765-374">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d1765-375">Backup</span><span class="sxs-lookup"><span data-stu-id="d1765-375">Backup</span></span>

* <span data-ttu-id="d1765-376">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="d1765-376">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="d1765-377">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-377">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="d1765-378">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="d1765-378">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="d1765-379">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="d1765-379">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="d1765-380">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-380">Container</span></span>

* <span data-ttu-id="d1765-381">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="d1765-381">Added `container exec` command.</span></span> <span data-ttu-id="d1765-382">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="d1765-382">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="d1765-383">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d1765-383">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-384">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-384">Extension</span></span>

* <span data-ttu-id="d1765-385">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d1765-385">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="d1765-386">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="d1765-386">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="d1765-387">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="d1765-387">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-388">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-388">Interactive</span></span>

* <span data-ttu-id="d1765-389">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-389">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="d1765-390">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="d1765-390">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="d1765-391">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-391">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="d1765-392">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="d1765-392">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="d1765-393">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-393">Lab</span></span>

* <span data-ttu-id="d1765-394">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="d1765-394">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-395">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-395">Monitor</span></span>

* <span data-ttu-id="d1765-396">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d1765-396">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="d1765-397">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="d1765-397">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="d1765-398">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d1765-398">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="d1765-399">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-399">Network</span></span>

* <span data-ttu-id="d1765-400">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="d1765-400">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-401">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-401">Profile</span></span>

* <span data-ttu-id="d1765-402">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="d1765-402">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1765-403">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1765-403">RDBMS</span></span>

* <span data-ttu-id="d1765-404">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="d1765-404">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-405">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-405">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="d1765-407">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-407">Role</span></span>

* <span data-ttu-id="d1765-408">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="d1765-408">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="d1765-409">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="d1765-409">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="d1765-410">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="d1765-410">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="d1765-411">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d1765-411">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="d1765-412">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="d1765-412">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-413">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-413">Storage</span></span>

* <span data-ttu-id="d1765-414">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="d1765-414">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="d1765-415">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="d1765-415">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-416">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-416">VM</span></span>

* <span data-ttu-id="d1765-417">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="d1765-417">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="d1765-418">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="d1765-418">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="d1765-419">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="d1765-419">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="d1765-420">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="d1765-420">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="d1765-421">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-421">March 13, 2018</span></span>

<span data-ttu-id="d1765-422">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="d1765-422">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-423">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-423">ACR</span></span>

* <span data-ttu-id="d1765-424">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="d1765-424">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="d1765-425">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="d1765-425">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="d1765-426">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="d1765-426">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-427">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-427">ACS</span></span>

* <span data-ttu-id="d1765-428">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="d1765-428">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="d1765-429">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="d1765-429">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="d1765-430">Advisor</span><span class="sxs-lookup"><span data-stu-id="d1765-430">Advisor</span></span>

* <span data-ttu-id="d1765-431">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="d1765-431">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="d1765-432">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="d1765-432">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="d1765-433">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="d1765-433">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="d1765-434">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="d1765-434">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="d1765-435">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="d1765-435">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-436">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-436">Appservice</span></span>

* <span data-ttu-id="d1765-437">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="d1765-437">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="d1765-438">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="d1765-438">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d1765-439">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="d1765-439">Eventhubs</span></span>

* <span data-ttu-id="d1765-440">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d1765-440">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-441">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-441">Extension</span></span>

* <span data-ttu-id="d1765-442">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="d1765-442">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-443">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-443">Interactive</span></span>

* <span data-ttu-id="d1765-444">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="d1765-444">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="d1765-445">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="d1765-445">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="d1765-446">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="d1765-446">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="d1765-447">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="d1765-447">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-448">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-448">Monitor</span></span>

* <span data-ttu-id="d1765-449">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="d1765-449">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="d1765-450">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="d1765-450">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="d1765-451">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="d1765-451">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="d1765-452">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="d1765-452">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="d1765-453">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-453">Network</span></span>

* <span data-ttu-id="d1765-454">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="d1765-454">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="d1765-455">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="d1765-455">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="d1765-456">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="d1765-456">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="d1765-457">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="d1765-457">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-458">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-458">Profile</span></span>

* <span data-ttu-id="d1765-459">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="d1765-459">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="d1765-460">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="d1765-460">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1765-461">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1765-461">RDBMS</span></span>

* <span data-ttu-id="d1765-462">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="d1765-462">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="d1765-463">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="d1765-463">Service Bus</span></span>

* <span data-ttu-id="d1765-464">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d1765-464">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-465">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-465">Storage</span></span>

* <span data-ttu-id="d1765-466">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="d1765-466">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="d1765-467">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="d1765-467">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-468">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-468">VM</span></span>

* <span data-ttu-id="d1765-469">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="d1765-469">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="d1765-470">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="d1765-470">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="d1765-471">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="d1765-471">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="d1765-472">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="d1765-472">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="d1765-473">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-473">February 27, 2018</span></span>

<span data-ttu-id="d1765-474">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="d1765-474">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="d1765-475">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-475">Core</span></span>

* <span data-ttu-id="d1765-476">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="d1765-476">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="d1765-477">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="d1765-477">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="d1765-478">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="d1765-478">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-479">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-479">ACS</span></span>

* <span data-ttu-id="d1765-480">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="d1765-480">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="d1765-481">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="d1765-481">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="d1765-482">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d1765-482">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="d1765-483">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="d1765-483">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-484">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-484">Appservice</span></span>

* <span data-ttu-id="d1765-485">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="d1765-485">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="d1765-486">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="d1765-486">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d1765-487">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d1765-487">Cognitive Services</span></span>

* <span data-ttu-id="d1765-488">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d1765-488">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="d1765-489">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1765-489">Consumption</span></span>

* <span data-ttu-id="d1765-490">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="d1765-490">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="d1765-491">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="d1765-491">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="d1765-492">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-492">Container</span></span>

* <span data-ttu-id="d1765-493">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="d1765-493">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="d1765-494">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-494">Network</span></span>

* <span data-ttu-id="d1765-495">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="d1765-495">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-496">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-496">Resource</span></span>

* <span data-ttu-id="d1765-497">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="d1765-497">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="d1765-498">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-498">Role</span></span>

* <span data-ttu-id="d1765-499">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="d1765-499">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-500">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-500">SQL</span></span>

* <span data-ttu-id="d1765-501">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="d1765-501">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-502">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-502">Storage</span></span>

* <span data-ttu-id="d1765-503">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="d1765-503">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-504">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-504">VM</span></span>

* <span data-ttu-id="d1765-505">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="d1765-505">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="d1765-506">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-506">February 13, 2018</span></span>

<span data-ttu-id="d1765-507">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="d1765-507">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="d1765-508">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-508">Core</span></span>

* <span data-ttu-id="d1765-509">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="d1765-509">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-510">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-510">ACS</span></span>

* <span data-ttu-id="d1765-511">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="d1765-511">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="d1765-512">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1765-512">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="d1765-513">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d1765-513">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="d1765-514">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="d1765-514">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="d1765-515">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="d1765-515">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="d1765-516">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="d1765-516">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="d1765-517">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d1765-517">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="d1765-518">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="d1765-518">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-519">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-519">Appservice</span></span>

* <span data-ttu-id="d1765-520">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="d1765-520">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="d1765-521">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="d1765-521">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="d1765-522">CDN</span><span class="sxs-lookup"><span data-stu-id="d1765-522">CDN</span></span>

* <span data-ttu-id="d1765-523">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="d1765-523">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="d1765-524">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-524">Container</span></span>

* <span data-ttu-id="d1765-525">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="d1765-525">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="d1765-526">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d1765-526">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1765-527">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1765-527">CosmosDB</span></span>

* <span data-ttu-id="d1765-528">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d1765-528">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-529">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-529">Extension</span></span>

* <span data-ttu-id="d1765-530">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-530">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="d1765-531">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-531">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="d1765-532">Comentarios</span><span class="sxs-lookup"><span data-stu-id="d1765-532">Feedback</span></span>

* <span data-ttu-id="d1765-533">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="d1765-533">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-534">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-534">Interactive</span></span>

* <span data-ttu-id="d1765-535">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d1765-535">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="d1765-536">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="d1765-536">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="d1765-537">IoT</span><span class="sxs-lookup"><span data-stu-id="d1765-537">IoT</span></span>

* <span data-ttu-id="d1765-538">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="d1765-538">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d1765-539">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="d1765-539">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d1765-540">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-540">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="d1765-541">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="d1765-541">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-542">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-542">Monitor</span></span>

* <span data-ttu-id="d1765-543">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="d1765-543">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="d1765-544">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-544">Network</span></span>

* <span data-ttu-id="d1765-545">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="d1765-545">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="d1765-546">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-546">Profile</span></span>

* <span data-ttu-id="d1765-547">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="d1765-547">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-548">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-548">Resource</span></span>

* <span data-ttu-id="d1765-549">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="d1765-549">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="d1765-550">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-550">Role</span></span>

* <span data-ttu-id="d1765-551">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="d1765-551">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-552">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-552">SQL</span></span>

* <span data-ttu-id="d1765-553">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="d1765-553">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="d1765-554">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="d1765-554">Added `sql db rename`</span></span>
* <span data-ttu-id="d1765-555">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="d1765-555">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-556">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-556">Storage</span></span>

* <span data-ttu-id="d1765-557">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="d1765-557">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-558">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-558">VM</span></span>

* <span data-ttu-id="d1765-559">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="d1765-559">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="d1765-560">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="d1765-560">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="d1765-561">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="d1765-561">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="d1765-562">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-562">January 31, 2018</span></span>

<span data-ttu-id="d1765-563">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="d1765-563">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="d1765-564">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-564">Core</span></span>

* <span data-ttu-id="d1765-565">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="d1765-565">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="d1765-566">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="d1765-566">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="d1765-567">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="d1765-567">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="d1765-568">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="d1765-568">Use `--verbose` to see</span></span>
* <span data-ttu-id="d1765-569">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="d1765-569">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-570">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-570">ACS</span></span>

* <span data-ttu-id="d1765-571">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="d1765-571">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="d1765-572">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="d1765-572">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-573">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-573">Appservice</span></span>

* <span data-ttu-id="d1765-574">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="d1765-574">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="d1765-575">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="d1765-575">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="d1765-576">CDN</span><span class="sxs-lookup"><span data-stu-id="d1765-576">CDN</span></span>

* <span data-ttu-id="d1765-577">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d1765-577">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1765-578">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1765-578">CosmosDB</span></span>

* <span data-ttu-id="d1765-579">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="d1765-579">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-580">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-580">Interactive</span></span>

* <span data-ttu-id="d1765-581">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="d1765-581">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="d1765-582">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-582">Network</span></span>

* <span data-ttu-id="d1765-583">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d1765-583">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="d1765-584">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="d1765-584">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="d1765-585">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d1765-585">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="d1765-586">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="d1765-586">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="d1765-587">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="d1765-587">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="d1765-588">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="d1765-588">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="d1765-589">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="d1765-589">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="d1765-590">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="d1765-590">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="d1765-591">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d1765-591">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="d1765-592">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="d1765-592">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-593">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-593">Profile</span></span>

* <span data-ttu-id="d1765-594">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="d1765-594">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-595">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-595">Resource</span></span>

* <span data-ttu-id="d1765-596">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="d1765-596">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-597">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-597">Storage</span></span>

* <span data-ttu-id="d1765-598">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="d1765-598">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="d1765-599">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="d1765-599">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="d1765-600">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="d1765-600">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="d1765-601">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d1765-601">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="d1765-602">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="d1765-602">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-603">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-603">VM</span></span>

* <span data-ttu-id="d1765-604">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="d1765-604">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="d1765-605">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="d1765-605">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="d1765-606">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="d1765-606">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="d1765-607">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1765-607">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="d1765-608">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="d1765-608">January 17, 2018</span></span>

<span data-ttu-id="d1765-609">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="d1765-609">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-610">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-610">ACR</span></span>

* <span data-ttu-id="d1765-611">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="d1765-611">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="d1765-612">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="d1765-612">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-613">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-613">ACS</span></span>

* <span data-ttu-id="d1765-614">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="d1765-614">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="d1765-615">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="d1765-615">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-616">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-616">Appservice</span></span>

* <span data-ttu-id="d1765-617">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="d1765-617">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="d1765-618">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="d1765-618">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="d1765-619">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="d1765-619">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="d1765-620">Backup</span><span class="sxs-lookup"><span data-stu-id="d1765-620">Backup</span></span>

* <span data-ttu-id="d1765-621">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="d1765-621">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="d1765-622">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="d1765-622">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="d1765-623">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="d1765-623">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="d1765-624">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="d1765-624">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="d1765-625">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="d1765-625">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="d1765-626">Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-626">Batch</span></span>

* <span data-ttu-id="d1765-627">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="d1765-627">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="d1765-628">Nube</span><span class="sxs-lookup"><span data-stu-id="d1765-628">Cloud</span></span>

* <span data-ttu-id="d1765-629">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="d1765-629">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="d1765-630">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1765-630">Consumption</span></span>

* <span data-ttu-id="d1765-631">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="d1765-631">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="d1765-632">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d1765-632">Event Grid</span></span>

* <span data-ttu-id="d1765-633">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d1765-633">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d1765-634">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d1765-634">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d1765-635">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="d1765-635">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="d1765-636">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="d1765-636">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="d1765-637">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="d1765-637">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="d1765-638">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="d1765-638">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="d1765-639">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="d1765-639">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="d1765-640">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="d1765-640">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-641">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-641">Interactive</span></span>

* <span data-ttu-id="d1765-642">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="d1765-642">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="d1765-643">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="d1765-643">Fixed errors on startup</span></span>
* <span data-ttu-id="d1765-644">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="d1765-644">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="d1765-645">IoT</span><span class="sxs-lookup"><span data-stu-id="d1765-645">IoT</span></span>

* <span data-ttu-id="d1765-646">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d1765-646">Added support for device provisioning service</span></span>
* <span data-ttu-id="d1765-647">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-647">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="d1765-648">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="d1765-648">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-649">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-649">Monitor</span></span>

* <span data-ttu-id="d1765-650">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="d1765-650">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="d1765-651">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d1765-651">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="d1765-652">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="d1765-652">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="d1765-653">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-653">Network</span></span>

* <span data-ttu-id="d1765-654">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="d1765-654">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="d1765-655">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-655">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-656">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-656">Profile</span></span>

* <span data-ttu-id="d1765-657">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="d1765-657">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="d1765-658">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-658">Role</span></span>

* <span data-ttu-id="d1765-659">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="d1765-659">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d1765-660">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1765-660">Service Fabric</span></span>

* <span data-ttu-id="d1765-661">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="d1765-661">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="d1765-662">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="d1765-662">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-663">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-663">VM</span></span>

* <span data-ttu-id="d1765-664">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="d1765-664">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="d1765-665">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="d1765-665">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="d1765-666">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="d1765-666">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="d1765-667">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="d1765-667">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="d1765-668">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="d1765-668">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="d1765-669">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1765-669">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="d1765-670">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1765-670">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="d1765-671">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="d1765-671">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="d1765-672">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-672">December 19, 2017</span></span>

<span data-ttu-id="d1765-673">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="d1765-673">Version 2.0.23</span></span>

* <span data-ttu-id="d1765-674">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="d1765-674">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="d1765-675">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-675">Container</span></span>

* <span data-ttu-id="d1765-676">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-676">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="d1765-677">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-677">Network</span></span>

* <span data-ttu-id="d1765-678">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-678">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="d1765-679">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-679">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-680">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-680">Storage</span></span>

* <span data-ttu-id="d1765-681">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="d1765-681">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-682">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-682">VM</span></span>

* <span data-ttu-id="d1765-683">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="d1765-683">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="d1765-684">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-684">December 5, 2017</span></span>

<span data-ttu-id="d1765-685">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="d1765-685">Version 2.0.22</span></span>

* <span data-ttu-id="d1765-686">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="d1765-686">Removed `az component` commands.</span></span> <span data-ttu-id="d1765-687">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="d1765-687">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="d1765-688">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-688">Core</span></span>
* <span data-ttu-id="d1765-689">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="d1765-689">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="d1765-690">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="d1765-690">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-691">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-691">ACS</span></span>

* <span data-ttu-id="d1765-692">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="d1765-692">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="d1765-693">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="d1765-693">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="d1765-694">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="d1765-694">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="d1765-695">Advisor</span><span class="sxs-lookup"><span data-stu-id="d1765-695">Advisor</span></span>

* <span data-ttu-id="d1765-696">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d1765-696">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-697">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-697">Appservice</span></span>

* <span data-ttu-id="d1765-698">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="d1765-698">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="d1765-699">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="d1765-699">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="d1765-700">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="d1765-700">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="d1765-701">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1765-701">Consumption</span></span>

* <span data-ttu-id="d1765-702">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="d1765-702">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="d1765-703">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-703">Container</span></span>

* <span data-ttu-id="d1765-704">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="d1765-704">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-705">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-705">Monitor</span></span>

* <span data-ttu-id="d1765-706">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="d1765-706">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-707">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-707">Resource</span></span>

* <span data-ttu-id="d1765-708">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="d1765-708">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="d1765-709">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-709">Role</span></span>

* <span data-ttu-id="d1765-710">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="d1765-710">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="d1765-711">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="d1765-711">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="d1765-712">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d1765-712">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-713">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-713">SQL</span></span>

* <span data-ttu-id="d1765-714">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="d1765-714">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="d1765-715">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="d1765-715">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-716">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-716">VM</span></span>

* <span data-ttu-id="d1765-717">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="d1765-717">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="d1765-718">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-718">November 14, 2017</span></span>

<span data-ttu-id="d1765-719">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="d1765-719">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-720">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-720">ACR</span></span>

* <span data-ttu-id="d1765-721">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="d1765-721">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="d1765-722">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-722">ACS</span></span>

* <span data-ttu-id="d1765-723">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="d1765-723">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="d1765-724">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="d1765-724">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="d1765-725">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="d1765-725">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="d1765-726">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="d1765-726">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="d1765-727">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="d1765-727">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-728">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-728">Appservice</span></span>

* <span data-ttu-id="d1765-729">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="d1765-729">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="d1765-730">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d1765-730">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="d1765-731">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d1765-731">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="d1765-732">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="d1765-732">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="d1765-733">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="d1765-733">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="d1765-734">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="d1765-734">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="d1765-735">Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-735">Batch</span></span>

* <span data-ttu-id="d1765-736">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="d1765-736">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="d1765-737">Batchai</span><span class="sxs-lookup"><span data-stu-id="d1765-737">Batchai</span></span>

* <span data-ttu-id="d1765-738">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d1765-738">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="d1765-739">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d1765-739">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="d1765-740">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="d1765-740">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="d1765-741">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="d1765-741">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="d1765-742">Nube</span><span class="sxs-lookup"><span data-stu-id="d1765-742">Cloud</span></span>

* <span data-ttu-id="d1765-743">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="d1765-743">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="d1765-744">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-744">Container</span></span>

* <span data-ttu-id="d1765-745">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="d1765-745">Added support to open multiple ports</span></span>
* <span data-ttu-id="d1765-746">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d1765-746">Added container group restart policy</span></span>
* <span data-ttu-id="d1765-747">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="d1765-747">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="d1765-748">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="d1765-748">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d1765-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1765-749">Data Lake Analytics</span></span>

* <span data-ttu-id="d1765-750">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="d1765-750">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d1765-751">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1765-751">Data Lake Store</span></span>

* <span data-ttu-id="d1765-752">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="d1765-752">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-753">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-753">Extension</span></span>

* <span data-ttu-id="d1765-754">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="d1765-754">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="d1765-755">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="d1765-755">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="d1765-756">IoT</span><span class="sxs-lookup"><span data-stu-id="d1765-756">IoT</span></span>

* <span data-ttu-id="d1765-757">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="d1765-757">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-758">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-758">Monitor</span></span>

* <span data-ttu-id="d1765-759">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="d1765-759">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d1765-760">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-760">Network</span></span>

* <span data-ttu-id="d1765-761">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="d1765-761">Added support for CAA DNS records</span></span>
* <span data-ttu-id="d1765-762">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="d1765-762">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="d1765-763">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-763">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="d1765-764">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="d1765-764">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="d1765-765">Reservations</span><span class="sxs-lookup"><span data-stu-id="d1765-765">Reservations</span></span>

* <span data-ttu-id="d1765-766">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="d1765-766">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-767">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-767">Resource</span></span>

* <span data-ttu-id="d1765-768">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-768">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-769">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-769">SQL</span></span>

* <span data-ttu-id="d1765-770">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-770">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-771">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-771">Storage</span></span>

* <span data-ttu-id="d1765-772">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="d1765-772">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="d1765-773">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="d1765-773">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="d1765-774">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="d1765-774">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="d1765-775">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="d1765-775">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="d1765-776">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="d1765-776">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="d1765-777">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="d1765-777">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="d1765-778">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="d1765-778">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-779">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-779">VM</span></span>

* <span data-ttu-id="d1765-780">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="d1765-780">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="d1765-781">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="d1765-781">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="d1765-782">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="d1765-782">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="d1765-783">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="d1765-783">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="d1765-784">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d1765-784">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="d1765-785">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-785">October 24, 2017</span></span>

<span data-ttu-id="d1765-786">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="d1765-786">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="d1765-787">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-787">Core</span></span>

* <span data-ttu-id="d1765-788">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="d1765-788">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-789">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-789">ACR</span></span>

* <span data-ttu-id="d1765-790">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="d1765-790">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="d1765-791">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="d1765-791">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="d1765-792">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="d1765-792">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-793">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-793">ACS</span></span>

* <span data-ttu-id="d1765-794">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="d1765-794">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="d1765-795">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d1765-795">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-796">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-796">Appservice</span></span>

* <span data-ttu-id="d1765-797">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="d1765-797">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="d1765-798">Componente</span><span class="sxs-lookup"><span data-stu-id="d1765-798">Component</span></span>

* <span data-ttu-id="d1765-799">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="d1765-799">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-800">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-800">Monitor</span></span>

* <span data-ttu-id="d1765-801">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="d1765-801">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-802">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-802">Resource</span></span>

* <span data-ttu-id="d1765-803">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="d1765-803">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="d1765-804">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="d1765-804">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-805">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-805">VM</span></span>

* <span data-ttu-id="d1765-806">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1765-806">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="d1765-807">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-807">October 9, 2017</span></span>

<span data-ttu-id="d1765-808">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="d1765-808">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="d1765-809">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-809">Core</span></span>

* <span data-ttu-id="d1765-810">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d1765-810">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-811">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-811">Appservice</span></span>

* <span data-ttu-id="d1765-812">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d1765-812">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="d1765-813">Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-813">Batch</span></span>

* <span data-ttu-id="d1765-814">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d1765-814">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="d1765-815">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="d1765-815">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="d1765-816">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-816">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="d1765-817">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="d1765-817">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="d1765-818">Batchai</span><span class="sxs-lookup"><span data-stu-id="d1765-818">Batchai</span></span>

* <span data-ttu-id="d1765-819">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-819">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1765-820">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1765-820">Keyvault</span></span>

* <span data-ttu-id="d1765-821">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d1765-821">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="d1765-822">(#4448)</span><span class="sxs-lookup"><span data-stu-id="d1765-822">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="d1765-823">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-823">Network</span></span>

* <span data-ttu-id="d1765-824">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="d1765-824">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="d1765-825">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="d1765-825">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-826">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-826">Resource</span></span>

* <span data-ttu-id="d1765-827">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-827">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="d1765-828">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="d1765-828">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="d1765-829">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="d1765-829">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="d1765-830">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-830">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-831">Sql</span><span class="sxs-lookup"><span data-stu-id="d1765-831">Sql</span></span>

* <span data-ttu-id="d1765-832">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="d1765-832">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="d1765-833">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="d1765-833">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="d1765-834">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="d1765-834">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-835">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-835">Storage</span></span>

* <span data-ttu-id="d1765-836">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="d1765-836">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-837">Vm</span><span class="sxs-lookup"><span data-stu-id="d1765-837">Vm</span></span>

* <span data-ttu-id="d1765-838">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="d1765-838">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="d1765-839">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1765-839">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="d1765-840">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d1765-840">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="d1765-841">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1765-841">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="d1765-842">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1765-842">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="d1765-843">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-843">September 22, 2017</span></span>

<span data-ttu-id="d1765-844">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="d1765-844">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-845">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-845">Resource</span></span>

* <span data-ttu-id="d1765-846">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="d1765-846">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="d1765-847">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="d1765-847">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="d1765-848">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="d1765-848">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="d1765-849">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="d1765-849">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="d1765-850">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-850">Network</span></span>

* <span data-ttu-id="d1765-851">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="d1765-851">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="d1765-852">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="d1765-852">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="d1765-853">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="d1765-853">Added `asg` application security group commands</span></span>
* <span data-ttu-id="d1765-854">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-854">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="d1765-855">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-855">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d1765-856">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-856">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="d1765-857">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="d1765-857">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-858">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-858">Storage</span></span>

* <span data-ttu-id="d1765-859">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="d1765-859">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d1765-860">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="d1765-860">Eventgrid</span></span>

* <span data-ttu-id="d1765-861">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="d1765-861">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-862">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-862">SQL</span></span>

* <span data-ttu-id="d1765-863">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="d1765-863">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="d1765-864">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="d1765-864">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="d1765-865">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-865">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1765-866">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1765-866">Keyvault</span></span>

* <span data-ttu-id="d1765-867">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="d1765-867">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-868">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-868">VM</span></span>

* <span data-ttu-id="d1765-869">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="d1765-869">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="d1765-870">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="d1765-870">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="d1765-871">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1765-871">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="d1765-872">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="d1765-872">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="d1765-873">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="d1765-873">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="d1765-874">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d1765-874">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-875">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-875">ACS</span></span>

* <span data-ttu-id="d1765-876">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-876">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-877">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-877">Appservice</span></span>

* <span data-ttu-id="d1765-878">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="d1765-878">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d1765-879">Backup</span><span class="sxs-lookup"><span data-stu-id="d1765-879">Backup</span></span>

* <span data-ttu-id="d1765-880">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d1765-880">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="d1765-881">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-881">September 11, 2017</span></span>

<span data-ttu-id="d1765-882">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="d1765-882">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="d1765-883">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-883">Core</span></span>

* <span data-ttu-id="d1765-884">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="d1765-884">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="d1765-885">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="d1765-885">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-886">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-886">Acs</span></span>

* <span data-ttu-id="d1765-887">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="d1765-887">Added `acs list-locations` command</span></span>
* <span data-ttu-id="d1765-888">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="d1765-888">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-889">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-889">Appservice</span></span>

* <span data-ttu-id="d1765-890">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="d1765-890">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="d1765-891">CDN</span><span class="sxs-lookup"><span data-stu-id="d1765-891">CDN</span></span>

* <span data-ttu-id="d1765-892">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d1765-892">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="d1765-893">Extensión</span><span class="sxs-lookup"><span data-stu-id="d1765-893">Extension</span></span>

* <span data-ttu-id="d1765-894">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="d1765-894">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1765-895">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1765-895">Keyvault</span></span>

* <span data-ttu-id="d1765-896">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="d1765-896">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="d1765-897">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-897">Network</span></span>

* <span data-ttu-id="d1765-898">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="d1765-898">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d1765-899">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-899">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="d1765-900">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-900">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="d1765-901">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-901">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d1765-902">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-902">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-903">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-903">Resource</span></span>

* <span data-ttu-id="d1765-904">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-904">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="d1765-905">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-905">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="d1765-906">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="d1765-906">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="d1765-907">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="d1765-907">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-908">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-908">SQL</span></span>

* <span data-ttu-id="d1765-909">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="d1765-909">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-910">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-910">VM</span></span>

* <span data-ttu-id="d1765-911">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="d1765-911">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="d1765-912">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="d1765-912">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="d1765-913">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-913">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="d1765-914">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="d1765-914">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="d1765-915">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="d1765-915">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="d1765-916">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-916">August 31, 2017</span></span>

<span data-ttu-id="d1765-917">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="d1765-917">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1765-918">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1765-918">Keyvault</span></span>

* <span data-ttu-id="d1765-919">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="d1765-919">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="d1765-920">Sf</span><span class="sxs-lookup"><span data-stu-id="d1765-920">Sf</span></span>

* <span data-ttu-id="d1765-921">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="d1765-921">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-922">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-922">Storage</span></span>

* <span data-ttu-id="d1765-923">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="d1765-923">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="d1765-924">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="d1765-924">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="d1765-925">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-925">August 28, 2017</span></span>

<span data-ttu-id="d1765-926">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="d1765-926">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="d1765-927">CLI</span><span class="sxs-lookup"><span data-stu-id="d1765-927">CLI</span></span>

* <span data-ttu-id="d1765-928">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="d1765-928">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-929">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-929">ACS</span></span>

* <span data-ttu-id="d1765-930">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d1765-930">Corrected preview regions</span></span>
* <span data-ttu-id="d1765-931">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="d1765-931">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="d1765-932">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="d1765-932">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-933">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-933">Appservice</span></span>

* <span data-ttu-id="d1765-934">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="d1765-934">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="d1765-935">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="d1765-935">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="d1765-936">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="d1765-936">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="d1765-937">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="d1765-937">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="d1765-938">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="d1765-938">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="d1765-939">IoT</span><span class="sxs-lookup"><span data-stu-id="d1765-939">IoT</span></span>

* <span data-ttu-id="d1765-940">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="d1765-940">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="d1765-941">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-941">Network</span></span>

* <span data-ttu-id="d1765-942">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d1765-942">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d1765-943">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1765-943">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="d1765-944">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="d1765-944">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d1765-945">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-945">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d1765-946">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-946">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-947">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-947">Profile</span></span>

* <span data-ttu-id="d1765-948">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="d1765-948">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d1765-949">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1765-949">Service Fabric</span></span>

* <span data-ttu-id="d1765-950">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d1765-950">Preview release</span></span>
* <span data-ttu-id="d1765-951">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="d1765-951">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="d1765-952">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="d1765-952">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="d1765-953">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="d1765-953">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-954">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-954">Storage</span></span>

* <span data-ttu-id="d1765-955">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="d1765-955">Enabled setting blob tier</span></span>
* <span data-ttu-id="d1765-956">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="d1765-956">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="d1765-957">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="d1765-957">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="d1765-958">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="d1765-958">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="d1765-959">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="d1765-959">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="d1765-960">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="d1765-960">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-961">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-961">VM</span></span>

* <span data-ttu-id="d1765-962">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="d1765-962">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="d1765-963">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-963">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="d1765-964">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-964">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="d1765-965">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="d1765-965">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="d1765-966">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="d1765-966">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="d1765-967">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-967">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="d1765-968">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-968">August 15, 2017</span></span>

<span data-ttu-id="d1765-969">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="d1765-969">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-970">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-970">ACS</span></span>

* <span data-ttu-id="d1765-971">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d1765-971">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-972">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-972">Appservice</span></span>

* <span data-ttu-id="d1765-973">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="d1765-973">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="d1765-974">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d1765-974">Event Grid</span></span>

* <span data-ttu-id="d1765-975">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="d1765-975">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="d1765-976">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-976">August 11, 2017</span></span>

<span data-ttu-id="d1765-977">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="d1765-977">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-978">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-978">ACS</span></span>

* <span data-ttu-id="d1765-979">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d1765-979">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="d1765-980">Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-980">Batch</span></span>

* <span data-ttu-id="d1765-981">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="d1765-981">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="d1765-982">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="d1765-982">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="d1765-983">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="d1765-983">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="d1765-984">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="d1765-984">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="d1765-985">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="d1765-985">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="d1765-986">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="d1765-986">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="d1765-987">Componente</span><span class="sxs-lookup"><span data-stu-id="d1765-987">Component</span></span>

* <span data-ttu-id="d1765-988">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="d1765-988">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="d1765-989">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d1765-989">Container</span></span>

* <span data-ttu-id="d1765-990">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="d1765-990">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="d1765-991">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1765-991">Data Lake Store</span></span>

* <span data-ttu-id="d1765-992">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="d1765-992">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="d1765-993">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d1765-993">Event Grid</span></span>

* <span data-ttu-id="d1765-994">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d1765-994">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="d1765-995">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-995">Network</span></span>

* <span data-ttu-id="d1765-996">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="d1765-996">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="d1765-997">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="d1765-997">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="d1765-998">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="d1765-998">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="d1765-999">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="d1765-999">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-1000">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-1000">Profile</span></span>

* <span data-ttu-id="d1765-1001">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="d1765-1001">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-1002">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-1002">Storage</span></span>

* <span data-ttu-id="d1765-1003">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="d1765-1003">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-1004">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-1004">VM</span></span>

* <span data-ttu-id="d1765-1005">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="d1765-1005">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="d1765-1006">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1006">Exposed `list-skus` command</span></span>
* <span data-ttu-id="d1765-1007">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="d1765-1007">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="d1765-1008">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="d1765-1008">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="d1765-1009">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="d1765-1009">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="d1765-1010">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-1010">July 28, 2017</span></span>

<span data-ttu-id="d1765-1011">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="d1765-1011">Version 2.0.12</span></span>

* <span data-ttu-id="d1765-1012">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="d1765-1012">Added container commands</span></span>
* <span data-ttu-id="d1765-1013">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="d1765-1013">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="d1765-1014">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-1014">Core</span></span>

* <span data-ttu-id="d1765-1015">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="d1765-1015">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="d1765-1016">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="d1765-1016">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="d1765-1017">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="d1765-1017">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="d1765-1018">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="d1765-1018">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="d1765-1019">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="d1765-1019">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="d1765-1020">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="d1765-1020">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="d1765-1021">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="d1765-1021">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d1765-1022">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="d1765-1022">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="d1765-1023">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="d1765-1023">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="d1765-1024">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="d1765-1024">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="d1765-1025">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="d1765-1025">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="d1765-1026">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="d1765-1026">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="d1765-1027">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d1765-1027">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="d1765-1028">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d1765-1028">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="d1765-1029">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d1765-1029">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="d1765-1030">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="d1765-1030">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="d1765-1031">ACR</span><span class="sxs-lookup"><span data-stu-id="d1765-1031">ACR</span></span>

* <span data-ttu-id="d1765-1032">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="d1765-1032">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="d1765-1033">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="d1765-1033">Support SKU update for managed registries</span></span>
* <span data-ttu-id="d1765-1034">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="d1765-1034">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="d1765-1035">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="d1765-1035">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="d1765-1036">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="d1765-1036">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="d1765-1037">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="d1765-1037">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-1038">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-1038">ACS</span></span>

* <span data-ttu-id="d1765-1039">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="d1765-1039">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-1040">Appservice</span><span class="sxs-lookup"><span data-stu-id="d1765-1040">Appservice</span></span>

* <span data-ttu-id="d1765-1041">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="d1765-1041">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="d1765-1042">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="d1765-1042">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="d1765-1043">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1043">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="d1765-1044">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="d1765-1044">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="d1765-1045">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="d1765-1045">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="d1765-1046">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="d1765-1046">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="d1765-1047">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="d1765-1047">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="d1765-1048">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="d1765-1048">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="d1765-1049">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="d1765-1049">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="d1765-1050">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="d1765-1050">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="d1765-1051">Batch</span><span class="sxs-lookup"><span data-stu-id="d1765-1051">Batch</span></span>

* <span data-ttu-id="d1765-1052">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="d1765-1052">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="d1765-1053">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1053">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="d1765-1054">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1054">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="d1765-1055">CDN</span><span class="sxs-lookup"><span data-stu-id="d1765-1055">CDN</span></span>

* <span data-ttu-id="d1765-1056">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="d1765-1056">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="d1765-1057">Nube</span><span class="sxs-lookup"><span data-stu-id="d1765-1057">Cloud</span></span>

* <span data-ttu-id="d1765-1058">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="d1765-1058">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="d1765-1059">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="d1765-1059">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="d1765-1060">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="d1765-1060">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="d1765-1061">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="d1765-1061">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="d1765-1062">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1062">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1765-1063">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1765-1063">CosmosDB</span></span>

* <span data-ttu-id="d1765-1064">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="d1765-1064">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="d1765-1065">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="d1765-1065">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d1765-1066">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1765-1066">Data Lake Analytics</span></span>

* <span data-ttu-id="d1765-1067">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1067">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="d1765-1068">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1068">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="d1765-1069">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1069">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d1765-1070">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1765-1070">Data Lake Store</span></span>

* <span data-ttu-id="d1765-1071">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1071">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="d1765-1072">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="d1765-1072">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="d1765-1073">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1073">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="d1765-1074">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="d1765-1074">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="d1765-1075">Interactive</span><span class="sxs-lookup"><span data-stu-id="d1765-1075">Interactive</span></span>

* <span data-ttu-id="d1765-1076">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="d1765-1076">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="d1765-1077">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="d1765-1077">Increased test coverage</span></span>
* <span data-ttu-id="d1765-1078">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="d1765-1078">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="d1765-1079">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="d1765-1079">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="d1765-1080">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="d1765-1080">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="d1765-1081">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="d1765-1081">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="d1765-1082">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="d1765-1082">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d1765-1083">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1083">Added `--progress` flag</span></span>
* <span data-ttu-id="d1765-1084">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="d1765-1084">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="d1765-1085">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="d1765-1085">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="d1765-1086">IoT</span><span class="sxs-lookup"><span data-stu-id="d1765-1086">IoT</span></span>

* <span data-ttu-id="d1765-1087">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="d1765-1087">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="d1765-1088">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="d1765-1088">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="d1765-1089">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="d1765-1089">Key vault</span></span>

* <span data-ttu-id="d1765-1090">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="d1765-1090">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="d1765-1091">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d1765-1091">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="d1765-1092">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d1765-1092">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d1765-1093">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d1765-1093">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d1765-1094">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d1765-1094">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="d1765-1095">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="d1765-1095">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="d1765-1096">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="d1765-1096">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="d1765-1097">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="d1765-1097">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="d1765-1098">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-1098">Lab</span></span>

* <span data-ttu-id="d1765-1099">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1099">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="d1765-1100">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1100">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-1101">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-1101">Monitor</span></span>

* <span data-ttu-id="d1765-1102">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="d1765-1102">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="d1765-1103">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1103">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="d1765-1104">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1104">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="d1765-1105">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1105">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="d1765-1106">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1106">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="d1765-1107">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="d1765-1107">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="d1765-1108">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="d1765-1108">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="d1765-1109">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="d1765-1109">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="d1765-1110">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="d1765-1110">`location` no longer required</span></span>
  * <span data-ttu-id="d1765-1111">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="d1765-1111">Add name and ID support for target</span></span>
  * <span data-ttu-id="d1765-1112">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1112">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="d1765-1113">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="d1765-1113">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="d1765-1114">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="d1765-1114">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="d1765-1115">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="d1765-1115">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="d1765-1116">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1116">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="d1765-1117">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="d1765-1117">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="d1765-1118">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-1118">Network</span></span>

* <span data-ttu-id="d1765-1119">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1119">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="d1765-1120">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1120">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="d1765-1121">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="d1765-1121">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="d1765-1122">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="d1765-1122">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="d1765-1123">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1123">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="d1765-1124">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1124">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="d1765-1125">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="d1765-1125">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="d1765-1126">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="d1765-1126">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="d1765-1127">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="d1765-1127">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="d1765-1128">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d1765-1128">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="d1765-1129">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="d1765-1129">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="d1765-1130">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1130">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="d1765-1131">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="d1765-1131">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="d1765-1132">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1132">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="d1765-1133">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1133">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="d1765-1134">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1134">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="d1765-1135">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="d1765-1135">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="d1765-1136">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1136">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="d1765-1137">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1137">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="d1765-1138">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1138">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="d1765-1139">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1139">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="d1765-1140">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1140">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="d1765-1141">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1141">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="d1765-1142">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="d1765-1142">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="d1765-1143">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="d1765-1143">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="d1765-1144">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="d1765-1144">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="d1765-1145">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="d1765-1145">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-1146">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-1146">Profile</span></span>

* <span data-ttu-id="d1765-1147">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="d1765-1147">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="d1765-1148">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="d1765-1148">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="d1765-1149">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="d1765-1149">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="d1765-1150">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="d1765-1150">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="d1765-1151">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="d1765-1151">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1765-1152">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1765-1152">RDBMS</span></span>

* <span data-ttu-id="d1765-1153">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="d1765-1153">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="d1765-1154">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="d1765-1154">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="d1765-1155">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="d1765-1155">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="d1765-1156">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="d1765-1156">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-1157">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-1157">Resource</span></span>

* <span data-ttu-id="d1765-1158">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1158">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="d1765-1159">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1159">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="d1765-1160">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1160">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="d1765-1161">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1161">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="d1765-1162">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="d1765-1162">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="d1765-1163">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1163">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="d1765-1164">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="d1765-1164">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="d1765-1165">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1165">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="d1765-1166">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-1166">Role</span></span>

* <span data-ttu-id="d1765-1167">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="d1765-1167">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="d1765-1168">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="d1765-1168">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="d1765-1169">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1169">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="d1765-1170">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1170">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="d1765-1171">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1171">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d1765-1172">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1765-1172">Service Fabric</span></span>
* <span data-ttu-id="d1765-1173">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="d1765-1173">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="d1765-1174">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="d1765-1174">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="d1765-1175">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="d1765-1175">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-1176">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-1176">SQL</span></span>

* <span data-ttu-id="d1765-1177">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="d1765-1177">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="d1765-1178">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1178">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="d1765-1179">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="d1765-1179">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-1180">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-1180">Storage</span></span>

* <span data-ttu-id="d1765-1181">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="d1765-1181">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="d1765-1182">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="d1765-1182">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="d1765-1183">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="d1765-1183">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="d1765-1184">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="d1765-1184">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="d1765-1185">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="d1765-1185">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="d1765-1186">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="d1765-1186">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-1187">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-1187">VM</span></span>

* <span data-ttu-id="d1765-1188">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="d1765-1188">Support configuring nsg</span></span>
* <span data-ttu-id="d1765-1189">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="d1765-1189">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="d1765-1190">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="d1765-1190">Support managed service identities</span></span>
* <span data-ttu-id="d1765-1191">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="d1765-1191">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="d1765-1192">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="d1765-1192">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="d1765-1193">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-1193">May 10, 2017</span></span>

<span data-ttu-id="d1765-1194">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="d1765-1194">Version 2.0.6</span></span>

* <span data-ttu-id="d1765-1195">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="d1765-1195">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="d1765-1196">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="d1765-1196">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="d1765-1197">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1765-1197">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="d1765-1198">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d1765-1198">Include Cognitive Services module</span></span>
* <span data-ttu-id="d1765-1199">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1765-1199">Include Service Fabric module</span></span>
* <span data-ttu-id="d1765-1200">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="d1765-1200">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="d1765-1201">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="d1765-1201">Add support for CDN commands</span></span>
* <span data-ttu-id="d1765-1202">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="d1765-1202">Remove Container module</span></span>
* <span data-ttu-id="d1765-1203">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="d1765-1203">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="d1765-1204">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="d1765-1204">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="d1765-1205">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-1205">Core</span></span>

* <span data-ttu-id="d1765-1206">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="d1765-1206">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="d1765-1207">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="d1765-1207">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="d1765-1208">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="d1765-1208">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="d1765-1209">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="d1765-1209">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="d1765-1210">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="d1765-1210">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="d1765-1211">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="d1765-1211">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="d1765-1212">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="d1765-1212">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="d1765-1213">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="d1765-1213">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="d1765-1214">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="d1765-1214">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="d1765-1215">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="d1765-1215">core: Improved performance</span></span>
* <span data-ttu-id="d1765-1216">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="d1765-1216">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="d1765-1217">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="d1765-1217">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-1218">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-1218">ACS</span></span>

* <span data-ttu-id="d1765-1219">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="d1765-1219">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="d1765-1220">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="d1765-1220">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="d1765-1221">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="d1765-1221">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="d1765-1222">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="d1765-1222">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-1223">AppService</span><span class="sxs-lookup"><span data-stu-id="d1765-1223">AppService</span></span>

* <span data-ttu-id="d1765-1224">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="d1765-1224">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="d1765-1225">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="d1765-1225">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="d1765-1226">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="d1765-1226">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="d1765-1227">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="d1765-1227">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="d1765-1228">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="d1765-1228">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="d1765-1229">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="d1765-1229">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="d1765-1230">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d1765-1230">support slot swap with preview</span></span>
* <span data-ttu-id="d1765-1231">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="d1765-1231">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="d1765-1232">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="d1765-1232">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1765-1233">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1765-1233">CosmosDB</span></span>

* <span data-ttu-id="d1765-1234">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1765-1234">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="d1765-1235">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="d1765-1235">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="d1765-1236">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="d1765-1236">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="d1765-1237">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="d1765-1237">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d1765-1238">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1765-1238">Data Lake Analytics</span></span>

* <span data-ttu-id="d1765-1239">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="d1765-1239">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="d1765-1240">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="d1765-1240">Add support for new catalog item type: package.</span></span> <span data-ttu-id="d1765-1241">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="d1765-1241">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="d1765-1242">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="d1765-1242">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="d1765-1243">Tabla</span><span class="sxs-lookup"><span data-stu-id="d1765-1243">Table</span></span>
  * <span data-ttu-id="d1765-1244">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="d1765-1244">Table valued function</span></span>
  * <span data-ttu-id="d1765-1245">Ver</span><span class="sxs-lookup"><span data-stu-id="d1765-1245">View</span></span>
  * <span data-ttu-id="d1765-1246">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="d1765-1246">Table Statistics.</span></span> <span data-ttu-id="d1765-1247">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="d1765-1247">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d1765-1248">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1765-1248">Data Lake Store</span></span>

* <span data-ttu-id="d1765-1249">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="d1765-1249">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="d1765-1250">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="d1765-1250">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="d1765-1251">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="d1765-1251">missed help for access show.</span></span> <span data-ttu-id="d1765-1252">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="d1765-1252">adding it.</span></span> <span data-ttu-id="d1765-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="d1765-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="d1765-1254">Buscar</span><span class="sxs-lookup"><span data-stu-id="d1765-1254">Find</span></span>

* <span data-ttu-id="d1765-1255">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="d1765-1255">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1765-1256">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d1765-1256">KeyVault</span></span>

* <span data-ttu-id="d1765-1257">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="d1765-1257">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="d1765-1258">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="d1765-1258">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="d1765-1259">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="d1765-1259">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="d1765-1260">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="d1765-1260">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="d1765-1261">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="d1765-1261">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="d1765-1262">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-1262">Lab</span></span>

* <span data-ttu-id="d1765-1263">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-1263">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="d1765-1264">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-1264">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="d1765-1265">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-1265">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="d1765-1266">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-1266">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="d1765-1267">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="d1765-1267">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="d1765-1268">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d1765-1268">Monitor</span></span>

* <span data-ttu-id="d1765-1269">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="d1765-1269">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="d1765-1270">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="d1765-1270">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="d1765-1271">Red</span><span class="sxs-lookup"><span data-stu-id="d1765-1271">Network</span></span>

* <span data-ttu-id="d1765-1272">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="d1765-1272">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="d1765-1273">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="d1765-1273">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="d1765-1274">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="d1765-1274">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="d1765-1275">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="d1765-1275">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="d1765-1276">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="d1765-1276">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="d1765-1277">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d1765-1277">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="d1765-1278">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="d1765-1278">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="d1765-1279">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="d1765-1279">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="d1765-1280">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="d1765-1280">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="d1765-1281">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="d1765-1281">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="d1765-1282">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="d1765-1282">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="d1765-1283">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d1765-1283">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="d1765-1284">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="d1765-1284">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="d1765-1285">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="d1765-1285">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="d1765-1286">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="d1765-1286">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="d1765-1287">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="d1765-1287">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="d1765-1288">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1765-1288">Profile</span></span>

* <span data-ttu-id="d1765-1289">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="d1765-1289">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="d1765-1290">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="d1765-1290">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="d1765-1291">Redis</span><span class="sxs-lookup"><span data-stu-id="d1765-1291">Redis</span></span>

* <span data-ttu-id="d1765-1292">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="d1765-1292">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="d1765-1293">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="d1765-1293">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="d1765-1294">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1765-1294">Resource</span></span>

* <span data-ttu-id="d1765-1295">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="d1765-1295">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="d1765-1296">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="d1765-1296">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="d1765-1297">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="d1765-1297">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="d1765-1298">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="d1765-1298">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="d1765-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="d1765-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="d1765-1300">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="d1765-1300">Add docs for az lock update.</span></span> <span data-ttu-id="d1765-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="d1765-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="d1765-1302">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="d1765-1302">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="d1765-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="d1765-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="d1765-1304">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="d1765-1304">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="d1765-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="d1765-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="d1765-1306">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="d1765-1306">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="d1765-1307">Rol</span><span class="sxs-lookup"><span data-stu-id="d1765-1307">Role</span></span>

* <span data-ttu-id="d1765-1308">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="d1765-1308">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="d1765-1309">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="d1765-1309">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="d1765-1310">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="d1765-1310">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="d1765-1311">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="d1765-1311">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="d1765-1312">SQL</span><span class="sxs-lookup"><span data-stu-id="d1765-1312">SQL</span></span>

* <span data-ttu-id="d1765-1313">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="d1765-1313">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="d1765-1314">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="d1765-1314">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="d1765-1315">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-1315">Storage</span></span>

* <span data-ttu-id="d1765-1316">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="d1765-1316">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="d1765-1317">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="d1765-1317">Add support for incremental blob copy</span></span>
* <span data-ttu-id="d1765-1318">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="d1765-1318">Add support for large block blob upload</span></span>
* <span data-ttu-id="d1765-1319">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="d1765-1319">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-1320">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-1320">VM</span></span>

* <span data-ttu-id="d1765-1321">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="d1765-1321">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="d1765-1322">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="d1765-1322">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="d1765-1323">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="d1765-1323">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="d1765-1324">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="d1765-1324">az vm/vmss disk</span></span>
  3. <span data-ttu-id="d1765-1325">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="d1765-1325">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="d1765-1326">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="d1765-1326">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="d1765-1327">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="d1765-1327">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="d1765-1328">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-1328">April 3, 2017</span></span>

<span data-ttu-id="d1765-1329">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="d1765-1329">Version 2.0.2</span></span>

<span data-ttu-id="d1765-1330">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="d1765-1330">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="d1765-1331">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1765-1331">Core</span></span>

* <span data-ttu-id="d1765-1332">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="d1765-1332">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="d1765-1333">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="d1765-1333">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="d1765-1334">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="d1765-1334">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="d1765-1335">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d1765-1335">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d1765-1336">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="d1765-1336">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="d1765-1337">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="d1765-1337">Add prompting for missing template parameters.</span></span> <span data-ttu-id="d1765-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="d1765-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="d1765-1339">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="d1765-1339">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="d1765-1340">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="d1765-1340">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="d1765-1341">ACS</span><span class="sxs-lookup"><span data-stu-id="d1765-1341">ACS</span></span>

* <span data-ttu-id="d1765-1342">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="d1765-1342">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="d1765-1343">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="d1765-1343">Add support for ssh key password prompting.</span></span> <span data-ttu-id="d1765-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="d1765-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="d1765-1345">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="d1765-1345">Add support for windows clusters.</span></span> <span data-ttu-id="d1765-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="d1765-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="d1765-1347">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="d1765-1347">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="d1765-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="d1765-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="d1765-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="d1765-1349">AppService</span></span>

* <span data-ttu-id="d1765-1350">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="d1765-1350">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="d1765-1351">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="d1765-1351">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="d1765-1352">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="d1765-1352">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="d1765-1353">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="d1765-1353">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="d1765-1354">DataLake</span><span class="sxs-lookup"><span data-stu-id="d1765-1354">DataLake</span></span>

* <span data-ttu-id="d1765-1355">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1765-1355">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="d1765-1356">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1765-1356">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="d1765-1357">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="d1765-1357">DocuemntDB</span></span>

* <span data-ttu-id="d1765-1358">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="d1765-1358">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="d1765-1359">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1765-1359">VM</span></span>

* <span data-ttu-id="d1765-1360">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="d1765-1360">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="d1765-1361">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="d1765-1361">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="d1765-1362">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="d1765-1362">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="d1765-1363">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d1765-1363">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d1765-1364">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="d1765-1364">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="d1765-1365">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="d1765-1365">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="d1765-1366">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="d1765-1366">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="d1765-1367">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="d1765-1367">February 27, 2017</span></span>

<span data-ttu-id="d1765-1368">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d1765-1368">Version 2.0.0</span></span>

<span data-ttu-id="d1765-1369">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="d1765-1369">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="d1765-1370">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="d1765-1370">Container Service (acs)</span></span>
- <span data-ttu-id="d1765-1371">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="d1765-1371">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="d1765-1372">Redes</span><span class="sxs-lookup"><span data-stu-id="d1765-1372">Networking</span></span>
- <span data-ttu-id="d1765-1373">Storage</span><span class="sxs-lookup"><span data-stu-id="d1765-1373">Storage</span></span>

<span data-ttu-id="d1765-1374">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d1765-1374">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="d1765-1375">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="d1765-1375">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="d1765-1376">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="d1765-1376">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="d1765-1377">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="d1765-1377">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="d1765-1378">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="d1765-1378">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="d1765-1379">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="d1765-1379">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="d1765-1380">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="d1765-1380">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="d1765-1381">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="d1765-1381">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="d1765-1382">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d1765-1382">Provide feedback from the command line with the `az feedback` command</span></span>

