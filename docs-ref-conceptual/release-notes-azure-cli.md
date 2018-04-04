---
title: Notas de la versión de la CLI de Azure 2.0
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0e81f5723af47242f908b854045deb7d74c50c17
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="22d92-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="22d92-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-27-2018"></a><span data-ttu-id="22d92-104">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="22d92-104">March 27, 2018</span></span>

<span data-ttu-id="22d92-105">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="22d92-105">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="22d92-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-106">Core</span></span>

* <span data-ttu-id="22d92-107">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="22d92-107">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-108">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-108">ACS</span></span>

* <span data-ttu-id="22d92-109">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="22d92-109">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-110">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-110">Appservice</span></span>

* <span data-ttu-id="22d92-111">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="22d92-111">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="22d92-112">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="22d92-112">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="22d92-113">Backup</span><span class="sxs-lookup"><span data-stu-id="22d92-113">Backup</span></span>

* <span data-ttu-id="22d92-114">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="22d92-114">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="22d92-115">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-115">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="22d92-116">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="22d92-116">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="22d92-117">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="22d92-117">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="22d92-118">Contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-118">Container</span></span>

* <span data-ttu-id="22d92-119">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="22d92-119">Added `container exec` command.</span></span> <span data-ttu-id="22d92-120">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="22d92-120">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="22d92-121">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="22d92-121">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="22d92-122">Extensión</span><span class="sxs-lookup"><span data-stu-id="22d92-122">Extension</span></span>

* <span data-ttu-id="22d92-123">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="22d92-123">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="22d92-124">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="22d92-124">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="22d92-125">[[CAMBIO IMPORTANTE]] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="22d92-125">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="22d92-126">Interactive</span><span class="sxs-lookup"><span data-stu-id="22d92-126">Interactive</span></span>

* <span data-ttu-id="22d92-127">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="22d92-127">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="22d92-128">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="22d92-128">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="22d92-129">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="22d92-129">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="22d92-130">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="22d92-130">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="22d92-131">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-131">Lab</span></span>

* <span data-ttu-id="22d92-132">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="22d92-132">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-133">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-133">Monitor</span></span>

* <span data-ttu-id="22d92-134">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="22d92-134">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="22d92-135">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="22d92-135">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="22d92-136">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="22d92-136">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="22d92-137">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-137">Network</span></span>

* <span data-ttu-id="22d92-138">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="22d92-138">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-139">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-139">Profile</span></span>

* <span data-ttu-id="22d92-140">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="22d92-140">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="22d92-141">RDBMS</span><span class="sxs-lookup"><span data-stu-id="22d92-141">RDBMS</span></span>

* <span data-ttu-id="22d92-142">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="22d92-142">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-143">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-143">Resource</span></span>

* <span data-ttu-id="22d92-144">[[CAMBIO IMPORTANTE]]: Changed `provider operation [list|show]` to not require `--api-version`</span><span class="sxs-lookup"><span data-stu-id="22d92-144">[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`</span></span>

### <a name="role"></a><span data-ttu-id="22d92-145">Rol</span><span class="sxs-lookup"><span data-stu-id="22d92-145">Role</span></span>

* <span data-ttu-id="22d92-146">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="22d92-146">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="22d92-147">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="22d92-147">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="22d92-148">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="22d92-148">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="22d92-149">[[CAMBIO IMPORTANTE]] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="22d92-149">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="22d92-150">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="22d92-150">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-151">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-151">Storage</span></span>

* <span data-ttu-id="22d92-152">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="22d92-152">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="22d92-153">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="22d92-153">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-154">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-154">VM</span></span>

* <span data-ttu-id="22d92-155">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="22d92-155">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="22d92-156">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="22d92-156">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="22d92-157">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="22d92-157">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="22d92-158">[[CAMBIO IMPORTANTE]] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="22d92-158">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="22d92-159">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="22d92-159">March 13, 2018</span></span>

<span data-ttu-id="22d92-160">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="22d92-160">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="22d92-161">ACR</span><span class="sxs-lookup"><span data-stu-id="22d92-161">ACR</span></span>

* <span data-ttu-id="22d92-162">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="22d92-162">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="22d92-163">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="22d92-163">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="22d92-164">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="22d92-164">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-165">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-165">ACS</span></span>

* <span data-ttu-id="22d92-166">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="22d92-166">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="22d92-167">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="22d92-167">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="22d92-168">Advisor</span><span class="sxs-lookup"><span data-stu-id="22d92-168">Advisor</span></span>

* <span data-ttu-id="22d92-169">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="22d92-169">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="22d92-170">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="22d92-170">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="22d92-171">[[CAMBIO IMPORTANTE]] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="22d92-171">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="22d92-172">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="22d92-172">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="22d92-173">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="22d92-173">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-174">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-174">Appservice</span></span>

* <span data-ttu-id="22d92-175">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="22d92-175">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="22d92-176">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="22d92-176">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="22d92-177">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="22d92-177">Eventhubs</span></span>

* <span data-ttu-id="22d92-178">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="22d92-178">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="22d92-179">Extensión</span><span class="sxs-lookup"><span data-stu-id="22d92-179">Extension</span></span>

* <span data-ttu-id="22d92-180">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="22d92-180">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="22d92-181">Interactive</span><span class="sxs-lookup"><span data-stu-id="22d92-181">Interactive</span></span>

* <span data-ttu-id="22d92-182">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="22d92-182">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="22d92-183">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="22d92-183">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="22d92-184">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="22d92-184">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="22d92-185">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="22d92-185">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-186">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-186">Monitor</span></span>

* <span data-ttu-id="22d92-187">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="22d92-187">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="22d92-188">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="22d92-188">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="22d92-189">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="22d92-189">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="22d92-190">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="22d92-190">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="22d92-191">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-191">Network</span></span>

* <span data-ttu-id="22d92-192">[[CAMBIO IMPORTANTE]] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="22d92-192">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="22d92-193">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="22d92-193">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="22d92-194">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="22d92-194">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="22d92-195">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="22d92-195">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-196">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-196">Profile</span></span>

* <span data-ttu-id="22d92-197">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="22d92-197">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="22d92-198">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="22d92-198">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="22d92-199">RDBMS</span><span class="sxs-lookup"><span data-stu-id="22d92-199">RDBMS</span></span>

* <span data-ttu-id="22d92-200">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="22d92-200">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="22d92-201">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="22d92-201">Service Bus</span></span>

* <span data-ttu-id="22d92-202">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="22d92-202">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-203">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-203">Storage</span></span>

* <span data-ttu-id="22d92-204">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="22d92-204">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="22d92-205">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="22d92-205">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-206">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-206">VM</span></span>

* <span data-ttu-id="22d92-207">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="22d92-207">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="22d92-208">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="22d92-208">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="22d92-209">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="22d92-209">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="22d92-210">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="22d92-210">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="22d92-211">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="22d92-211">February 27, 2018</span></span>

<span data-ttu-id="22d92-212">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="22d92-212">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="22d92-213">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-213">Core</span></span>

* <span data-ttu-id="22d92-214">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="22d92-214">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="22d92-215">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="22d92-215">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="22d92-216">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="22d92-216">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-217">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-217">ACS</span></span>

* <span data-ttu-id="22d92-218">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="22d92-218">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="22d92-219">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="22d92-219">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="22d92-220">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="22d92-220">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="22d92-221">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="22d92-221">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-222">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-222">Appservice</span></span>

* <span data-ttu-id="22d92-223">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="22d92-223">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="22d92-224">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="22d92-224">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="22d92-225">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="22d92-225">Cognitive Services</span></span>

* <span data-ttu-id="22d92-226">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="22d92-226">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="22d92-227">Consumo</span><span class="sxs-lookup"><span data-stu-id="22d92-227">Consumption</span></span>

* <span data-ttu-id="22d92-228">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="22d92-228">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="22d92-229">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="22d92-229">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="22d92-230">Contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-230">Container</span></span>

* <span data-ttu-id="22d92-231">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="22d92-231">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="22d92-232">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-232">Network</span></span>

* <span data-ttu-id="22d92-233">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="22d92-233">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-234">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-234">Resource</span></span>

* <span data-ttu-id="22d92-235">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="22d92-235">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="22d92-236">Rol</span><span class="sxs-lookup"><span data-stu-id="22d92-236">Role</span></span>

* <span data-ttu-id="22d92-237">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="22d92-237">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-238">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-238">SQL</span></span>

* <span data-ttu-id="22d92-239">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="22d92-239">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-240">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-240">Storage</span></span>

* <span data-ttu-id="22d92-241">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="22d92-241">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-242">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-242">VM</span></span>

* <span data-ttu-id="22d92-243">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="22d92-243">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="22d92-244">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="22d92-244">February 13, 2018</span></span>

<span data-ttu-id="22d92-245">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="22d92-245">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="22d92-246">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-246">Core</span></span>

* <span data-ttu-id="22d92-247">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="22d92-247">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-248">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-248">ACS</span></span>

* <span data-ttu-id="22d92-249">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="22d92-249">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="22d92-250">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="22d92-250">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="22d92-251">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="22d92-251">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="22d92-252">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="22d92-252">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="22d92-253">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="22d92-253">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="22d92-254">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="22d92-254">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="22d92-255">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="22d92-255">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="22d92-256">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="22d92-256">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-257">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-257">Appservice</span></span>

* <span data-ttu-id="22d92-258">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="22d92-258">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="22d92-259">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="22d92-259">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="22d92-260">CDN</span><span class="sxs-lookup"><span data-stu-id="22d92-260">CDN</span></span>

* <span data-ttu-id="22d92-261">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="22d92-261">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="22d92-262">Contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-262">Container</span></span>

* <span data-ttu-id="22d92-263">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="22d92-263">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="22d92-264">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="22d92-264">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="22d92-265">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="22d92-265">CosmosDB</span></span>

* <span data-ttu-id="22d92-266">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="22d92-266">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="22d92-267">Extensión</span><span class="sxs-lookup"><span data-stu-id="22d92-267">Extension</span></span>

* <span data-ttu-id="22d92-268">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-268">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="22d92-269">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-269">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="22d92-270">Comentarios</span><span class="sxs-lookup"><span data-stu-id="22d92-270">Feedback</span></span>

* <span data-ttu-id="22d92-271">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="22d92-271">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="22d92-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="22d92-272">Interactive</span></span>

* <span data-ttu-id="22d92-273">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="22d92-273">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="22d92-274">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="22d92-274">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="22d92-275">IoT</span><span class="sxs-lookup"><span data-stu-id="22d92-275">IoT</span></span>

* <span data-ttu-id="22d92-276">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="22d92-276">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="22d92-277">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="22d92-277">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="22d92-278">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-278">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="22d92-279">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="22d92-279">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-280">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-280">Monitor</span></span>

* <span data-ttu-id="22d92-281">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="22d92-281">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="22d92-282">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-282">Network</span></span>

* <span data-ttu-id="22d92-283">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="22d92-283">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="22d92-284">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-284">Profile</span></span>

* <span data-ttu-id="22d92-285">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="22d92-285">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-286">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-286">Resource</span></span>

* <span data-ttu-id="22d92-287">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="22d92-287">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="22d92-288">Rol</span><span class="sxs-lookup"><span data-stu-id="22d92-288">Role</span></span>

* <span data-ttu-id="22d92-289">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="22d92-289">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-290">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-290">SQL</span></span>

* <span data-ttu-id="22d92-291">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="22d92-291">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="22d92-292">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="22d92-292">Added `sql db rename`</span></span>
* <span data-ttu-id="22d92-293">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="22d92-293">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-294">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-294">Storage</span></span>

* <span data-ttu-id="22d92-295">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="22d92-295">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-296">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-296">VM</span></span>

* <span data-ttu-id="22d92-297">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="22d92-297">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="22d92-298">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="22d92-298">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="22d92-299">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="22d92-299">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="22d92-300">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="22d92-300">January 31, 2018</span></span>

<span data-ttu-id="22d92-301">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="22d92-301">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="22d92-302">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-302">Core</span></span>

* <span data-ttu-id="22d92-303">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="22d92-303">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="22d92-304">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="22d92-304">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="22d92-305">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="22d92-305">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="22d92-306">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="22d92-306">Use `--verbose` to see</span></span>
* <span data-ttu-id="22d92-307">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="22d92-307">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-308">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-308">ACS</span></span>

* <span data-ttu-id="22d92-309">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="22d92-309">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="22d92-310">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="22d92-310">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-311">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-311">Appservice</span></span>

* <span data-ttu-id="22d92-312">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="22d92-312">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="22d92-313">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="22d92-313">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="22d92-314">CDN</span><span class="sxs-lookup"><span data-stu-id="22d92-314">CDN</span></span>

* <span data-ttu-id="22d92-315">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="22d92-315">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="22d92-316">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="22d92-316">CosmosDB</span></span>

* <span data-ttu-id="22d92-317">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="22d92-317">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="22d92-318">Interactive</span><span class="sxs-lookup"><span data-stu-id="22d92-318">Interactive</span></span>

* <span data-ttu-id="22d92-319">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="22d92-319">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="22d92-320">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-320">Network</span></span>

* <span data-ttu-id="22d92-321">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="22d92-321">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="22d92-322">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="22d92-322">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="22d92-323">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="22d92-323">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="22d92-324">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="22d92-324">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="22d92-325">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="22d92-325">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="22d92-326">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="22d92-326">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="22d92-327">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="22d92-327">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="22d92-328">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="22d92-328">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="22d92-329">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="22d92-329">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="22d92-330">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="22d92-330">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-331">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-331">Profile</span></span>

* <span data-ttu-id="22d92-332">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="22d92-332">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-333">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-333">Resource</span></span>

* <span data-ttu-id="22d92-334">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="22d92-334">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-335">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-335">Storage</span></span>

* <span data-ttu-id="22d92-336">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="22d92-336">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="22d92-337">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="22d92-337">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="22d92-338">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="22d92-338">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="22d92-339">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="22d92-339">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="22d92-340">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="22d92-340">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-341">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-341">VM</span></span>

* <span data-ttu-id="22d92-342">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="22d92-342">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="22d92-343">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="22d92-343">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="22d92-344">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="22d92-344">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="22d92-345">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="22d92-345">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="22d92-346">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="22d92-346">January 17, 2018</span></span>

<span data-ttu-id="22d92-347">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="22d92-347">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="22d92-348">ACR</span><span class="sxs-lookup"><span data-stu-id="22d92-348">ACR</span></span>

* <span data-ttu-id="22d92-349">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="22d92-349">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="22d92-350">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="22d92-350">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-351">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-351">ACS</span></span>

* <span data-ttu-id="22d92-352">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="22d92-352">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="22d92-353">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="22d92-353">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-354">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-354">Appservice</span></span>

* <span data-ttu-id="22d92-355">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="22d92-355">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="22d92-356">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="22d92-356">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="22d92-357">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="22d92-357">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="22d92-358">Backup</span><span class="sxs-lookup"><span data-stu-id="22d92-358">Backup</span></span>

* <span data-ttu-id="22d92-359">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="22d92-359">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="22d92-360">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="22d92-360">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="22d92-361">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="22d92-361">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="22d92-362">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="22d92-362">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="22d92-363">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="22d92-363">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="22d92-364">Batch</span><span class="sxs-lookup"><span data-stu-id="22d92-364">Batch</span></span>

* <span data-ttu-id="22d92-365">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="22d92-365">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="22d92-366">Nube</span><span class="sxs-lookup"><span data-stu-id="22d92-366">Cloud</span></span>

* <span data-ttu-id="22d92-367">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="22d92-367">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="22d92-368">Consumo</span><span class="sxs-lookup"><span data-stu-id="22d92-368">Consumption</span></span>

* <span data-ttu-id="22d92-369">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="22d92-369">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="22d92-370">Event Grid</span><span class="sxs-lookup"><span data-stu-id="22d92-370">Event Grid</span></span>

* <span data-ttu-id="22d92-371">[[CAMBIO IMPORTANTE]] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="22d92-371">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="22d92-372">[[CAMBIO IMPORTANTE]] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="22d92-372">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="22d92-373">[[CAMBIO IMPORTANTE]] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="22d92-373">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="22d92-374">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="22d92-374">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="22d92-375">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="22d92-375">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="22d92-376">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="22d92-376">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="22d92-377">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="22d92-377">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="22d92-378">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="22d92-378">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="22d92-379">Interactive</span><span class="sxs-lookup"><span data-stu-id="22d92-379">Interactive</span></span>

* <span data-ttu-id="22d92-380">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="22d92-380">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="22d92-381">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="22d92-381">Fixed errors on startup</span></span>
* <span data-ttu-id="22d92-382">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="22d92-382">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="22d92-383">IoT</span><span class="sxs-lookup"><span data-stu-id="22d92-383">IoT</span></span>

* <span data-ttu-id="22d92-384">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="22d92-384">Added support for device provisioning service</span></span>
* <span data-ttu-id="22d92-385">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="22d92-385">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="22d92-386">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="22d92-386">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-387">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-387">Monitor</span></span>

* <span data-ttu-id="22d92-388">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="22d92-388">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="22d92-389">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="22d92-389">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="22d92-390">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="22d92-390">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="22d92-391">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-391">Network</span></span>

* <span data-ttu-id="22d92-392">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="22d92-392">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="22d92-393">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-393">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-394">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-394">Profile</span></span>

* <span data-ttu-id="22d92-395">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="22d92-395">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="22d92-396">Rol</span><span class="sxs-lookup"><span data-stu-id="22d92-396">Role</span></span>

* <span data-ttu-id="22d92-397">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="22d92-397">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="22d92-398">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="22d92-398">Service Fabric</span></span>

* <span data-ttu-id="22d92-399">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="22d92-399">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="22d92-400">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="22d92-400">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-401">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-401">VM</span></span>

* <span data-ttu-id="22d92-402">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="22d92-402">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="22d92-403">[[CAMBIO IMPORTANTE]] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="22d92-403">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="22d92-404">[[CAMBIO IMPORTANTE]] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="22d92-404">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="22d92-405">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="22d92-405">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="22d92-406">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="22d92-406">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="22d92-407">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="22d92-407">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="22d92-408">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="22d92-408">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="22d92-409">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="22d92-409">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="22d92-410">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-410">December 19, 2017</span></span>

<span data-ttu-id="22d92-411">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="22d92-411">Version 2.0.23</span></span>

* <span data-ttu-id="22d92-412">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="22d92-412">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="22d92-413">Contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-413">Container</span></span>

* <span data-ttu-id="22d92-414">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-414">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="22d92-415">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-415">Network</span></span>

* <span data-ttu-id="22d92-416">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-416">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="22d92-417">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-417">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-418">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-418">Storage</span></span>

* <span data-ttu-id="22d92-419">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="22d92-419">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-420">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-420">VM</span></span>

* <span data-ttu-id="22d92-421">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="22d92-421">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="22d92-422">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-422">December 5, 2017</span></span>

<span data-ttu-id="22d92-423">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="22d92-423">Version 2.0.22</span></span>

* <span data-ttu-id="22d92-424">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="22d92-424">Removed `az component` commands.</span></span> <span data-ttu-id="22d92-425">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="22d92-425">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="22d92-426">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-426">Core</span></span>
* <span data-ttu-id="22d92-427">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="22d92-427">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="22d92-428">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="22d92-428">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-429">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-429">ACS</span></span>

* <span data-ttu-id="22d92-430">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="22d92-430">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="22d92-431">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="22d92-431">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="22d92-432">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="22d92-432">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="22d92-433">Advisor</span><span class="sxs-lookup"><span data-stu-id="22d92-433">Advisor</span></span>

* <span data-ttu-id="22d92-434">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="22d92-434">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-435">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-435">Appservice</span></span>

* <span data-ttu-id="22d92-436">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="22d92-436">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="22d92-437">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="22d92-437">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="22d92-438">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="22d92-438">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="22d92-439">Consumo</span><span class="sxs-lookup"><span data-stu-id="22d92-439">Consumption</span></span>

* <span data-ttu-id="22d92-440">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="22d92-440">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="22d92-441">Contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-441">Container</span></span>

* <span data-ttu-id="22d92-442">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="22d92-442">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-443">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-443">Monitor</span></span>

* <span data-ttu-id="22d92-444">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="22d92-444">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-445">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-445">Resource</span></span>

* <span data-ttu-id="22d92-446">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="22d92-446">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="22d92-447">Rol</span><span class="sxs-lookup"><span data-stu-id="22d92-447">Role</span></span>

* <span data-ttu-id="22d92-448">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="22d92-448">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="22d92-449">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="22d92-449">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="22d92-450">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="22d92-450">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-451">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-451">SQL</span></span>

* <span data-ttu-id="22d92-452">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="22d92-452">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="22d92-453">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="22d92-453">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-454">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-454">VM</span></span>

* <span data-ttu-id="22d92-455">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="22d92-455">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="22d92-456">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-456">November 14, 2017</span></span>

<span data-ttu-id="22d92-457">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="22d92-457">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="22d92-458">ACR</span><span class="sxs-lookup"><span data-stu-id="22d92-458">ACR</span></span>

* <span data-ttu-id="22d92-459">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="22d92-459">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="22d92-460">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-460">ACS</span></span>

* <span data-ttu-id="22d92-461">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="22d92-461">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="22d92-462">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="22d92-462">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="22d92-463">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="22d92-463">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="22d92-464">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="22d92-464">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="22d92-465">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="22d92-465">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-466">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-466">Appservice</span></span>

* <span data-ttu-id="22d92-467">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="22d92-467">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="22d92-468">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="22d92-468">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="22d92-469">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="22d92-469">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="22d92-470">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="22d92-470">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="22d92-471">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="22d92-471">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="22d92-472">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="22d92-472">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="22d92-473">Batch</span><span class="sxs-lookup"><span data-stu-id="22d92-473">Batch</span></span>

* <span data-ttu-id="22d92-474">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="22d92-474">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="22d92-475">Batchai</span><span class="sxs-lookup"><span data-stu-id="22d92-475">Batchai</span></span>

* <span data-ttu-id="22d92-476">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="22d92-476">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="22d92-477">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="22d92-477">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="22d92-478">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="22d92-478">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="22d92-479">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="22d92-479">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="22d92-480">Nube</span><span class="sxs-lookup"><span data-stu-id="22d92-480">Cloud</span></span>

* <span data-ttu-id="22d92-481">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="22d92-481">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="22d92-482">Contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-482">Container</span></span>

* <span data-ttu-id="22d92-483">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="22d92-483">Added support to open multiple ports</span></span>
* <span data-ttu-id="22d92-484">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="22d92-484">Added container group restart policy</span></span>
* <span data-ttu-id="22d92-485">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="22d92-485">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="22d92-486">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="22d92-486">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="22d92-487">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="22d92-487">Data Lake Analytics</span></span>

* <span data-ttu-id="22d92-488">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="22d92-488">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="22d92-489">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="22d92-489">Data Lake Store</span></span>

* <span data-ttu-id="22d92-490">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="22d92-490">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="22d92-491">Extensión</span><span class="sxs-lookup"><span data-stu-id="22d92-491">Extension</span></span>

* <span data-ttu-id="22d92-492">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="22d92-492">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="22d92-493">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="22d92-493">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="22d92-494">IoT</span><span class="sxs-lookup"><span data-stu-id="22d92-494">IoT</span></span>

* <span data-ttu-id="22d92-495">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="22d92-495">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-496">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-496">Monitor</span></span>

* <span data-ttu-id="22d92-497">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="22d92-497">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="22d92-498">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-498">Network</span></span>

* <span data-ttu-id="22d92-499">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="22d92-499">Added support for CAA DNS records</span></span>
* <span data-ttu-id="22d92-500">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="22d92-500">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="22d92-501">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-501">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="22d92-502">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="22d92-502">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="22d92-503">Reservations</span><span class="sxs-lookup"><span data-stu-id="22d92-503">Reservations</span></span>

* <span data-ttu-id="22d92-504">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="22d92-504">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-505">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-505">Resource</span></span>

* <span data-ttu-id="22d92-506">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-506">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-507">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-507">SQL</span></span>

* <span data-ttu-id="22d92-508">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-508">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-509">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-509">Storage</span></span>

* <span data-ttu-id="22d92-510">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="22d92-510">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="22d92-511">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="22d92-511">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="22d92-512">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="22d92-512">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="22d92-513">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="22d92-513">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="22d92-514">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="22d92-514">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="22d92-515">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="22d92-515">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="22d92-516">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="22d92-516">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-517">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-517">VM</span></span>

* <span data-ttu-id="22d92-518">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="22d92-518">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="22d92-519">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="22d92-519">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="22d92-520">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="22d92-520">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="22d92-521">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="22d92-521">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="22d92-522">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="22d92-522">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="22d92-523">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-523">October 24, 2017</span></span>

<span data-ttu-id="22d92-524">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="22d92-524">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="22d92-525">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-525">Core</span></span>

* <span data-ttu-id="22d92-526">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="22d92-526">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="22d92-527">ACR</span><span class="sxs-lookup"><span data-stu-id="22d92-527">ACR</span></span>

* <span data-ttu-id="22d92-528">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="22d92-528">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="22d92-529">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="22d92-529">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="22d92-530">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="22d92-530">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-531">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-531">ACS</span></span>

* <span data-ttu-id="22d92-532">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="22d92-532">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="22d92-533">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="22d92-533">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-534">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-534">Appservice</span></span>

* <span data-ttu-id="22d92-535">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="22d92-535">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="22d92-536">Componente</span><span class="sxs-lookup"><span data-stu-id="22d92-536">Component</span></span>

* <span data-ttu-id="22d92-537">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="22d92-537">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-538">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-538">Monitor</span></span>

* <span data-ttu-id="22d92-539">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="22d92-539">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-540">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-540">Resource</span></span>

* <span data-ttu-id="22d92-541">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="22d92-541">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="22d92-542">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="22d92-542">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-543">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-543">VM</span></span>

* <span data-ttu-id="22d92-544">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="22d92-544">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="22d92-545">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-545">October 9, 2017</span></span>

<span data-ttu-id="22d92-546">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="22d92-546">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="22d92-547">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-547">Core</span></span>

* <span data-ttu-id="22d92-548">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="22d92-548">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-549">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-549">Appservice</span></span>

* <span data-ttu-id="22d92-550">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="22d92-550">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="22d92-551">Batch</span><span class="sxs-lookup"><span data-stu-id="22d92-551">Batch</span></span>

* <span data-ttu-id="22d92-552">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="22d92-552">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="22d92-553">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="22d92-553">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="22d92-554">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="22d92-554">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="22d92-555">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="22d92-555">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="22d92-556">Batchai</span><span class="sxs-lookup"><span data-stu-id="22d92-556">Batchai</span></span>

* <span data-ttu-id="22d92-557">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="22d92-557">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="22d92-558">Keyvault</span><span class="sxs-lookup"><span data-stu-id="22d92-558">Keyvault</span></span>

* <span data-ttu-id="22d92-559">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="22d92-559">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="22d92-560">(#4448)</span><span class="sxs-lookup"><span data-stu-id="22d92-560">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="22d92-561">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-561">Network</span></span>

* <span data-ttu-id="22d92-562">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="22d92-562">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="22d92-563">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="22d92-563">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-564">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-564">Resource</span></span>

* <span data-ttu-id="22d92-565">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-565">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="22d92-566">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="22d92-566">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="22d92-567">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="22d92-567">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="22d92-568">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-568">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-569">Sql</span><span class="sxs-lookup"><span data-stu-id="22d92-569">Sql</span></span>

* <span data-ttu-id="22d92-570">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="22d92-570">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="22d92-571">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="22d92-571">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="22d92-572">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="22d92-572">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-573">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-573">Storage</span></span>

* <span data-ttu-id="22d92-574">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="22d92-574">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-575">Vm</span><span class="sxs-lookup"><span data-stu-id="22d92-575">Vm</span></span>

* <span data-ttu-id="22d92-576">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="22d92-576">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="22d92-577">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="22d92-577">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="22d92-578">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="22d92-578">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="22d92-579">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="22d92-579">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="22d92-580">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="22d92-580">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="22d92-581">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-581">September 22, 2017</span></span>

<span data-ttu-id="22d92-582">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="22d92-582">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-583">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-583">Resource</span></span>

* <span data-ttu-id="22d92-584">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="22d92-584">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="22d92-585">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="22d92-585">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="22d92-586">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="22d92-586">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="22d92-587">[[CAMBIO IMPORTANTE]] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="22d92-587">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="22d92-588">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-588">Network</span></span>

* <span data-ttu-id="22d92-589">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="22d92-589">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="22d92-590">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="22d92-590">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="22d92-591">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="22d92-591">Added `asg` application security group commands</span></span>
* <span data-ttu-id="22d92-592">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-592">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="22d92-593">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-593">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="22d92-594">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-594">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="22d92-595">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="22d92-595">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-596">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-596">Storage</span></span>

* <span data-ttu-id="22d92-597">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="22d92-597">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="22d92-598">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="22d92-598">Eventgrid</span></span>

* <span data-ttu-id="22d92-599">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="22d92-599">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-600">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-600">SQL</span></span>

* <span data-ttu-id="22d92-601">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="22d92-601">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="22d92-602">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="22d92-602">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="22d92-603">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-603">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="22d92-604">Keyvault</span><span class="sxs-lookup"><span data-stu-id="22d92-604">Keyvault</span></span>

* <span data-ttu-id="22d92-605">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="22d92-605">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-606">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-606">VM</span></span>

* <span data-ttu-id="22d92-607">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="22d92-607">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="22d92-608">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="22d92-608">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="22d92-609">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="22d92-609">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="22d92-610">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="22d92-610">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="22d92-611">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="22d92-611">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="22d92-612">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="22d92-612">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-613">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-613">ACS</span></span>

* <span data-ttu-id="22d92-614">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-614">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-615">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-615">Appservice</span></span>

* <span data-ttu-id="22d92-616">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="22d92-616">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="22d92-617">Backup</span><span class="sxs-lookup"><span data-stu-id="22d92-617">Backup</span></span>

* <span data-ttu-id="22d92-618">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="22d92-618">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="22d92-619">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-619">September 11, 2017</span></span>

<span data-ttu-id="22d92-620">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="22d92-620">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="22d92-621">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-621">Core</span></span>

* <span data-ttu-id="22d92-622">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="22d92-622">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="22d92-623">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="22d92-623">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-624">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-624">Acs</span></span>

* <span data-ttu-id="22d92-625">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="22d92-625">Added `acs list-locations` command</span></span>
* <span data-ttu-id="22d92-626">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="22d92-626">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-627">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-627">Appservice</span></span>

* <span data-ttu-id="22d92-628">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="22d92-628">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="22d92-629">CDN</span><span class="sxs-lookup"><span data-stu-id="22d92-629">CDN</span></span>

* <span data-ttu-id="22d92-630">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="22d92-630">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="22d92-631">Extensión</span><span class="sxs-lookup"><span data-stu-id="22d92-631">Extension</span></span>

* <span data-ttu-id="22d92-632">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="22d92-632">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="22d92-633">Keyvault</span><span class="sxs-lookup"><span data-stu-id="22d92-633">Keyvault</span></span>

* <span data-ttu-id="22d92-634">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="22d92-634">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="22d92-635">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-635">Network</span></span>

* <span data-ttu-id="22d92-636">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="22d92-636">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="22d92-637">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-637">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="22d92-638">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-638">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="22d92-639">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-639">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="22d92-640">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-640">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-641">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-641">Resource</span></span>

* <span data-ttu-id="22d92-642">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-642">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="22d92-643">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-643">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="22d92-644">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="22d92-644">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="22d92-645">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="22d92-645">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-646">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-646">SQL</span></span>

* <span data-ttu-id="22d92-647">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="22d92-647">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-648">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-648">VM</span></span>

* <span data-ttu-id="22d92-649">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="22d92-649">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="22d92-650">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="22d92-650">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="22d92-651">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-651">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="22d92-652">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="22d92-652">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="22d92-653">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="22d92-653">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="22d92-654">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-654">August 31, 2017</span></span>

<span data-ttu-id="22d92-655">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="22d92-655">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="22d92-656">Keyvault</span><span class="sxs-lookup"><span data-stu-id="22d92-656">Keyvault</span></span>

* <span data-ttu-id="22d92-657">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="22d92-657">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="22d92-658">Sf</span><span class="sxs-lookup"><span data-stu-id="22d92-658">Sf</span></span>

* <span data-ttu-id="22d92-659">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="22d92-659">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-660">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-660">Storage</span></span>

* <span data-ttu-id="22d92-661">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="22d92-661">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="22d92-662">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="22d92-662">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="22d92-663">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-663">August 28, 2017</span></span>

<span data-ttu-id="22d92-664">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="22d92-664">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="22d92-665">CLI</span><span class="sxs-lookup"><span data-stu-id="22d92-665">CLI</span></span>

* <span data-ttu-id="22d92-666">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="22d92-666">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-667">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-667">ACS</span></span>

* <span data-ttu-id="22d92-668">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="22d92-668">Corrected preview regions</span></span>
* <span data-ttu-id="22d92-669">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="22d92-669">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="22d92-670">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="22d92-670">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-671">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-671">Appservice</span></span>

* <span data-ttu-id="22d92-672">[[CAMBIO IMPORTANTE]] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="22d92-672">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="22d92-673">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="22d92-673">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="22d92-674">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="22d92-674">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="22d92-675">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="22d92-675">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="22d92-676">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="22d92-676">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="22d92-677">IoT</span><span class="sxs-lookup"><span data-stu-id="22d92-677">IoT</span></span>

* <span data-ttu-id="22d92-678">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="22d92-678">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="22d92-679">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-679">Network</span></span>

* <span data-ttu-id="22d92-680">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="22d92-680">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="22d92-681">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="22d92-681">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="22d92-682">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="22d92-682">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="22d92-683">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-683">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="22d92-684">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-684">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-685">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-685">Profile</span></span>

* <span data-ttu-id="22d92-686">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="22d92-686">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="22d92-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="22d92-687">Service Fabric</span></span>

* <span data-ttu-id="22d92-688">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="22d92-688">Preview release</span></span>
* <span data-ttu-id="22d92-689">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="22d92-689">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="22d92-690">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="22d92-690">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="22d92-691">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="22d92-691">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-692">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-692">Storage</span></span>

* <span data-ttu-id="22d92-693">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="22d92-693">Enabled setting blob tier</span></span>
* <span data-ttu-id="22d92-694">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="22d92-694">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="22d92-695">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="22d92-695">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="22d92-696">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="22d92-696">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="22d92-697">[[CAMBIO IMPORTANTE]] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="22d92-697">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="22d92-698">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="22d92-698">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-699">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-699">VM</span></span>

* <span data-ttu-id="22d92-700">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="22d92-700">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="22d92-701">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-701">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="22d92-702">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-702">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="22d92-703">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="22d92-703">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="22d92-704">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="22d92-704">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="22d92-705">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-705">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="22d92-706">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-706">August 15, 2017</span></span>

<span data-ttu-id="22d92-707">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="22d92-707">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-708">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-708">ACS</span></span>

* <span data-ttu-id="22d92-709">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="22d92-709">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-710">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-710">Appservice</span></span>

* <span data-ttu-id="22d92-711">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="22d92-711">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="22d92-712">Event Grid</span><span class="sxs-lookup"><span data-stu-id="22d92-712">Event Grid</span></span>

* <span data-ttu-id="22d92-713">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="22d92-713">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="22d92-714">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-714">August 11, 2017</span></span>

<span data-ttu-id="22d92-715">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="22d92-715">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-716">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-716">ACS</span></span>

* <span data-ttu-id="22d92-717">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="22d92-717">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="22d92-718">Batch</span><span class="sxs-lookup"><span data-stu-id="22d92-718">Batch</span></span>

* <span data-ttu-id="22d92-719">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="22d92-719">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="22d92-720">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="22d92-720">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="22d92-721">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="22d92-721">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="22d92-722">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="22d92-722">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="22d92-723">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="22d92-723">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="22d92-724">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="22d92-724">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="22d92-725">Componente</span><span class="sxs-lookup"><span data-stu-id="22d92-725">Component</span></span>

* <span data-ttu-id="22d92-726">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="22d92-726">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="22d92-727">Contenedor</span><span class="sxs-lookup"><span data-stu-id="22d92-727">Container</span></span>

* <span data-ttu-id="22d92-728">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="22d92-728">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="22d92-729">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="22d92-729">Data Lake Store</span></span>

* <span data-ttu-id="22d92-730">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="22d92-730">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="22d92-731">Event Grid</span><span class="sxs-lookup"><span data-stu-id="22d92-731">Event Grid</span></span>

* <span data-ttu-id="22d92-732">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="22d92-732">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="22d92-733">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-733">Network</span></span>

* <span data-ttu-id="22d92-734">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="22d92-734">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="22d92-735">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="22d92-735">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="22d92-736">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="22d92-736">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="22d92-737">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="22d92-737">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-738">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-738">Profile</span></span>

* <span data-ttu-id="22d92-739">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="22d92-739">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-740">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-740">Storage</span></span>

* <span data-ttu-id="22d92-741">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="22d92-741">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-742">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-742">VM</span></span>

* <span data-ttu-id="22d92-743">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="22d92-743">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="22d92-744">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="22d92-744">Exposed `list-skus` command</span></span>
* <span data-ttu-id="22d92-745">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="22d92-745">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="22d92-746">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="22d92-746">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="22d92-747">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="22d92-747">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="22d92-748">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-748">July 28, 2017</span></span>

<span data-ttu-id="22d92-749">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="22d92-749">Version 2.0.12</span></span>

* <span data-ttu-id="22d92-750">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="22d92-750">Added container commands</span></span>
* <span data-ttu-id="22d92-751">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="22d92-751">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="22d92-752">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-752">Core</span></span>

* <span data-ttu-id="22d92-753">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="22d92-753">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="22d92-754">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="22d92-754">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="22d92-755">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="22d92-755">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="22d92-756">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="22d92-756">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="22d92-757">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="22d92-757">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="22d92-758">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="22d92-758">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="22d92-759">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="22d92-759">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="22d92-760">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="22d92-760">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="22d92-761">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="22d92-761">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="22d92-762">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="22d92-762">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="22d92-763">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="22d92-763">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="22d92-764">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="22d92-764">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="22d92-765">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="22d92-765">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="22d92-766">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="22d92-766">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="22d92-767">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="22d92-767">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="22d92-768">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="22d92-768">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="22d92-769">ACR</span><span class="sxs-lookup"><span data-stu-id="22d92-769">ACR</span></span>

* <span data-ttu-id="22d92-770">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="22d92-770">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="22d92-771">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="22d92-771">Support SKU update for managed registries</span></span>
* <span data-ttu-id="22d92-772">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="22d92-772">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="22d92-773">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="22d92-773">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="22d92-774">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="22d92-774">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="22d92-775">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="22d92-775">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-776">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-776">ACS</span></span>

* <span data-ttu-id="22d92-777">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="22d92-777">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-778">Appservice</span><span class="sxs-lookup"><span data-stu-id="22d92-778">Appservice</span></span>

* <span data-ttu-id="22d92-779">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="22d92-779">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="22d92-780">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="22d92-780">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="22d92-781">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="22d92-781">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="22d92-782">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="22d92-782">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="22d92-783">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="22d92-783">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="22d92-784">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="22d92-784">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="22d92-785">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="22d92-785">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="22d92-786">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="22d92-786">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="22d92-787">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="22d92-787">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="22d92-788">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="22d92-788">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="22d92-789">Batch</span><span class="sxs-lookup"><span data-stu-id="22d92-789">Batch</span></span>

* <span data-ttu-id="22d92-790">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="22d92-790">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="22d92-791">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="22d92-791">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="22d92-792">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-792">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="22d92-793">CDN</span><span class="sxs-lookup"><span data-stu-id="22d92-793">CDN</span></span>

* <span data-ttu-id="22d92-794">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="22d92-794">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="22d92-795">Nube</span><span class="sxs-lookup"><span data-stu-id="22d92-795">Cloud</span></span>

* <span data-ttu-id="22d92-796">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="22d92-796">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="22d92-797">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="22d92-797">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="22d92-798">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="22d92-798">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="22d92-799">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="22d92-799">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="22d92-800">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="22d92-800">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="22d92-801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="22d92-801">CosmosDB</span></span>

* <span data-ttu-id="22d92-802">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="22d92-802">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="22d92-803">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="22d92-803">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="22d92-804">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="22d92-804">Data Lake Analytics</span></span>

* <span data-ttu-id="22d92-805">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="22d92-805">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="22d92-806">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="22d92-806">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="22d92-807">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="22d92-807">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="22d92-808">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="22d92-808">Data Lake Store</span></span>

* <span data-ttu-id="22d92-809">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-809">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="22d92-810">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="22d92-810">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="22d92-811">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="22d92-811">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="22d92-812">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="22d92-812">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="22d92-813">Interactive</span><span class="sxs-lookup"><span data-stu-id="22d92-813">Interactive</span></span>

* <span data-ttu-id="22d92-814">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="22d92-814">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="22d92-815">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="22d92-815">Increased test coverage</span></span>
* <span data-ttu-id="22d92-816">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="22d92-816">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="22d92-817">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="22d92-817">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="22d92-818">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="22d92-818">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="22d92-819">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="22d92-819">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="22d92-820">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="22d92-820">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="22d92-821">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="22d92-821">Added `--progress` flag</span></span>
* <span data-ttu-id="22d92-822">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="22d92-822">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="22d92-823">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="22d92-823">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="22d92-824">IoT</span><span class="sxs-lookup"><span data-stu-id="22d92-824">IoT</span></span>

* <span data-ttu-id="22d92-825">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="22d92-825">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="22d92-826">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="22d92-826">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="22d92-827">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="22d92-827">Key vault</span></span>

* <span data-ttu-id="22d92-828">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="22d92-828">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="22d92-829">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="22d92-829">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="22d92-830">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="22d92-830">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="22d92-831">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="22d92-831">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="22d92-832">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="22d92-832">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="22d92-833">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="22d92-833">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="22d92-834">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="22d92-834">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="22d92-835">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="22d92-835">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="22d92-836">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-836">Lab</span></span>

* <span data-ttu-id="22d92-837">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="22d92-837">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="22d92-838">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="22d92-838">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-839">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-839">Monitor</span></span>

* <span data-ttu-id="22d92-840">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="22d92-840">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="22d92-841">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="22d92-841">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="22d92-842">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="22d92-842">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="22d92-843">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="22d92-843">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="22d92-844">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="22d92-844">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="22d92-845">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="22d92-845">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="22d92-846">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="22d92-846">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="22d92-847">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="22d92-847">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="22d92-848">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="22d92-848">`location` no longer required</span></span>
  * <span data-ttu-id="22d92-849">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="22d92-849">Add name and ID support for target</span></span>
  * <span data-ttu-id="22d92-850">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="22d92-850">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="22d92-851">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="22d92-851">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="22d92-852">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="22d92-852">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="22d92-853">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="22d92-853">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="22d92-854">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="22d92-854">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="22d92-855">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="22d92-855">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="22d92-856">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-856">Network</span></span>

* <span data-ttu-id="22d92-857">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="22d92-857">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="22d92-858">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-858">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="22d92-859">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="22d92-859">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="22d92-860">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="22d92-860">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="22d92-861">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-861">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="22d92-862">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="22d92-862">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="22d92-863">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="22d92-863">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="22d92-864">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="22d92-864">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="22d92-865">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="22d92-865">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="22d92-866">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="22d92-866">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="22d92-867">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="22d92-867">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="22d92-868">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="22d92-868">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="22d92-869">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="22d92-869">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="22d92-870">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-870">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="22d92-871">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-871">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="22d92-872">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-872">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="22d92-873">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="22d92-873">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="22d92-874">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="22d92-874">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="22d92-875">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-875">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="22d92-876">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-876">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="22d92-877">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-877">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="22d92-878">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="22d92-878">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="22d92-879">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="22d92-879">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="22d92-880">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="22d92-880">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="22d92-881">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="22d92-881">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="22d92-882">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="22d92-882">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="22d92-883">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="22d92-883">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-884">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-884">Profile</span></span>

* <span data-ttu-id="22d92-885">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="22d92-885">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="22d92-886">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="22d92-886">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="22d92-887">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="22d92-887">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="22d92-888">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="22d92-888">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="22d92-889">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="22d92-889">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="22d92-890">RDBMS</span><span class="sxs-lookup"><span data-stu-id="22d92-890">RDBMS</span></span>

* <span data-ttu-id="22d92-891">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="22d92-891">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="22d92-892">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="22d92-892">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="22d92-893">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="22d92-893">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="22d92-894">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="22d92-894">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-895">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-895">Resource</span></span>

* <span data-ttu-id="22d92-896">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-896">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="22d92-897">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="22d92-897">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="22d92-898">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="22d92-898">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="22d92-899">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="22d92-899">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="22d92-900">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="22d92-900">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="22d92-901">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="22d92-901">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="22d92-902">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="22d92-902">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="22d92-903">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="22d92-903">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="22d92-904">Rol</span><span class="sxs-lookup"><span data-stu-id="22d92-904">Role</span></span>

* <span data-ttu-id="22d92-905">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="22d92-905">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="22d92-906">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="22d92-906">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="22d92-907">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="22d92-907">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="22d92-908">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="22d92-908">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="22d92-909">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="22d92-909">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="22d92-910">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="22d92-910">Service Fabric</span></span>
* <span data-ttu-id="22d92-911">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="22d92-911">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="22d92-912">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="22d92-912">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="22d92-913">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="22d92-913">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-914">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-914">SQL</span></span>

* <span data-ttu-id="22d92-915">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="22d92-915">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="22d92-916">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="22d92-916">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="22d92-917">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="22d92-917">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-918">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-918">Storage</span></span>

* <span data-ttu-id="22d92-919">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="22d92-919">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="22d92-920">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="22d92-920">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="22d92-921">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="22d92-921">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="22d92-922">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="22d92-922">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="22d92-923">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="22d92-923">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="22d92-924">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="22d92-924">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-925">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-925">VM</span></span>

* <span data-ttu-id="22d92-926">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="22d92-926">Support configuring nsg</span></span>
* <span data-ttu-id="22d92-927">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="22d92-927">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="22d92-928">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="22d92-928">Support managed service identities</span></span>
* <span data-ttu-id="22d92-929">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="22d92-929">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="22d92-930">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="22d92-930">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="22d92-931">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-931">May 10, 2017</span></span>

<span data-ttu-id="22d92-932">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="22d92-932">Version 2.0.6</span></span>

* <span data-ttu-id="22d92-933">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="22d92-933">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="22d92-934">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="22d92-934">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="22d92-935">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="22d92-935">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="22d92-936">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="22d92-936">Include Cognitive Services module</span></span>
* <span data-ttu-id="22d92-937">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="22d92-937">Include Service Fabric module</span></span>
* <span data-ttu-id="22d92-938">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="22d92-938">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="22d92-939">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="22d92-939">Add support for CDN commands</span></span>
* <span data-ttu-id="22d92-940">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="22d92-940">Remove Container module</span></span>
* <span data-ttu-id="22d92-941">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="22d92-941">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="22d92-942">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="22d92-942">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="22d92-943">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-943">Core</span></span>

* <span data-ttu-id="22d92-944">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="22d92-944">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="22d92-945">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="22d92-945">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="22d92-946">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="22d92-946">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="22d92-947">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="22d92-947">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="22d92-948">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="22d92-948">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="22d92-949">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="22d92-949">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="22d92-950">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="22d92-950">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="22d92-951">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="22d92-951">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="22d92-952">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="22d92-952">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="22d92-953">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="22d92-953">core: Improved performance</span></span>
* <span data-ttu-id="22d92-954">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="22d92-954">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="22d92-955">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="22d92-955">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-956">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-956">ACS</span></span>

* <span data-ttu-id="22d92-957">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="22d92-957">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="22d92-958">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="22d92-958">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="22d92-959">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="22d92-959">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="22d92-960">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="22d92-960">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-961">AppService</span><span class="sxs-lookup"><span data-stu-id="22d92-961">AppService</span></span>

* <span data-ttu-id="22d92-962">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="22d92-962">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="22d92-963">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="22d92-963">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="22d92-964">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="22d92-964">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="22d92-965">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="22d92-965">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="22d92-966">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="22d92-966">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="22d92-967">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="22d92-967">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="22d92-968">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="22d92-968">support slot swap with preview</span></span>
* <span data-ttu-id="22d92-969">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="22d92-969">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="22d92-970">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="22d92-970">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="22d92-971">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="22d92-971">CosmosDB</span></span>

* <span data-ttu-id="22d92-972">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="22d92-972">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="22d92-973">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="22d92-973">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="22d92-974">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="22d92-974">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="22d92-975">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="22d92-975">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="22d92-976">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="22d92-976">Data Lake Analytics</span></span>

* <span data-ttu-id="22d92-977">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="22d92-977">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="22d92-978">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="22d92-978">Add support for new catalog item type: package.</span></span> <span data-ttu-id="22d92-979">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="22d92-979">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="22d92-980">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="22d92-980">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="22d92-981">Tabla</span><span class="sxs-lookup"><span data-stu-id="22d92-981">Table</span></span>
  * <span data-ttu-id="22d92-982">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="22d92-982">Table valued function</span></span>
  * <span data-ttu-id="22d92-983">Ver</span><span class="sxs-lookup"><span data-stu-id="22d92-983">View</span></span>
  * <span data-ttu-id="22d92-984">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="22d92-984">Table Statistics.</span></span> <span data-ttu-id="22d92-985">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="22d92-985">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="22d92-986">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="22d92-986">Data Lake Store</span></span>

* <span data-ttu-id="22d92-987">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="22d92-987">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="22d92-988">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="22d92-988">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="22d92-989">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="22d92-989">missed help for access show.</span></span> <span data-ttu-id="22d92-990">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="22d92-990">adding it.</span></span> <span data-ttu-id="22d92-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="22d92-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="22d92-992">Buscar</span><span class="sxs-lookup"><span data-stu-id="22d92-992">Find</span></span>

* <span data-ttu-id="22d92-993">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="22d92-993">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="22d92-994">KeyVault</span><span class="sxs-lookup"><span data-stu-id="22d92-994">KeyVault</span></span>

* <span data-ttu-id="22d92-995">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="22d92-995">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="22d92-996">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="22d92-996">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="22d92-997">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="22d92-997">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="22d92-998">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="22d92-998">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="22d92-999">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="22d92-999">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="22d92-1000">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-1000">Lab</span></span>

* <span data-ttu-id="22d92-1001">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-1001">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="22d92-1002">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-1002">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="22d92-1003">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-1003">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="22d92-1004">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-1004">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="22d92-1005">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="22d92-1005">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="22d92-1006">Supervisión</span><span class="sxs-lookup"><span data-stu-id="22d92-1006">Monitor</span></span>

* <span data-ttu-id="22d92-1007">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="22d92-1007">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="22d92-1008">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="22d92-1008">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="22d92-1009">Red</span><span class="sxs-lookup"><span data-stu-id="22d92-1009">Network</span></span>

* <span data-ttu-id="22d92-1010">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="22d92-1010">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="22d92-1011">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="22d92-1011">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="22d92-1012">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="22d92-1012">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="22d92-1013">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="22d92-1013">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="22d92-1014">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="22d92-1014">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="22d92-1015">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="22d92-1015">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="22d92-1016">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="22d92-1016">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="22d92-1017">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="22d92-1017">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="22d92-1018">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="22d92-1018">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="22d92-1019">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="22d92-1019">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="22d92-1020">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="22d92-1020">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="22d92-1021">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="22d92-1021">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="22d92-1022">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="22d92-1022">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="22d92-1023">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="22d92-1023">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="22d92-1024">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="22d92-1024">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="22d92-1025">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="22d92-1025">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="22d92-1026">Perfil</span><span class="sxs-lookup"><span data-stu-id="22d92-1026">Profile</span></span>

* <span data-ttu-id="22d92-1027">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="22d92-1027">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="22d92-1028">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="22d92-1028">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="22d92-1029">Redis</span><span class="sxs-lookup"><span data-stu-id="22d92-1029">Redis</span></span>

* <span data-ttu-id="22d92-1030">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="22d92-1030">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="22d92-1031">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="22d92-1031">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="22d92-1032">Recurso</span><span class="sxs-lookup"><span data-stu-id="22d92-1032">Resource</span></span>

* <span data-ttu-id="22d92-1033">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="22d92-1033">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="22d92-1034">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="22d92-1034">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="22d92-1035">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="22d92-1035">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="22d92-1036">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="22d92-1036">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="22d92-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="22d92-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="22d92-1038">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="22d92-1038">Add docs for az lock update.</span></span> <span data-ttu-id="22d92-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="22d92-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="22d92-1040">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="22d92-1040">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="22d92-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="22d92-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="22d92-1042">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="22d92-1042">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="22d92-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="22d92-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="22d92-1044">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="22d92-1044">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="22d92-1045">Rol</span><span class="sxs-lookup"><span data-stu-id="22d92-1045">Role</span></span>

* <span data-ttu-id="22d92-1046">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="22d92-1046">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="22d92-1047">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="22d92-1047">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="22d92-1048">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="22d92-1048">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="22d92-1049">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="22d92-1049">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="22d92-1050">SQL</span><span class="sxs-lookup"><span data-stu-id="22d92-1050">SQL</span></span>

* <span data-ttu-id="22d92-1051">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="22d92-1051">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="22d92-1052">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="22d92-1052">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="22d92-1053">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-1053">Storage</span></span>

* <span data-ttu-id="22d92-1054">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="22d92-1054">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="22d92-1055">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="22d92-1055">Add support for incremental blob copy</span></span>
* <span data-ttu-id="22d92-1056">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="22d92-1056">Add support for large block blob upload</span></span>
* <span data-ttu-id="22d92-1057">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="22d92-1057">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-1058">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-1058">VM</span></span>

* <span data-ttu-id="22d92-1059">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="22d92-1059">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="22d92-1060">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="22d92-1060">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="22d92-1061">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="22d92-1061">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="22d92-1062">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="22d92-1062">az vm/vmss disk</span></span>
  3. <span data-ttu-id="22d92-1063">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="22d92-1063">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="22d92-1064">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="22d92-1064">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="22d92-1065">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="22d92-1065">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="22d92-1066">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-1066">April 3, 2017</span></span>

<span data-ttu-id="22d92-1067">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="22d92-1067">Version 2.0.2</span></span>

<span data-ttu-id="22d92-1068">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="22d92-1068">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="22d92-1069">Núcleo</span><span class="sxs-lookup"><span data-stu-id="22d92-1069">Core</span></span>

* <span data-ttu-id="22d92-1070">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="22d92-1070">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="22d92-1071">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="22d92-1071">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="22d92-1072">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="22d92-1072">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="22d92-1073">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="22d92-1073">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="22d92-1074">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="22d92-1074">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="22d92-1075">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="22d92-1075">Add prompting for missing template parameters.</span></span> <span data-ttu-id="22d92-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="22d92-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="22d92-1077">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="22d92-1077">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="22d92-1078">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="22d92-1078">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="22d92-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="22d92-1079">ACS</span></span>

* <span data-ttu-id="22d92-1080">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="22d92-1080">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="22d92-1081">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="22d92-1081">Add support for ssh key password prompting.</span></span> <span data-ttu-id="22d92-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="22d92-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="22d92-1083">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="22d92-1083">Add support for windows clusters.</span></span> <span data-ttu-id="22d92-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="22d92-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="22d92-1085">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="22d92-1085">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="22d92-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="22d92-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="22d92-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="22d92-1087">AppService</span></span>

* <span data-ttu-id="22d92-1088">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="22d92-1088">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="22d92-1089">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="22d92-1089">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="22d92-1090">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="22d92-1090">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="22d92-1091">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="22d92-1091">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="22d92-1092">DataLake</span><span class="sxs-lookup"><span data-stu-id="22d92-1092">DataLake</span></span>

* <span data-ttu-id="22d92-1093">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="22d92-1093">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="22d92-1094">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="22d92-1094">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="22d92-1095">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="22d92-1095">DocuemntDB</span></span>

* <span data-ttu-id="22d92-1096">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="22d92-1096">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="22d92-1097">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="22d92-1097">VM</span></span>

* <span data-ttu-id="22d92-1098">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="22d92-1098">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="22d92-1099">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="22d92-1099">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="22d92-1100">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="22d92-1100">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="22d92-1101">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="22d92-1101">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="22d92-1102">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="22d92-1102">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="22d92-1103">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="22d92-1103">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="22d92-1104">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="22d92-1104">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="22d92-1105">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="22d92-1105">February 27, 2017</span></span>

<span data-ttu-id="22d92-1106">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="22d92-1106">Version 2.0.0</span></span>

<span data-ttu-id="22d92-1107">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="22d92-1107">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="22d92-1108">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="22d92-1108">Container Service (acs)</span></span>
- <span data-ttu-id="22d92-1109">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="22d92-1109">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="22d92-1110">Redes</span><span class="sxs-lookup"><span data-stu-id="22d92-1110">Networking</span></span>
- <span data-ttu-id="22d92-1111">Storage</span><span class="sxs-lookup"><span data-stu-id="22d92-1111">Storage</span></span>

<span data-ttu-id="22d92-1112">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="22d92-1112">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="22d92-1113">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="22d92-1113">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="22d92-1114">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="22d92-1114">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="22d92-1115">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="22d92-1115">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="22d92-1116">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="22d92-1116">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="22d92-1117">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="22d92-1117">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="22d92-1118">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="22d92-1118">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="22d92-1119">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="22d92-1119">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="22d92-1120">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="22d92-1120">Provide feedback from the command line with the `az feedback` command</span></span>

