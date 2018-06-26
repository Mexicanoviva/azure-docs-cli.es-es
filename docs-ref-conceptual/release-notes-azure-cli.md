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
ms.openlocfilehash: 64db2b58ca883518757d8e189bf7263ed818b283
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262665"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="a0667-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="a0667-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="a0667-104">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-104">June 19, 2018</span></span>

<span data-ttu-id="a0667-105">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="a0667-105">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="a0667-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-106">Core</span></span>

* <span data-ttu-id="a0667-107">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-107">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-108">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-108">ACR</span></span>

* <span data-ttu-id="a0667-109">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="a0667-109">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="a0667-110">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="a0667-110">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-111">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-111">ACS</span></span>

* <span data-ttu-id="a0667-112">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a0667-112">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="a0667-113">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="a0667-113">Added `--update` support</span></span>
* <span data-ttu-id="a0667-114">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="a0667-114">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="a0667-115">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="a0667-115">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="a0667-116">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="a0667-116">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="a0667-117">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="a0667-117">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="a0667-118">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="a0667-118">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="a0667-119">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="a0667-119">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span> 

### <a name="appservice"></a><span data-ttu-id="a0667-120">AppService</span><span class="sxs-lookup"><span data-stu-id="a0667-120">AppService</span></span>

* <span data-ttu-id="a0667-121">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="a0667-121">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="a0667-122">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="a0667-122">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="a0667-123">Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-123">Batch</span></span>

* <span data-ttu-id="a0667-124">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="a0667-124">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a0667-125">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0667-125">Batch AI</span></span>

* <span data-ttu-id="a0667-126">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="a0667-126">Added support for workspaces.</span></span> <span data-ttu-id="a0667-127">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="a0667-127">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="a0667-128">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="a0667-128">Added support for experiments.</span></span> <span data-ttu-id="a0667-129">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="a0667-129">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="a0667-130">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="a0667-130">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="a0667-131">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="a0667-131">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="a0667-132">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="a0667-132">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="a0667-133">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="a0667-133">Added support for `--ids` to `batchai` commands</span></span> 
* <span data-ttu-id="a0667-134">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="a0667-134">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="a0667-135">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="a0667-135">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="a0667-136">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-136">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="a0667-137">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="a0667-137">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="a0667-138">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-138">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="a0667-139">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="a0667-139">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="a0667-140">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="a0667-140">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="a0667-141">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="a0667-141">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="a0667-142">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-142">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="a0667-143">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="a0667-143">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="a0667-144">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="a0667-144">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="a0667-145">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a0667-145">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="a0667-146">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a0667-146">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="a0667-147">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="a0667-147">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="a0667-148">Mapas</span><span class="sxs-lookup"><span data-stu-id="a0667-148">Maps</span></span>

* <span data-ttu-id="a0667-149">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="a0667-149">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="a0667-150">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-150">Network</span></span>

* <span data-ttu-id="a0667-151">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="a0667-151">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="a0667-152">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a0667-152">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="a0667-153">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="a0667-153">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="a0667-154">Reservations</span><span class="sxs-lookup"><span data-stu-id="a0667-154">Reservations</span></span>

* <span data-ttu-id="a0667-155">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="a0667-155">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="a0667-156">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="a0667-156">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="a0667-157">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="a0667-157">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="a0667-158">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="a0667-158">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="a0667-159">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="a0667-159">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="a0667-160">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-160">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="a0667-161">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-161">Role</span></span>

* <span data-ttu-id="a0667-162">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="a0667-162">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-163">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-163">SQL</span></span>

* <span data-ttu-id="a0667-164">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="a0667-164">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-165">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-165">Storage</span></span>

* <span data-ttu-id="a0667-166">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="a0667-166">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-167">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-167">VM</span></span>

* <span data-ttu-id="a0667-168">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="a0667-168">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="a0667-169">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="a0667-169">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="a0667-170">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="a0667-170">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a0667-171">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-171">June 13, 2018</span></span>

<span data-ttu-id="a0667-172">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="a0667-172">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="a0667-173">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-173">Core</span></span>

* <span data-ttu-id="a0667-174">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="a0667-174">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a0667-175">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-175">June 13, 2018</span></span>

<span data-ttu-id="a0667-176">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a0667-176">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a0667-177">AKS</span><span class="sxs-lookup"><span data-stu-id="a0667-177">AKS</span></span>

* <span data-ttu-id="a0667-178">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="a0667-178">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="a0667-179">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="a0667-179">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="a0667-180">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="a0667-180">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="a0667-181">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="a0667-181">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="a0667-182">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="a0667-182">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-183">AppService</span><span class="sxs-lookup"><span data-stu-id="a0667-183">AppService</span></span>

* <span data-ttu-id="a0667-184">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="a0667-184">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a0667-185">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-185">June 5, 2018</span></span>

<span data-ttu-id="a0667-186">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a0667-186">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-187">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-187">Interactive</span></span>

* <span data-ttu-id="a0667-188">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="a0667-188">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a0667-189">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-189">June 5, 2018</span></span>

<span data-ttu-id="a0667-190">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a0667-190">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a0667-191">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-191">Core</span></span>

* <span data-ttu-id="a0667-192">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="a0667-192">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a0667-193">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="a0667-193">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-194">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-194">ACR</span></span>

* <span data-ttu-id="a0667-195">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="a0667-195">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a0667-196">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="a0667-196">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a0667-197">AKS</span><span class="sxs-lookup"><span data-stu-id="a0667-197">AKS</span></span>

* <span data-ttu-id="a0667-198">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="a0667-198">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a0667-199">Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-199">Batch</span></span>

* <span data-ttu-id="a0667-200">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a0667-200">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a0667-201">IoT</span><span class="sxs-lookup"><span data-stu-id="a0667-201">IOT</span></span>

* <span data-ttu-id="a0667-202">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="a0667-202">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a0667-203">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-203">Network</span></span>

* <span data-ttu-id="a0667-204">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="a0667-204">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a0667-205">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="a0667-205">Policy Insights</span></span>

* <span data-ttu-id="a0667-206">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="a0667-206">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a0667-207">ARM</span><span class="sxs-lookup"><span data-stu-id="a0667-207">ARM</span></span>

* <span data-ttu-id="a0667-208">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="a0667-208">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-209">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-209">SQL</span></span>

* <span data-ttu-id="a0667-210">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="a0667-210">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a0667-211">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="a0667-211">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a0667-212">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-212">Storage</span></span>

* <span data-ttu-id="a0667-213">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="a0667-213">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-214">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-214">VM</span></span>

* <span data-ttu-id="a0667-215">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="a0667-215">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a0667-216">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="a0667-216">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="a0667-217">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="a0667-217">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="a0667-218">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-218">May 22, 2018</span></span>

<span data-ttu-id="a0667-219">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a0667-219">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a0667-220">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-220">Core</span></span>

* <span data-ttu-id="a0667-221">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="a0667-221">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-222">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-222">ACS</span></span>

* <span data-ttu-id="a0667-223">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="a0667-223">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="a0667-224">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="a0667-224">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-225">AppService</span><span class="sxs-lookup"><span data-stu-id="a0667-225">AppService</span></span>

* <span data-ttu-id="a0667-226">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="a0667-226">Improved generic update commands</span></span>
* <span data-ttu-id="a0667-227">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="a0667-227">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="a0667-228">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-228">Container</span></span>

* <span data-ttu-id="a0667-229">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="a0667-229">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a0667-230">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="a0667-230">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-231">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-231">Extension</span></span>

* <span data-ttu-id="a0667-232">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="a0667-232">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-233">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-233">Interactive</span></span>

* <span data-ttu-id="a0667-234">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="a0667-234">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a0667-235">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="a0667-235">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0667-236">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0667-236">KeyVault</span></span>

* <span data-ttu-id="a0667-237">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="a0667-237">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a0667-238">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-238">Network</span></span>

* <span data-ttu-id="a0667-239">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a0667-239">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a0667-240">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a0667-240">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-241">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-241">SQL</span></span>

* <span data-ttu-id="a0667-242">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="a0667-242">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a0667-243">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="a0667-243">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="a0667-244">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="a0667-244">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="a0667-245">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="a0667-245">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a0667-246">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="a0667-246">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="a0667-247">(Unión permanente)(Unión permanente).</span><span class="sxs-lookup"><span data-stu-id="a0667-247">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="a0667-248">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="a0667-248">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="a0667-249">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a0667-249">`edition`.</span></span> <span data-ttu-id="a0667-250">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="a0667-250">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="a0667-251">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="a0667-251">`elasticPoolName`.</span></span> <span data-ttu-id="a0667-252">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="a0667-252">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a0667-253">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="a0667-253">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="a0667-254">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a0667-254">`edition`.</span></span> <span data-ttu-id="a0667-255">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="a0667-255">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="a0667-256">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="a0667-256">`dtu`.</span></span> <span data-ttu-id="a0667-257">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="a0667-257">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="a0667-258">(Unión permanente)(Unión permanente).</span><span class="sxs-lookup"><span data-stu-id="a0667-258">`databaseDtuMin`.</span></span> <span data-ttu-id="a0667-259">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="a0667-259">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="a0667-260">(Unión permanente)(Unión permanente).</span><span class="sxs-lookup"><span data-stu-id="a0667-260">`databaseDtuMax`.</span></span> <span data-ttu-id="a0667-261">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="a0667-261">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a0667-262">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a0667-262">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a0667-263">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a0667-263">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-264">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-264">Storage</span></span>

* <span data-ttu-id="a0667-265">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="a0667-265">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a0667-266">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="a0667-266">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-267">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-267">VM</span></span>

* <span data-ttu-id="a0667-268">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-268">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a0667-269">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="a0667-269">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="a0667-270">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="a0667-270">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="a0667-271">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="a0667-271">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a0667-272">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="a0667-272">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="a0667-273">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-273">May 7, 2018</span></span>

<span data-ttu-id="a0667-274">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a0667-274">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a0667-275">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-275">Core</span></span>

* <span data-ttu-id="a0667-276">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="a0667-276">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a0667-277">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="a0667-277">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a0667-278">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a0667-278">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a0667-279">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="a0667-279">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a0667-280">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a0667-280">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a0667-281">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="a0667-281">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a0667-282">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-282">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a0667-283">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="a0667-283">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="a0667-284">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-284">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-285">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-285">ACR</span></span>

* <span data-ttu-id="a0667-286">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="a0667-286">Added ACR Build commands</span></span>
* <span data-ttu-id="a0667-287">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="a0667-287">Improved resource not found error messages</span></span>
* <span data-ttu-id="a0667-288">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="a0667-288">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a0667-289">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="a0667-289">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a0667-290">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="a0667-290">Improved repository commands error messages</span></span>
* <span data-ttu-id="a0667-291">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="a0667-291">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-292">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-292">ACS</span></span>

* <span data-ttu-id="a0667-293">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="a0667-293">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a0667-294">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="a0667-294">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a0667-295">AMS</span><span class="sxs-lookup"><span data-stu-id="a0667-295">AMS</span></span>

* <span data-ttu-id="a0667-296">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="a0667-296">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-297">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-297">Appservice</span></span>

* <span data-ttu-id="a0667-298">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="a0667-298">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a0667-299">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="a0667-299">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="a0667-300">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="a0667-300">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a0667-301">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="a0667-301">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a0667-302">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0667-302">Batch AI</span></span>

* <span data-ttu-id="a0667-303">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="a0667-303">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a0667-304">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0667-304">Cognitive Services</span></span>

* <span data-ttu-id="a0667-305">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="a0667-305">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a0667-306">Consumo</span><span class="sxs-lookup"><span data-stu-id="a0667-306">Consumption</span></span>

* <span data-ttu-id="a0667-307">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="a0667-307">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a0667-308">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-308">Container</span></span>

* <span data-ttu-id="a0667-309">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="a0667-309">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a0667-310">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a0667-310">Cosmos DB</span></span>

* <span data-ttu-id="a0667-311">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a0667-311">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a0667-312">DMS</span><span class="sxs-lookup"><span data-stu-id="a0667-312">DMS</span></span>

* <span data-ttu-id="a0667-313">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-313">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-314">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-314">Extension</span></span>

* <span data-ttu-id="a0667-315">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="a0667-315">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-316">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-316">Interactive</span></span>

* <span data-ttu-id="a0667-317">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="a0667-317">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a0667-318">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="a0667-318">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a0667-319">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="a0667-319">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a0667-320">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-320">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a0667-321">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-321">Lab</span></span>

* <span data-ttu-id="a0667-322">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="a0667-322">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a0667-323">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-323">Network</span></span>

* <span data-ttu-id="a0667-324">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="a0667-324">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a0667-325">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-325">Profile</span></span>

* <span data-ttu-id="a0667-326">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="a0667-326">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a0667-327">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="a0667-327">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a0667-328">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="a0667-328">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a0667-329">Redis</span><span class="sxs-lookup"><span data-stu-id="a0667-329">Redis</span></span>

* <span data-ttu-id="a0667-330">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="a0667-330">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="a0667-331">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="a0667-331">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a0667-332">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="a0667-332">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="a0667-333">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="a0667-333">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="a0667-334">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-334">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a0667-335">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-335">Role</span></span>

* <span data-ttu-id="a0667-336">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="a0667-336">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-337">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-337">Storage</span></span>

* <span data-ttu-id="a0667-338">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="a0667-338">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a0667-339">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="a0667-339">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a0667-340">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="a0667-340">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a0667-341">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="a0667-341">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a0667-342">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="a0667-342">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-343">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-343">VM</span></span>

* <span data-ttu-id="a0667-344">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="a0667-344">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a0667-345">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="a0667-345">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a0667-346">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="a0667-346">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a0667-347">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="a0667-347">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="a0667-348">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="a0667-348">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a0667-349">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="a0667-349">Added write accelerator support</span></span> 
* <span data-ttu-id="a0667-350">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="a0667-350">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="a0667-351">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="a0667-351">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a0667-352">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="a0667-352">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a0667-353">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-353">April 10, 2018</span></span>

<span data-ttu-id="a0667-354">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a0667-354">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-355">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-355">ACR</span></span>

* <span data-ttu-id="a0667-356">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="a0667-356">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-357">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-357">ACS</span></span>

* <span data-ttu-id="a0667-358">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="a0667-358">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-359">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-359">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="a0667-361">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="a0667-361">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a0667-362">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a0667-362">BatchAI</span></span>

* <span data-ttu-id="a0667-363">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="a0667-363">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="a0667-364">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="a0667-364">Job level mounting</span></span>
 - <span data-ttu-id="a0667-365">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="a0667-365">Environment variables with secret values</span></span>
 - <span data-ttu-id="a0667-366">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="a0667-366">Performance counters settings</span></span>
 - <span data-ttu-id="a0667-367">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="a0667-367">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="a0667-368">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="a0667-368">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="a0667-369">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="a0667-369">Usage and limits reporting</span></span>
 - <span data-ttu-id="a0667-370">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="a0667-370">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="a0667-371">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="a0667-371">Support for custom images</span></span>
 - <span data-ttu-id="a0667-372">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="a0667-372">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a0667-373">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="a0667-373">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a0667-374">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="a0667-374">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a0667-375">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="a0667-375">National clouds are supported</span></span>
* <span data-ttu-id="a0667-376">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="a0667-376">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a0667-377">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="a0667-377">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a0667-378">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0667-378">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a0667-379">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="a0667-379">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a0667-380">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="a0667-380">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a0667-381">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="a0667-381">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a0667-382">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="a0667-382">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a0667-383">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="a0667-383">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a0667-384">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="a0667-384">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a0667-385">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a0667-385">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="a0667-386">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-386">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a0667-387">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="a0667-387">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a0667-388">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a0667-388">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a0667-389">Facturación</span><span class="sxs-lookup"><span data-stu-id="a0667-389">Billing</span></span>

* <span data-ttu-id="a0667-390">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="a0667-390">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a0667-391">Consumo</span><span class="sxs-lookup"><span data-stu-id="a0667-391">Consumption</span></span>

* <span data-ttu-id="a0667-392">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="a0667-392">Added `marketplace` commands</span></span>
* <span data-ttu-id="a0667-393">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a0667-393">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="a0667-394">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="a0667-394">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="a0667-395">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="a0667-395">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a0667-396">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a0667-396">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a0667-397">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="a0667-397">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a0667-398">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-398">Container</span></span>

* <span data-ttu-id="a0667-399">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="a0667-399">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="a0667-400">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="a0667-400">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-401">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-401">Extension</span></span>

* <span data-ttu-id="a0667-402">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="a0667-402">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-403">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-403">Interactive</span></span>

* <span data-ttu-id="a0667-404">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="a0667-404">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a0667-405">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-405">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a0667-406">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="a0667-406">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a0667-407">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-407">Network</span></span>

* <span data-ttu-id="a0667-408">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="a0667-408">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a0667-409">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a0667-409">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="a0667-410">4910</span><span class="sxs-lookup"><span data-stu-id="a0667-410">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="a0667-411">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="a0667-411">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="a0667-412">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="a0667-412">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a0667-413">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-413">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="a0667-414">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-414">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="a0667-415">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="a0667-415">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-416">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-416">Profile</span></span>

* <span data-ttu-id="a0667-417">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="a0667-417">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="a0667-418">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="a0667-418">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0667-419">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a0667-419">RDBMS</span></span>

* <span data-ttu-id="a0667-420">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="a0667-420">Added `georestore` command</span></span>
* <span data-ttu-id="a0667-421">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="a0667-421">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-422">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-422">Resource</span></span>

* <span data-ttu-id="a0667-423">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-423">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="a0667-424">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="a0667-424">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-425">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-425">SQL</span></span>

* <span data-ttu-id="a0667-426">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="a0667-426">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-427">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-427">Storage</span></span>

* <span data-ttu-id="a0667-428">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="a0667-428">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-429">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-429">VM</span></span>

* <span data-ttu-id="a0667-430">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a0667-430">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="a0667-431">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="a0667-431">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="a0667-433">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="a0667-433">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="a0667-434">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="a0667-434">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="a0667-435">5718</span><span class="sxs-lookup"><span data-stu-id="a0667-435">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="a0667-436">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="a0667-436">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a0667-437">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-437">March 27, 2018</span></span>

<span data-ttu-id="a0667-438">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a0667-438">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a0667-439">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-439">Core</span></span>

* <span data-ttu-id="a0667-440">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="a0667-440">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-441">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-441">ACS</span></span>

* <span data-ttu-id="a0667-442">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a0667-442">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-443">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-443">Appservice</span></span>

* <span data-ttu-id="a0667-444">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="a0667-444">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="a0667-445">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="a0667-445">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a0667-446">Backup</span><span class="sxs-lookup"><span data-stu-id="a0667-446">Backup</span></span>

* <span data-ttu-id="a0667-447">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="a0667-447">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a0667-448">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-448">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a0667-449">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="a0667-449">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a0667-450">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="a0667-450">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a0667-451">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-451">Container</span></span>

* <span data-ttu-id="a0667-452">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="a0667-452">Added `container exec` command.</span></span> <span data-ttu-id="a0667-453">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="a0667-453">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a0667-454">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="a0667-454">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-455">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-455">Extension</span></span>

* <span data-ttu-id="a0667-456">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="a0667-456">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a0667-457">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="a0667-457">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="a0667-458">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="a0667-458">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-459">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-459">Interactive</span></span>

* <span data-ttu-id="a0667-460">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-460">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a0667-461">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="a0667-461">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a0667-462">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-462">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a0667-463">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="a0667-463">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a0667-464">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-464">Lab</span></span>

* <span data-ttu-id="a0667-465">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="a0667-465">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-466">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-466">Monitor</span></span>

* <span data-ttu-id="a0667-467">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a0667-467">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a0667-468">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="a0667-468">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a0667-469">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a0667-469">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a0667-470">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-470">Network</span></span>

* <span data-ttu-id="a0667-471">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="a0667-471">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-472">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-472">Profile</span></span>

* <span data-ttu-id="a0667-473">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="a0667-473">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0667-474">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a0667-474">RDBMS</span></span>

* <span data-ttu-id="a0667-475">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a0667-475">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-476">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-476">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a0667-478">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-478">Role</span></span>

* <span data-ttu-id="a0667-479">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="a0667-479">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="a0667-480">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="a0667-480">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a0667-481">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="a0667-481">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="a0667-482">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a0667-482">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a0667-483">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="a0667-483">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-484">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-484">Storage</span></span>

* <span data-ttu-id="a0667-485">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="a0667-485">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a0667-486">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="a0667-486">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-487">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-487">VM</span></span>

* <span data-ttu-id="a0667-488">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="a0667-488">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a0667-489">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="a0667-489">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="a0667-490">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="a0667-490">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a0667-491">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="a0667-491">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a0667-492">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-492">March 13, 2018</span></span>

<span data-ttu-id="a0667-493">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a0667-493">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-494">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-494">ACR</span></span>

* <span data-ttu-id="a0667-495">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="a0667-495">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="a0667-496">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="a0667-496">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a0667-497">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="a0667-497">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-498">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-498">ACS</span></span>

* <span data-ttu-id="a0667-499">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="a0667-499">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a0667-500">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="a0667-500">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a0667-501">Advisor</span><span class="sxs-lookup"><span data-stu-id="a0667-501">Advisor</span></span>

* <span data-ttu-id="a0667-502">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="a0667-502">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="a0667-503">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="a0667-503">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="a0667-504">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="a0667-504">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="a0667-505">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="a0667-505">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="a0667-506">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="a0667-506">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-507">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-507">Appservice</span></span>

* <span data-ttu-id="a0667-508">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="a0667-508">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="a0667-509">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="a0667-509">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a0667-510">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="a0667-510">Eventhubs</span></span>

* <span data-ttu-id="a0667-511">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="a0667-511">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-512">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-512">Extension</span></span>

* <span data-ttu-id="a0667-513">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="a0667-513">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-514">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-514">Interactive</span></span>

* <span data-ttu-id="a0667-515">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="a0667-515">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a0667-516">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="a0667-516">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a0667-517">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="a0667-517">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a0667-518">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="a0667-518">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-519">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-519">Monitor</span></span>

* <span data-ttu-id="a0667-520">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="a0667-520">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a0667-521">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="a0667-521">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a0667-522">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="a0667-522">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a0667-523">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="a0667-523">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a0667-524">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-524">Network</span></span>

* <span data-ttu-id="a0667-525">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="a0667-525">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="a0667-526">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="a0667-526">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a0667-527">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="a0667-527">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a0667-528">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a0667-528">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-529">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-529">Profile</span></span>

* <span data-ttu-id="a0667-530">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="a0667-530">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="a0667-531">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="a0667-531">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0667-532">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a0667-532">RDBMS</span></span>

* <span data-ttu-id="a0667-533">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="a0667-533">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a0667-534">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="a0667-534">Service Bus</span></span>

* <span data-ttu-id="a0667-535">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="a0667-535">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-536">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-536">Storage</span></span>

* <span data-ttu-id="a0667-537">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="a0667-537">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a0667-538">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="a0667-538">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-539">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-539">VM</span></span>

* <span data-ttu-id="a0667-540">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="a0667-540">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a0667-541">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="a0667-541">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="a0667-542">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="a0667-542">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a0667-543">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="a0667-543">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a0667-544">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-544">February 27, 2018</span></span>

<span data-ttu-id="a0667-545">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a0667-545">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a0667-546">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-546">Core</span></span>

* <span data-ttu-id="a0667-547">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="a0667-547">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a0667-548">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="a0667-548">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a0667-549">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="a0667-549">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-550">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-550">ACS</span></span>

* <span data-ttu-id="a0667-551">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="a0667-551">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a0667-552">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="a0667-552">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a0667-553">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="a0667-553">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="a0667-554">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="a0667-554">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-555">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-555">Appservice</span></span>

* <span data-ttu-id="a0667-556">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a0667-556">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a0667-557">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="a0667-557">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a0667-558">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0667-558">Cognitive Services</span></span>

* <span data-ttu-id="a0667-559">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0667-559">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a0667-560">Consumo</span><span class="sxs-lookup"><span data-stu-id="a0667-560">Consumption</span></span>

* <span data-ttu-id="a0667-561">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="a0667-561">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a0667-562">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="a0667-562">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a0667-563">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-563">Container</span></span>

* <span data-ttu-id="a0667-564">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="a0667-564">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a0667-565">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-565">Network</span></span>

* <span data-ttu-id="a0667-566">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="a0667-566">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-567">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-567">Resource</span></span>

* <span data-ttu-id="a0667-568">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="a0667-568">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a0667-569">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-569">Role</span></span>

* <span data-ttu-id="a0667-570">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="a0667-570">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-571">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-571">SQL</span></span>

* <span data-ttu-id="a0667-572">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="a0667-572">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-573">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-573">Storage</span></span>

* <span data-ttu-id="a0667-574">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="a0667-574">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-575">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-575">VM</span></span>

* <span data-ttu-id="a0667-576">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="a0667-576">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a0667-577">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-577">February 13, 2018</span></span>

<span data-ttu-id="a0667-578">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a0667-578">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a0667-579">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-579">Core</span></span>

* <span data-ttu-id="a0667-580">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="a0667-580">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-581">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-581">ACS</span></span>

* <span data-ttu-id="a0667-582">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="a0667-582">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a0667-583">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="a0667-583">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="a0667-584">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0667-584">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a0667-585">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="a0667-585">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a0667-586">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="a0667-586">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a0667-587">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="a0667-587">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="a0667-588">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0667-588">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a0667-589">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="a0667-589">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-590">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-590">Appservice</span></span>

* <span data-ttu-id="a0667-591">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="a0667-591">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a0667-592">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="a0667-592">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="a0667-593">CDN</span><span class="sxs-lookup"><span data-stu-id="a0667-593">CDN</span></span>

* <span data-ttu-id="a0667-594">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="a0667-594">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a0667-595">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-595">Container</span></span>

* <span data-ttu-id="a0667-596">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="a0667-596">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a0667-597">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="a0667-597">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0667-598">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0667-598">CosmosDB</span></span>

* <span data-ttu-id="a0667-599">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a0667-599">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-600">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-600">Extension</span></span>

* <span data-ttu-id="a0667-601">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-601">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a0667-602">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-602">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a0667-603">Comentarios</span><span class="sxs-lookup"><span data-stu-id="a0667-603">Feedback</span></span>

* <span data-ttu-id="a0667-604">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="a0667-604">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-605">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-605">Interactive</span></span>

* <span data-ttu-id="a0667-606">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a0667-606">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a0667-607">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="a0667-607">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a0667-608">IoT</span><span class="sxs-lookup"><span data-stu-id="a0667-608">IoT</span></span>

* <span data-ttu-id="a0667-609">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="a0667-609">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a0667-610">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="a0667-610">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a0667-611">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-611">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="a0667-612">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="a0667-612">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-613">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-613">Monitor</span></span>

* <span data-ttu-id="a0667-614">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="a0667-614">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a0667-615">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-615">Network</span></span>

* <span data-ttu-id="a0667-616">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="a0667-616">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a0667-617">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-617">Profile</span></span>

* <span data-ttu-id="a0667-618">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="a0667-618">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-619">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-619">Resource</span></span>

* <span data-ttu-id="a0667-620">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="a0667-620">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="a0667-621">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-621">Role</span></span>

* <span data-ttu-id="a0667-622">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="a0667-622">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-623">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-623">SQL</span></span>

* <span data-ttu-id="a0667-624">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="a0667-624">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a0667-625">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="a0667-625">Added `sql db rename`</span></span>
* <span data-ttu-id="a0667-626">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="a0667-626">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-627">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-627">Storage</span></span>

* <span data-ttu-id="a0667-628">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="a0667-628">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-629">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-629">VM</span></span>

* <span data-ttu-id="a0667-630">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="a0667-630">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a0667-631">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="a0667-631">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a0667-632">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="a0667-632">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="a0667-633">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-633">January 31, 2018</span></span>

<span data-ttu-id="a0667-634">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a0667-634">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a0667-635">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-635">Core</span></span>

* <span data-ttu-id="a0667-636">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="a0667-636">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a0667-637">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="a0667-637">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a0667-638">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="a0667-638">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a0667-639">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="a0667-639">Use `--verbose` to see</span></span>
* <span data-ttu-id="a0667-640">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="a0667-640">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-641">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-641">ACS</span></span>

* <span data-ttu-id="a0667-642">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="a0667-642">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a0667-643">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="a0667-643">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-644">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-644">Appservice</span></span>

* <span data-ttu-id="a0667-645">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="a0667-645">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="a0667-646">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="a0667-646">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a0667-647">CDN</span><span class="sxs-lookup"><span data-stu-id="a0667-647">CDN</span></span>

* <span data-ttu-id="a0667-648">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="a0667-648">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0667-649">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0667-649">CosmosDB</span></span>

* <span data-ttu-id="a0667-650">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="a0667-650">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-651">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-651">Interactive</span></span>

* <span data-ttu-id="a0667-652">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="a0667-652">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a0667-653">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-653">Network</span></span>

* <span data-ttu-id="a0667-654">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="a0667-654">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="a0667-655">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="a0667-655">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a0667-656">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="a0667-656">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="a0667-657">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="a0667-657">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="a0667-658">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="a0667-658">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="a0667-659">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="a0667-659">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a0667-660">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="a0667-660">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a0667-661">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="a0667-661">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a0667-662">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="a0667-662">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="a0667-663">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="a0667-663">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-664">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-664">Profile</span></span>

* <span data-ttu-id="a0667-665">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="a0667-665">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-666">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-666">Resource</span></span>

* <span data-ttu-id="a0667-667">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="a0667-667">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-668">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-668">Storage</span></span>

* <span data-ttu-id="a0667-669">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="a0667-669">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a0667-670">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="a0667-670">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a0667-671">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="a0667-671">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="a0667-672">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a0667-672">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="a0667-673">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="a0667-673">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-674">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-674">VM</span></span>

* <span data-ttu-id="a0667-675">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="a0667-675">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a0667-676">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="a0667-676">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a0667-677">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="a0667-677">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a0667-678">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a0667-678">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="a0667-679">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="a0667-679">January 17, 2018</span></span>

<span data-ttu-id="a0667-680">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a0667-680">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-681">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-681">ACR</span></span>

* <span data-ttu-id="a0667-682">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="a0667-682">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a0667-683">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="a0667-683">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-684">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-684">ACS</span></span>

* <span data-ttu-id="a0667-685">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a0667-685">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a0667-686">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="a0667-686">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-687">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-687">Appservice</span></span>

* <span data-ttu-id="a0667-688">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="a0667-688">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a0667-689">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="a0667-689">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="a0667-690">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="a0667-690">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="a0667-691">Backup</span><span class="sxs-lookup"><span data-stu-id="a0667-691">Backup</span></span>

* <span data-ttu-id="a0667-692">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="a0667-692">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a0667-693">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="a0667-693">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="a0667-694">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="a0667-694">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a0667-695">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="a0667-695">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a0667-696">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="a0667-696">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a0667-697">Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-697">Batch</span></span>

* <span data-ttu-id="a0667-698">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="a0667-698">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a0667-699">Nube</span><span class="sxs-lookup"><span data-stu-id="a0667-699">Cloud</span></span>

* <span data-ttu-id="a0667-700">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="a0667-700">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a0667-701">Consumo</span><span class="sxs-lookup"><span data-stu-id="a0667-701">Consumption</span></span>

* <span data-ttu-id="a0667-702">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="a0667-702">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="a0667-703">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a0667-703">Event Grid</span></span>

* <span data-ttu-id="a0667-704">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="a0667-704">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a0667-705">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="a0667-705">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a0667-706">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="a0667-706">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a0667-707">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="a0667-707">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a0667-708">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="a0667-708">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="a0667-709">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="a0667-709">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="a0667-710">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="a0667-710">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a0667-711">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="a0667-711">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-712">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-712">Interactive</span></span>

* <span data-ttu-id="a0667-713">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="a0667-713">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a0667-714">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="a0667-714">Fixed errors on startup</span></span>
* <span data-ttu-id="a0667-715">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="a0667-715">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a0667-716">IoT</span><span class="sxs-lookup"><span data-stu-id="a0667-716">IoT</span></span>

* <span data-ttu-id="a0667-717">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a0667-717">Added support for device provisioning service</span></span>
* <span data-ttu-id="a0667-718">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-718">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a0667-719">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="a0667-719">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-720">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-720">Monitor</span></span>

* <span data-ttu-id="a0667-721">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="a0667-721">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a0667-722">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="a0667-722">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="a0667-723">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="a0667-723">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a0667-724">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-724">Network</span></span>

* <span data-ttu-id="a0667-725">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="a0667-725">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="a0667-726">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-726">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-727">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-727">Profile</span></span>

* <span data-ttu-id="a0667-728">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="a0667-728">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a0667-729">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-729">Role</span></span>

* <span data-ttu-id="a0667-730">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="a0667-730">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a0667-731">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0667-731">Service Fabric</span></span>

* <span data-ttu-id="a0667-732">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="a0667-732">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a0667-733">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="a0667-733">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-734">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-734">VM</span></span>

* <span data-ttu-id="a0667-735">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="a0667-735">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="a0667-736">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="a0667-736">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a0667-737">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="a0667-737">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a0667-738">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="a0667-738">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a0667-739">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="a0667-739">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a0667-740">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a0667-740">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a0667-741">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a0667-741">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="a0667-742">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="a0667-742">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="a0667-743">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-743">December 19, 2017</span></span>

<span data-ttu-id="a0667-744">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a0667-744">Version 2.0.23</span></span>

* <span data-ttu-id="a0667-745">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="a0667-745">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a0667-746">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-746">Container</span></span>

* <span data-ttu-id="a0667-747">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-747">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a0667-748">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-748">Network</span></span>

* <span data-ttu-id="a0667-749">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-749">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="a0667-750">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-750">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-751">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-751">Storage</span></span>

* <span data-ttu-id="a0667-752">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="a0667-752">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-753">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-753">VM</span></span>

* <span data-ttu-id="a0667-754">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="a0667-754">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a0667-755">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-755">December 5, 2017</span></span>

<span data-ttu-id="a0667-756">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a0667-756">Version 2.0.22</span></span>

* <span data-ttu-id="a0667-757">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="a0667-757">Removed `az component` commands.</span></span> <span data-ttu-id="a0667-758">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="a0667-758">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a0667-759">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-759">Core</span></span>
* <span data-ttu-id="a0667-760">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="a0667-760">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a0667-761">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="a0667-761">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-762">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-762">ACS</span></span>

* <span data-ttu-id="a0667-763">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="a0667-763">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a0667-764">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="a0667-764">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="a0667-765">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="a0667-765">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a0667-766">Advisor</span><span class="sxs-lookup"><span data-stu-id="a0667-766">Advisor</span></span>

* <span data-ttu-id="a0667-767">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="a0667-767">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-768">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-768">Appservice</span></span>

* <span data-ttu-id="a0667-769">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="a0667-769">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="a0667-770">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="a0667-770">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a0667-771">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="a0667-771">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="a0667-772">Consumo</span><span class="sxs-lookup"><span data-stu-id="a0667-772">Consumption</span></span>

* <span data-ttu-id="a0667-773">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="a0667-773">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a0667-774">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-774">Container</span></span>

* <span data-ttu-id="a0667-775">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="a0667-775">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-776">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-776">Monitor</span></span>

* <span data-ttu-id="a0667-777">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="a0667-777">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-778">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-778">Resource</span></span>

* <span data-ttu-id="a0667-779">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="a0667-779">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="a0667-780">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-780">Role</span></span>

* <span data-ttu-id="a0667-781">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="a0667-781">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="a0667-782">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="a0667-782">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a0667-783">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="a0667-783">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-784">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-784">SQL</span></span>

* <span data-ttu-id="a0667-785">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="a0667-785">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a0667-786">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="a0667-786">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-787">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-787">VM</span></span>

* <span data-ttu-id="a0667-788">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="a0667-788">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="a0667-789">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-789">November 14, 2017</span></span>

<span data-ttu-id="a0667-790">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a0667-790">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-791">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-791">ACR</span></span>

* <span data-ttu-id="a0667-792">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="a0667-792">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a0667-793">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-793">ACS</span></span>

* <span data-ttu-id="a0667-794">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="a0667-794">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a0667-795">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="a0667-795">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="a0667-796">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="a0667-796">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="a0667-797">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="a0667-797">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a0667-798">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="a0667-798">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-799">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-799">Appservice</span></span>

* <span data-ttu-id="a0667-800">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="a0667-800">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a0667-801">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="a0667-801">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="a0667-802">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="a0667-802">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="a0667-803">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="a0667-803">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="a0667-804">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="a0667-804">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a0667-805">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="a0667-805">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="a0667-806">Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-806">Batch</span></span>

* <span data-ttu-id="a0667-807">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="a0667-807">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a0667-808">Batchai</span><span class="sxs-lookup"><span data-stu-id="a0667-808">Batchai</span></span>

* <span data-ttu-id="a0667-809">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a0667-809">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a0667-810">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a0667-810">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a0667-811">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="a0667-811">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="a0667-812">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="a0667-812">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a0667-813">Nube</span><span class="sxs-lookup"><span data-stu-id="a0667-813">Cloud</span></span>

* <span data-ttu-id="a0667-814">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="a0667-814">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a0667-815">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-815">Container</span></span>

* <span data-ttu-id="a0667-816">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="a0667-816">Added support to open multiple ports</span></span>
* <span data-ttu-id="a0667-817">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="a0667-817">Added container group restart policy</span></span>
* <span data-ttu-id="a0667-818">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="a0667-818">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a0667-819">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="a0667-819">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a0667-820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0667-820">Data Lake Analytics</span></span>

* <span data-ttu-id="a0667-821">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="a0667-821">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a0667-822">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0667-822">Data Lake Store</span></span>

* <span data-ttu-id="a0667-823">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="a0667-823">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-824">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-824">Extension</span></span>

* <span data-ttu-id="a0667-825">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="a0667-825">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a0667-826">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="a0667-826">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a0667-827">IoT</span><span class="sxs-lookup"><span data-stu-id="a0667-827">IoT</span></span>

* <span data-ttu-id="a0667-828">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="a0667-828">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-829">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-829">Monitor</span></span>

* <span data-ttu-id="a0667-830">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="a0667-830">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a0667-831">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-831">Network</span></span>

* <span data-ttu-id="a0667-832">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="a0667-832">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a0667-833">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="a0667-833">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="a0667-834">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-834">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a0667-835">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="a0667-835">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="a0667-836">Reservations</span><span class="sxs-lookup"><span data-stu-id="a0667-836">Reservations</span></span>

* <span data-ttu-id="a0667-837">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="a0667-837">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-838">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-838">Resource</span></span>

* <span data-ttu-id="a0667-839">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-839">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-840">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-840">SQL</span></span>

* <span data-ttu-id="a0667-841">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-841">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-842">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-842">Storage</span></span>

* <span data-ttu-id="a0667-843">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="a0667-843">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a0667-844">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="a0667-844">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a0667-845">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="a0667-845">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="a0667-846">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="a0667-846">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="a0667-847">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="a0667-847">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="a0667-848">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="a0667-848">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="a0667-849">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="a0667-849">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-850">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-850">VM</span></span>

* <span data-ttu-id="a0667-851">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="a0667-851">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a0667-852">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="a0667-852">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a0667-853">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="a0667-853">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a0667-854">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="a0667-854">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="a0667-855">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a0667-855">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="a0667-856">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-856">October 24, 2017</span></span>

<span data-ttu-id="a0667-857">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a0667-857">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a0667-858">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-858">Core</span></span>

* <span data-ttu-id="a0667-859">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="a0667-859">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-860">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-860">ACR</span></span>

* <span data-ttu-id="a0667-861">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="a0667-861">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a0667-862">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="a0667-862">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a0667-863">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="a0667-863">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-864">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-864">ACS</span></span>

* <span data-ttu-id="a0667-865">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="a0667-865">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a0667-866">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0667-866">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-867">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-867">Appservice</span></span>

* <span data-ttu-id="a0667-868">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="a0667-868">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a0667-869">Componente</span><span class="sxs-lookup"><span data-stu-id="a0667-869">Component</span></span>

* <span data-ttu-id="a0667-870">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="a0667-870">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-871">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-871">Monitor</span></span>

* <span data-ttu-id="a0667-872">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="a0667-872">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-873">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-873">Resource</span></span>

* <span data-ttu-id="a0667-874">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="a0667-874">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="a0667-875">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="a0667-875">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-876">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-876">VM</span></span>

* <span data-ttu-id="a0667-877">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a0667-877">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="a0667-878">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-878">October 9, 2017</span></span>

<span data-ttu-id="a0667-879">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a0667-879">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a0667-880">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-880">Core</span></span>

* <span data-ttu-id="a0667-881">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a0667-881">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-882">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-882">Appservice</span></span>

* <span data-ttu-id="a0667-883">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="a0667-883">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="a0667-884">Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-884">Batch</span></span>

* <span data-ttu-id="a0667-885">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a0667-885">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a0667-886">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="a0667-886">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a0667-887">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-887">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a0667-888">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="a0667-888">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a0667-889">Batchai</span><span class="sxs-lookup"><span data-stu-id="a0667-889">Batchai</span></span>

* <span data-ttu-id="a0667-890">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-890">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0667-891">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a0667-891">Keyvault</span></span>

* <span data-ttu-id="a0667-892">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a0667-892">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a0667-893">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a0667-893">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a0667-894">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-894">Network</span></span>

* <span data-ttu-id="a0667-895">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="a0667-895">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a0667-896">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="a0667-896">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-897">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-897">Resource</span></span>

* <span data-ttu-id="a0667-898">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-898">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="a0667-899">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="a0667-899">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a0667-900">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="a0667-900">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a0667-901">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-901">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-902">Sql</span><span class="sxs-lookup"><span data-stu-id="a0667-902">Sql</span></span>

* <span data-ttu-id="a0667-903">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="a0667-903">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a0667-904">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="a0667-904">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a0667-905">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="a0667-905">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-906">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-906">Storage</span></span>

* <span data-ttu-id="a0667-907">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="a0667-907">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-908">Vm</span><span class="sxs-lookup"><span data-stu-id="a0667-908">Vm</span></span>

* <span data-ttu-id="a0667-909">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="a0667-909">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a0667-910">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a0667-910">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="a0667-911">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a0667-911">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="a0667-912">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="a0667-912">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="a0667-913">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a0667-913">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="a0667-914">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-914">September 22, 2017</span></span>

<span data-ttu-id="a0667-915">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a0667-915">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-916">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-916">Resource</span></span>

* <span data-ttu-id="a0667-917">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="a0667-917">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a0667-918">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="a0667-918">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a0667-919">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="a0667-919">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="a0667-920">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="a0667-920">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="a0667-921">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-921">Network</span></span>

* <span data-ttu-id="a0667-922">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a0667-922">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a0667-923">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="a0667-923">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="a0667-924">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="a0667-924">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a0667-925">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-925">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="a0667-926">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-926">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a0667-927">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-927">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="a0667-928">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="a0667-928">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-929">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-929">Storage</span></span>

* <span data-ttu-id="a0667-930">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="a0667-930">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a0667-931">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="a0667-931">Eventgrid</span></span>

* <span data-ttu-id="a0667-932">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="a0667-932">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-933">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-933">SQL</span></span>

* <span data-ttu-id="a0667-934">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="a0667-934">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a0667-935">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="a0667-935">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a0667-936">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-936">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0667-937">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a0667-937">Keyvault</span></span>

* <span data-ttu-id="a0667-938">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="a0667-938">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-939">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-939">VM</span></span>

* <span data-ttu-id="a0667-940">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="a0667-940">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="a0667-941">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="a0667-941">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a0667-942">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="a0667-942">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="a0667-943">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="a0667-943">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="a0667-944">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="a0667-944">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="a0667-945">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a0667-945">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-946">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-946">ACS</span></span>

* <span data-ttu-id="a0667-947">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-947">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-948">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-948">Appservice</span></span>

* <span data-ttu-id="a0667-949">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="a0667-949">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a0667-950">Backup</span><span class="sxs-lookup"><span data-stu-id="a0667-950">Backup</span></span>

* <span data-ttu-id="a0667-951">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="a0667-951">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a0667-952">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-952">September 11, 2017</span></span>

<span data-ttu-id="a0667-953">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a0667-953">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a0667-954">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-954">Core</span></span>

* <span data-ttu-id="a0667-955">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="a0667-955">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a0667-956">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a0667-956">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-957">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-957">Acs</span></span>

* <span data-ttu-id="a0667-958">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="a0667-958">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a0667-959">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="a0667-959">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-960">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-960">Appservice</span></span>

* <span data-ttu-id="a0667-961">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="a0667-961">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a0667-962">CDN</span><span class="sxs-lookup"><span data-stu-id="a0667-962">CDN</span></span>

* <span data-ttu-id="a0667-963">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="a0667-963">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="a0667-964">Extensión</span><span class="sxs-lookup"><span data-stu-id="a0667-964">Extension</span></span>

* <span data-ttu-id="a0667-965">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="a0667-965">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0667-966">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a0667-966">Keyvault</span></span>

* <span data-ttu-id="a0667-967">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="a0667-967">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="a0667-968">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-968">Network</span></span>

* <span data-ttu-id="a0667-969">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="a0667-969">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a0667-970">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-970">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="a0667-971">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-971">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="a0667-972">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-972">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a0667-973">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-973">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-974">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-974">Resource</span></span>

* <span data-ttu-id="a0667-975">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-975">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="a0667-976">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-976">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="a0667-977">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="a0667-977">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a0667-978">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="a0667-978">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-979">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-979">SQL</span></span>

* <span data-ttu-id="a0667-980">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="a0667-980">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-981">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-981">VM</span></span>

* <span data-ttu-id="a0667-982">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="a0667-982">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a0667-983">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="a0667-983">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a0667-984">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-984">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a0667-985">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="a0667-985">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a0667-986">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="a0667-986">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a0667-987">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-987">August 31, 2017</span></span>

<span data-ttu-id="a0667-988">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a0667-988">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0667-989">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a0667-989">Keyvault</span></span>

* <span data-ttu-id="a0667-990">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="a0667-990">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="a0667-991">Sf</span><span class="sxs-lookup"><span data-stu-id="a0667-991">Sf</span></span>

* <span data-ttu-id="a0667-992">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="a0667-992">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-993">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-993">Storage</span></span>

* <span data-ttu-id="a0667-994">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="a0667-994">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a0667-995">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="a0667-995">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a0667-996">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-996">August 28, 2017</span></span>

<span data-ttu-id="a0667-997">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a0667-997">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a0667-998">CLI</span><span class="sxs-lookup"><span data-stu-id="a0667-998">CLI</span></span>

* <span data-ttu-id="a0667-999">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="a0667-999">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-1000">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-1000">ACS</span></span>

* <span data-ttu-id="a0667-1001">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="a0667-1001">Corrected preview regions</span></span>
* <span data-ttu-id="a0667-1002">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="a0667-1002">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a0667-1003">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="a0667-1003">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-1004">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-1004">Appservice</span></span>

* <span data-ttu-id="a0667-1005">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="a0667-1005">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="a0667-1006">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1006">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="a0667-1007">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1007">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="a0667-1008">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="a0667-1008">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a0667-1009">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="a0667-1009">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a0667-1010">IoT</span><span class="sxs-lookup"><span data-stu-id="a0667-1010">IoT</span></span>

* <span data-ttu-id="a0667-1011">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="a0667-1011">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a0667-1012">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-1012">Network</span></span>

* <span data-ttu-id="a0667-1013">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="a0667-1013">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a0667-1014">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a0667-1014">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="a0667-1015">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1015">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a0667-1016">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1016">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a0667-1017">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1017">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-1018">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-1018">Profile</span></span>

* <span data-ttu-id="a0667-1019">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="a0667-1019">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a0667-1020">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0667-1020">Service Fabric</span></span>

* <span data-ttu-id="a0667-1021">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="a0667-1021">Preview release</span></span>
* <span data-ttu-id="a0667-1022">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="a0667-1022">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a0667-1023">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="a0667-1023">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a0667-1024">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1024">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-1025">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-1025">Storage</span></span>

* <span data-ttu-id="a0667-1026">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="a0667-1026">Enabled setting blob tier</span></span>
* <span data-ttu-id="a0667-1027">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="a0667-1027">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a0667-1028">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1028">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="a0667-1029">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="a0667-1029">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a0667-1030">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="a0667-1030">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a0667-1031">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="a0667-1031">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-1032">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-1032">VM</span></span>

* <span data-ttu-id="a0667-1033">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1033">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="a0667-1034">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1034">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a0667-1035">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1035">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="a0667-1036">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="a0667-1036">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a0667-1037">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="a0667-1037">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a0667-1038">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1038">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="a0667-1039">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-1039">August 15, 2017</span></span>

<span data-ttu-id="a0667-1040">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a0667-1040">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-1041">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-1041">ACS</span></span>

* <span data-ttu-id="a0667-1042">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0667-1042">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-1043">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-1043">Appservice</span></span>

* <span data-ttu-id="a0667-1044">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="a0667-1044">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a0667-1045">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a0667-1045">Event Grid</span></span>

* <span data-ttu-id="a0667-1046">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="a0667-1046">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a0667-1047">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-1047">August 11, 2017</span></span>

<span data-ttu-id="a0667-1048">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a0667-1048">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-1049">ACS</span></span>

* <span data-ttu-id="a0667-1050">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="a0667-1050">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a0667-1051">Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-1051">Batch</span></span>

* <span data-ttu-id="a0667-1052">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="a0667-1052">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a0667-1053">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="a0667-1053">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a0667-1054">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="a0667-1054">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a0667-1055">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="a0667-1055">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a0667-1056">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="a0667-1056">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a0667-1057">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="a0667-1057">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a0667-1058">Componente</span><span class="sxs-lookup"><span data-stu-id="a0667-1058">Component</span></span>

* <span data-ttu-id="a0667-1059">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="a0667-1059">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a0667-1060">Contenedor</span><span class="sxs-lookup"><span data-stu-id="a0667-1060">Container</span></span>

* <span data-ttu-id="a0667-1061">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="a0667-1061">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a0667-1062">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0667-1062">Data Lake Store</span></span>

* <span data-ttu-id="a0667-1063">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="a0667-1063">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a0667-1064">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a0667-1064">Event Grid</span></span>

* <span data-ttu-id="a0667-1065">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="a0667-1065">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a0667-1066">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-1066">Network</span></span>

* <span data-ttu-id="a0667-1067">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="a0667-1067">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="a0667-1068">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1068">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="a0667-1069">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="a0667-1069">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a0667-1070">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1070">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-1071">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-1071">Profile</span></span>

* <span data-ttu-id="a0667-1072">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="a0667-1072">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-1073">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-1073">Storage</span></span>

* <span data-ttu-id="a0667-1074">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="a0667-1074">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-1075">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-1075">VM</span></span>

* <span data-ttu-id="a0667-1076">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="a0667-1076">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a0667-1077">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1077">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a0667-1078">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="a0667-1078">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a0667-1079">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="a0667-1079">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a0667-1080">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="a0667-1080">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a0667-1081">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-1081">July 28, 2017</span></span>

<span data-ttu-id="a0667-1082">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a0667-1082">Version 2.0.12</span></span>

* <span data-ttu-id="a0667-1083">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="a0667-1083">Added container commands</span></span>
* <span data-ttu-id="a0667-1084">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="a0667-1084">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a0667-1085">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-1085">Core</span></span>

* <span data-ttu-id="a0667-1086">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="a0667-1086">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a0667-1087">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="a0667-1087">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a0667-1088">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="a0667-1088">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a0667-1089">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="a0667-1089">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a0667-1090">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="a0667-1090">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a0667-1091">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="a0667-1091">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a0667-1092">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="a0667-1092">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a0667-1093">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="a0667-1093">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a0667-1094">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="a0667-1094">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a0667-1095">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="a0667-1095">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a0667-1096">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="a0667-1096">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a0667-1097">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="a0667-1097">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a0667-1098">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a0667-1098">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a0667-1099">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a0667-1099">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a0667-1100">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a0667-1100">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a0667-1101">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="a0667-1101">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a0667-1102">ACR</span><span class="sxs-lookup"><span data-stu-id="a0667-1102">ACR</span></span>

* <span data-ttu-id="a0667-1103">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="a0667-1103">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a0667-1104">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="a0667-1104">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a0667-1105">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="a0667-1105">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a0667-1106">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="a0667-1106">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a0667-1107">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="a0667-1107">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a0667-1108">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="a0667-1108">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-1109">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-1109">ACS</span></span>

* <span data-ttu-id="a0667-1110">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="a0667-1110">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-1111">Appservice</span><span class="sxs-lookup"><span data-stu-id="a0667-1111">Appservice</span></span>

* <span data-ttu-id="a0667-1112">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="a0667-1112">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a0667-1113">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="a0667-1113">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a0667-1114">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1114">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="a0667-1115">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="a0667-1115">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a0667-1116">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="a0667-1116">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a0667-1117">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="a0667-1117">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a0667-1118">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="a0667-1118">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a0667-1119">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="a0667-1119">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a0667-1120">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="a0667-1120">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a0667-1121">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="a0667-1121">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="a0667-1122">Batch</span><span class="sxs-lookup"><span data-stu-id="a0667-1122">Batch</span></span>

* <span data-ttu-id="a0667-1123">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="a0667-1123">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a0667-1124">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1124">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="a0667-1125">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1125">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="a0667-1126">CDN</span><span class="sxs-lookup"><span data-stu-id="a0667-1126">CDN</span></span>

* <span data-ttu-id="a0667-1127">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="a0667-1127">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a0667-1128">Nube</span><span class="sxs-lookup"><span data-stu-id="a0667-1128">Cloud</span></span>

* <span data-ttu-id="a0667-1129">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="a0667-1129">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a0667-1130">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="a0667-1130">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a0667-1131">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="a0667-1131">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a0667-1132">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="a0667-1132">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a0667-1133">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1133">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0667-1134">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0667-1134">CosmosDB</span></span>

* <span data-ttu-id="a0667-1135">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="a0667-1135">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a0667-1136">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="a0667-1136">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a0667-1137">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0667-1137">Data Lake Analytics</span></span>

* <span data-ttu-id="a0667-1138">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1138">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a0667-1139">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1139">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="a0667-1140">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1140">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a0667-1141">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0667-1141">Data Lake Store</span></span>

* <span data-ttu-id="a0667-1142">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1142">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="a0667-1143">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="a0667-1143">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a0667-1144">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1144">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a0667-1145">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a0667-1145">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a0667-1146">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0667-1146">Interactive</span></span>

* <span data-ttu-id="a0667-1147">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="a0667-1147">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a0667-1148">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="a0667-1148">Increased test coverage</span></span>
* <span data-ttu-id="a0667-1149">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="a0667-1149">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a0667-1150">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="a0667-1150">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a0667-1151">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="a0667-1151">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a0667-1152">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="a0667-1152">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a0667-1153">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="a0667-1153">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a0667-1154">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1154">Added `--progress` flag</span></span>
* <span data-ttu-id="a0667-1155">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="a0667-1155">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a0667-1156">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="a0667-1156">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a0667-1157">IoT</span><span class="sxs-lookup"><span data-stu-id="a0667-1157">IoT</span></span>

* <span data-ttu-id="a0667-1158">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="a0667-1158">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a0667-1159">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="a0667-1159">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a0667-1160">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="a0667-1160">Key vault</span></span>

* <span data-ttu-id="a0667-1161">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="a0667-1161">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="a0667-1162">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a0667-1162">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="a0667-1163">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a0667-1163">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a0667-1164">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a0667-1164">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a0667-1165">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a0667-1165">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="a0667-1166">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="a0667-1166">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a0667-1167">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="a0667-1167">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a0667-1168">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="a0667-1168">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a0667-1169">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-1169">Lab</span></span>

* <span data-ttu-id="a0667-1170">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1170">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="a0667-1171">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1171">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-1172">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-1172">Monitor</span></span>

* <span data-ttu-id="a0667-1173">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="a0667-1173">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a0667-1174">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1174">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="a0667-1175">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1175">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="a0667-1176">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1176">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="a0667-1177">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1177">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="a0667-1178">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="a0667-1178">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="a0667-1179">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="a0667-1179">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a0667-1180">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="a0667-1180">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="a0667-1181">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="a0667-1181">`location` no longer required</span></span>
  * <span data-ttu-id="a0667-1182">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="a0667-1182">Add name and ID support for target</span></span>
  * <span data-ttu-id="a0667-1183">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1183">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="a0667-1184">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="a0667-1184">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="a0667-1185">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="a0667-1185">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a0667-1186">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="a0667-1186">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a0667-1187">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1187">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a0667-1188">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="a0667-1188">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="a0667-1189">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-1189">Network</span></span>

* <span data-ttu-id="a0667-1190">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1190">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a0667-1191">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1191">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="a0667-1192">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="a0667-1192">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a0667-1193">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="a0667-1193">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a0667-1194">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1194">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="a0667-1195">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1195">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a0667-1196">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="a0667-1196">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="a0667-1197">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="a0667-1197">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="a0667-1198">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="a0667-1198">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a0667-1199">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a0667-1199">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="a0667-1200">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="a0667-1200">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="a0667-1201">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1201">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="a0667-1202">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="a0667-1202">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="a0667-1203">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1203">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="a0667-1204">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1204">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="a0667-1205">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1205">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="a0667-1206">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="a0667-1206">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a0667-1207">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1207">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="a0667-1208">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1208">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="a0667-1209">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1209">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="a0667-1210">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1210">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="a0667-1211">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1211">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a0667-1212">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1212">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="a0667-1213">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="a0667-1213">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a0667-1214">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="a0667-1214">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a0667-1215">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="a0667-1215">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a0667-1216">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="a0667-1216">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-1217">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-1217">Profile</span></span>

* <span data-ttu-id="a0667-1218">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="a0667-1218">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a0667-1219">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="a0667-1219">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a0667-1220">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="a0667-1220">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a0667-1221">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="a0667-1221">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a0667-1222">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="a0667-1222">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0667-1223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a0667-1223">RDBMS</span></span>

* <span data-ttu-id="a0667-1224">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="a0667-1224">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a0667-1225">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="a0667-1225">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a0667-1226">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="a0667-1226">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a0667-1227">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="a0667-1227">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-1228">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-1228">Resource</span></span>

* <span data-ttu-id="a0667-1229">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1229">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="a0667-1230">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1230">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a0667-1231">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1231">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a0667-1232">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1232">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a0667-1233">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="a0667-1233">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a0667-1234">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1234">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="a0667-1235">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="a0667-1235">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a0667-1236">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1236">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a0667-1237">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-1237">Role</span></span>

* <span data-ttu-id="a0667-1238">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="a0667-1238">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="a0667-1239">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="a0667-1239">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a0667-1240">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1240">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a0667-1241">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1241">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="a0667-1242">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1242">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a0667-1243">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0667-1243">Service Fabric</span></span>
* <span data-ttu-id="a0667-1244">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="a0667-1244">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a0667-1245">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="a0667-1245">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a0667-1246">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="a0667-1246">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-1247">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-1247">SQL</span></span>

* <span data-ttu-id="a0667-1248">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="a0667-1248">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a0667-1249">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1249">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a0667-1250">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="a0667-1250">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-1251">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-1251">Storage</span></span>

* <span data-ttu-id="a0667-1252">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="a0667-1252">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a0667-1253">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="a0667-1253">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a0667-1254">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="a0667-1254">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a0667-1255">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="a0667-1255">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a0667-1256">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="a0667-1256">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a0667-1257">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="a0667-1257">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-1258">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-1258">VM</span></span>

* <span data-ttu-id="a0667-1259">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="a0667-1259">Support configuring nsg</span></span>
* <span data-ttu-id="a0667-1260">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="a0667-1260">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a0667-1261">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="a0667-1261">Support managed service identities</span></span>
* <span data-ttu-id="a0667-1262">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="a0667-1262">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="a0667-1263">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="a0667-1263">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a0667-1264">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-1264">May 10, 2017</span></span>

<span data-ttu-id="a0667-1265">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a0667-1265">Version 2.0.6</span></span>

* <span data-ttu-id="a0667-1266">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="a0667-1266">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a0667-1267">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="a0667-1267">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a0667-1268">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0667-1268">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a0667-1269">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0667-1269">Include Cognitive Services module</span></span>
* <span data-ttu-id="a0667-1270">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0667-1270">Include Service Fabric module</span></span>
* <span data-ttu-id="a0667-1271">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="a0667-1271">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a0667-1272">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="a0667-1272">Add support for CDN commands</span></span>
* <span data-ttu-id="a0667-1273">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="a0667-1273">Remove Container module</span></span>
* <span data-ttu-id="a0667-1274">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="a0667-1274">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a0667-1275">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a0667-1275">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a0667-1276">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-1276">Core</span></span>

* <span data-ttu-id="a0667-1277">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="a0667-1277">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a0667-1278">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="a0667-1278">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a0667-1279">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="a0667-1279">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a0667-1280">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="a0667-1280">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a0667-1281">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="a0667-1281">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a0667-1282">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="a0667-1282">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a0667-1283">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="a0667-1283">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a0667-1284">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="a0667-1284">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a0667-1285">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="a0667-1285">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a0667-1286">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="a0667-1286">core: Improved performance</span></span>
* <span data-ttu-id="a0667-1287">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="a0667-1287">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a0667-1288">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="a0667-1288">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-1289">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-1289">ACS</span></span>

* <span data-ttu-id="a0667-1290">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="a0667-1290">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a0667-1291">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="a0667-1291">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a0667-1292">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="a0667-1292">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a0667-1293">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="a0667-1293">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-1294">AppService</span><span class="sxs-lookup"><span data-stu-id="a0667-1294">AppService</span></span>

* <span data-ttu-id="a0667-1295">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="a0667-1295">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a0667-1296">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="a0667-1296">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a0667-1297">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="a0667-1297">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a0667-1298">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="a0667-1298">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a0667-1299">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="a0667-1299">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a0667-1300">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="a0667-1300">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a0667-1301">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="a0667-1301">support slot swap with preview</span></span>
* <span data-ttu-id="a0667-1302">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="a0667-1302">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a0667-1303">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="a0667-1303">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0667-1304">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0667-1304">CosmosDB</span></span>

* <span data-ttu-id="a0667-1305">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0667-1305">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a0667-1306">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="a0667-1306">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a0667-1307">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="a0667-1307">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a0667-1308">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="a0667-1308">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a0667-1309">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0667-1309">Data Lake Analytics</span></span>

* <span data-ttu-id="a0667-1310">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="a0667-1310">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a0667-1311">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="a0667-1311">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a0667-1312">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="a0667-1312">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a0667-1313">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="a0667-1313">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a0667-1314">Tabla</span><span class="sxs-lookup"><span data-stu-id="a0667-1314">Table</span></span>
  * <span data-ttu-id="a0667-1315">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="a0667-1315">Table valued function</span></span>
  * <span data-ttu-id="a0667-1316">Ver</span><span class="sxs-lookup"><span data-stu-id="a0667-1316">View</span></span>
  * <span data-ttu-id="a0667-1317">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="a0667-1317">Table Statistics.</span></span> <span data-ttu-id="a0667-1318">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="a0667-1318">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a0667-1319">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0667-1319">Data Lake Store</span></span>

* <span data-ttu-id="a0667-1320">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="a0667-1320">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a0667-1321">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a0667-1321">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a0667-1322">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="a0667-1322">missed help for access show.</span></span> <span data-ttu-id="a0667-1323">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="a0667-1323">adding it.</span></span> <span data-ttu-id="a0667-1324">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a0667-1324">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a0667-1325">Buscar</span><span class="sxs-lookup"><span data-stu-id="a0667-1325">Find</span></span>

* <span data-ttu-id="a0667-1326">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="a0667-1326">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0667-1327">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0667-1327">KeyVault</span></span>

* <span data-ttu-id="a0667-1328">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="a0667-1328">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a0667-1329">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="a0667-1329">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a0667-1330">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="a0667-1330">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a0667-1331">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="a0667-1331">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a0667-1332">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="a0667-1332">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a0667-1333">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-1333">Lab</span></span>

* <span data-ttu-id="a0667-1334">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-1334">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a0667-1335">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-1335">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a0667-1336">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-1336">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a0667-1337">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-1337">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a0667-1338">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="a0667-1338">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a0667-1339">Supervisión</span><span class="sxs-lookup"><span data-stu-id="a0667-1339">Monitor</span></span>

* <span data-ttu-id="a0667-1340">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="a0667-1340">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a0667-1341">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="a0667-1341">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a0667-1342">Red</span><span class="sxs-lookup"><span data-stu-id="a0667-1342">Network</span></span>

* <span data-ttu-id="a0667-1343">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="a0667-1343">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a0667-1344">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="a0667-1344">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="a0667-1345">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a0667-1345">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a0667-1346">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a0667-1346">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a0667-1347">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="a0667-1347">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a0667-1348">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a0667-1348">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a0667-1349">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="a0667-1349">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a0667-1350">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="a0667-1350">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a0667-1351">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="a0667-1351">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a0667-1352">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="a0667-1352">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a0667-1353">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="a0667-1353">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a0667-1354">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="a0667-1354">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="a0667-1355">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="a0667-1355">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a0667-1356">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="a0667-1356">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a0667-1357">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="a0667-1357">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a0667-1358">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="a0667-1358">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a0667-1359">Perfil</span><span class="sxs-lookup"><span data-stu-id="a0667-1359">Profile</span></span>

* <span data-ttu-id="a0667-1360">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="a0667-1360">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a0667-1361">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="a0667-1361">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a0667-1362">Redis</span><span class="sxs-lookup"><span data-stu-id="a0667-1362">Redis</span></span>

* <span data-ttu-id="a0667-1363">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="a0667-1363">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a0667-1364">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="a0667-1364">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a0667-1365">Recurso</span><span class="sxs-lookup"><span data-stu-id="a0667-1365">Resource</span></span>

* <span data-ttu-id="a0667-1366">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="a0667-1366">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a0667-1367">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="a0667-1367">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a0667-1368">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="a0667-1368">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a0667-1369">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="a0667-1369">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a0667-1370">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a0667-1370">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a0667-1371">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="a0667-1371">Add docs for az lock update.</span></span> <span data-ttu-id="a0667-1372">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a0667-1372">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a0667-1373">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="a0667-1373">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a0667-1374">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a0667-1374">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a0667-1375">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="a0667-1375">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a0667-1376">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a0667-1376">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a0667-1377">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="a0667-1377">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a0667-1378">Rol</span><span class="sxs-lookup"><span data-stu-id="a0667-1378">Role</span></span>

* <span data-ttu-id="a0667-1379">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="a0667-1379">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a0667-1380">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="a0667-1380">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a0667-1381">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="a0667-1381">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a0667-1382">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="a0667-1382">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a0667-1383">SQL</span><span class="sxs-lookup"><span data-stu-id="a0667-1383">SQL</span></span>

* <span data-ttu-id="a0667-1384">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="a0667-1384">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a0667-1385">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="a0667-1385">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a0667-1386">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-1386">Storage</span></span>

* <span data-ttu-id="a0667-1387">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="a0667-1387">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="a0667-1388">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="a0667-1388">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a0667-1389">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="a0667-1389">Add support for large block blob upload</span></span>
* <span data-ttu-id="a0667-1390">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="a0667-1390">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-1391">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-1391">VM</span></span>

* <span data-ttu-id="a0667-1392">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="a0667-1392">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a0667-1393">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="a0667-1393">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a0667-1394">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a0667-1394">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a0667-1395">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a0667-1395">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a0667-1396">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="a0667-1396">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a0667-1397">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="a0667-1397">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a0667-1398">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="a0667-1398">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a0667-1399">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-1399">April 3, 2017</span></span>

<span data-ttu-id="a0667-1400">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a0667-1400">Version 2.0.2</span></span>

<span data-ttu-id="a0667-1401">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="a0667-1401">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a0667-1402">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a0667-1402">Core</span></span>

* <span data-ttu-id="a0667-1403">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="a0667-1403">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a0667-1404">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="a0667-1404">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a0667-1405">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="a0667-1405">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a0667-1406">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a0667-1406">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a0667-1407">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="a0667-1407">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a0667-1408">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="a0667-1408">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a0667-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="a0667-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a0667-1410">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="a0667-1410">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a0667-1411">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="a0667-1411">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a0667-1412">ACS</span><span class="sxs-lookup"><span data-stu-id="a0667-1412">ACS</span></span>

* <span data-ttu-id="a0667-1413">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="a0667-1413">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a0667-1414">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="a0667-1414">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a0667-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="a0667-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a0667-1416">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="a0667-1416">Add support for windows clusters.</span></span> <span data-ttu-id="a0667-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="a0667-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a0667-1418">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="a0667-1418">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a0667-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="a0667-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a0667-1420">AppService</span><span class="sxs-lookup"><span data-stu-id="a0667-1420">AppService</span></span>

* <span data-ttu-id="a0667-1421">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="a0667-1421">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a0667-1422">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="a0667-1422">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a0667-1423">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="a0667-1423">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a0667-1424">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="a0667-1424">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a0667-1425">DataLake</span><span class="sxs-lookup"><span data-stu-id="a0667-1425">DataLake</span></span>

* <span data-ttu-id="a0667-1426">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0667-1426">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a0667-1427">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0667-1427">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a0667-1428">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a0667-1428">DocuemntDB</span></span>

* <span data-ttu-id="a0667-1429">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="a0667-1429">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a0667-1430">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a0667-1430">VM</span></span>

* <span data-ttu-id="a0667-1431">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="a0667-1431">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a0667-1432">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="a0667-1432">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a0667-1433">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="a0667-1433">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a0667-1434">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a0667-1434">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a0667-1435">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="a0667-1435">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a0667-1436">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="a0667-1436">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="a0667-1437">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="a0667-1437">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a0667-1438">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="a0667-1438">February 27, 2017</span></span>

<span data-ttu-id="a0667-1439">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a0667-1439">Version 2.0.0</span></span>

<span data-ttu-id="a0667-1440">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="a0667-1440">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a0667-1441">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="a0667-1441">Container Service (acs)</span></span>
- <span data-ttu-id="a0667-1442">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="a0667-1442">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a0667-1443">Redes</span><span class="sxs-lookup"><span data-stu-id="a0667-1443">Networking</span></span>
- <span data-ttu-id="a0667-1444">Storage</span><span class="sxs-lookup"><span data-stu-id="a0667-1444">Storage</span></span>

<span data-ttu-id="a0667-1445">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="a0667-1445">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a0667-1446">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="a0667-1446">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a0667-1447">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="a0667-1447">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a0667-1448">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="a0667-1448">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a0667-1449">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a0667-1449">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a0667-1450">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="a0667-1450">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a0667-1451">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="a0667-1451">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a0667-1452">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="a0667-1452">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a0667-1453">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="a0667-1453">Provide feedback from the command line with the `az feedback` command</span></span>

