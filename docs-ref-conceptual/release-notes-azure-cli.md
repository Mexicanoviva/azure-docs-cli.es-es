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
ms.openlocfilehash: 116fa95e51399b9b97c1b35c38445f30db7efc94
ms.sourcegitcommit: fefb5bb6a21cab30c44592c0577408a8d1a2ccc7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/17/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="12960-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="12960-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="12960-104">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="12960-104">March 13, 2018</span></span>

<span data-ttu-id="12960-105">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="12960-105">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="12960-106">ACR</span><span class="sxs-lookup"><span data-stu-id="12960-106">ACR</span></span>

* <span data-ttu-id="12960-107">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="12960-107">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="12960-108">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="12960-108">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="12960-109">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="12960-109">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="12960-110">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-110">ACS</span></span>

* <span data-ttu-id="12960-111">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="12960-111">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="12960-112">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="12960-112">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="12960-113">Advisor</span><span class="sxs-lookup"><span data-stu-id="12960-113">Advisor</span></span>

* <span data-ttu-id="12960-114">[NUEVO CAMBIO] Se cambió el nombre de `advisor configuration get` a `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="12960-114">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="12960-115">[NUEVO CAMBIO] Se cambió el nombre de `advisor configuration set` a `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="12960-115">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="12960-116">[NUEVO CAMBIO] Se ha quitado `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="12960-116">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="12960-117">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="12960-117">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="12960-118">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="12960-118">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-119">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-119">Appservice</span></span>

* <span data-ttu-id="12960-120">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="12960-120">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="12960-121">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="12960-121">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="12960-122">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="12960-122">Eventhubs</span></span>

* <span data-ttu-id="12960-123">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="12960-123">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="12960-124">Extensión</span><span class="sxs-lookup"><span data-stu-id="12960-124">Extension</span></span>

* <span data-ttu-id="12960-125">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="12960-125">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="12960-126">Interactive</span><span class="sxs-lookup"><span data-stu-id="12960-126">Interactive</span></span>

* <span data-ttu-id="12960-127">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="12960-127">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="12960-128">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="12960-128">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="12960-129">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="12960-129">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="12960-130">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="12960-130">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-131">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-131">Monitor</span></span>

* <span data-ttu-id="12960-132">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="12960-132">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="12960-133">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="12960-133">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="12960-134">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="12960-134">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="12960-135">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="12960-135">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="12960-136">Red</span><span class="sxs-lookup"><span data-stu-id="12960-136">Network</span></span>

* <span data-ttu-id="12960-137">[CAMBIO IMPORTANTE] Se ha quitado el parámetro `--tags` de `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="12960-137">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="12960-138">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="12960-138">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="12960-139">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="12960-139">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="12960-140">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="12960-140">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="12960-141">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-141">Profile</span></span>

* <span data-ttu-id="12960-142">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="12960-142">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="12960-143">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="12960-143">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="12960-144">RDBMS</span><span class="sxs-lookup"><span data-stu-id="12960-144">RDBMS</span></span>

* <span data-ttu-id="12960-145">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="12960-145">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="12960-146">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="12960-146">Service Bus</span></span>

* <span data-ttu-id="12960-147">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="12960-147">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="12960-148">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-148">Storage</span></span>

* <span data-ttu-id="12960-149">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="12960-149">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds.</span></span>
* <span data-ttu-id="12960-150">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="12960-150">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="12960-151">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-151">VM</span></span>

* <span data-ttu-id="12960-152">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="12960-152">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="12960-153">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="12960-153">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="12960-154">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="12960-154">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="12960-155">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="12960-155">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="12960-156">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="12960-156">February 27, 2018</span></span>

<span data-ttu-id="12960-157">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="12960-157">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="12960-158">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-158">Core</span></span>

* <span data-ttu-id="12960-159">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="12960-159">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="12960-160">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="12960-160">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="12960-161">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="12960-161">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="12960-162">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-162">ACS</span></span>

* <span data-ttu-id="12960-163">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="12960-163">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="12960-164">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="12960-164">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="12960-165">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="12960-165">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="12960-166">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="12960-166">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-167">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-167">Appservice</span></span>

* <span data-ttu-id="12960-168">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="12960-168">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="12960-169">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="12960-169">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="12960-170">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="12960-170">Cognitive Services</span></span>

* <span data-ttu-id="12960-171">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="12960-171">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="12960-172">Consumo</span><span class="sxs-lookup"><span data-stu-id="12960-172">Consumption</span></span>

* <span data-ttu-id="12960-173">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="12960-173">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="12960-174">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="12960-174">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="12960-175">Contenedor</span><span class="sxs-lookup"><span data-stu-id="12960-175">Container</span></span>

* <span data-ttu-id="12960-176">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="12960-176">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="12960-177">Red</span><span class="sxs-lookup"><span data-stu-id="12960-177">Network</span></span>

* <span data-ttu-id="12960-178">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="12960-178">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="12960-179">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-179">Resource</span></span>

* <span data-ttu-id="12960-180">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="12960-180">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="12960-181">Rol</span><span class="sxs-lookup"><span data-stu-id="12960-181">Role</span></span>

* <span data-ttu-id="12960-182">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="12960-182">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="12960-183">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-183">SQL</span></span>

* <span data-ttu-id="12960-184">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="12960-184">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="12960-185">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-185">Storage</span></span>

* <span data-ttu-id="12960-186">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="12960-186">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="12960-187">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-187">VM</span></span>

* <span data-ttu-id="12960-188">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="12960-188">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="12960-189">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="12960-189">February 13, 2018</span></span>

<span data-ttu-id="12960-190">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="12960-190">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="12960-191">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-191">Core</span></span>

* <span data-ttu-id="12960-192">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="12960-192">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="12960-193">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-193">ACS</span></span>

* <span data-ttu-id="12960-194">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="12960-194">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="12960-195">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="12960-195">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="12960-196">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="12960-196">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="12960-197">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="12960-197">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="12960-198">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="12960-198">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="12960-199">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="12960-199">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="12960-200">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="12960-200">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="12960-201">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="12960-201">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-202">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-202">Appservice</span></span>

* <span data-ttu-id="12960-203">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="12960-203">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="12960-204">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="12960-204">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="12960-205">CDN</span><span class="sxs-lookup"><span data-stu-id="12960-205">CDN</span></span>

* <span data-ttu-id="12960-206">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="12960-206">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="12960-207">Contenedor</span><span class="sxs-lookup"><span data-stu-id="12960-207">Container</span></span>

* <span data-ttu-id="12960-208">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="12960-208">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="12960-209">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="12960-209">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="12960-210">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="12960-210">CosmosDB</span></span>

* <span data-ttu-id="12960-211">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="12960-211">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="12960-212">Extensión</span><span class="sxs-lookup"><span data-stu-id="12960-212">Extension</span></span>

* <span data-ttu-id="12960-213">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-213">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="12960-214">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-214">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="12960-215">Comentarios</span><span class="sxs-lookup"><span data-stu-id="12960-215">Feedback</span></span>

* <span data-ttu-id="12960-216">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="12960-216">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="12960-217">Interactive</span><span class="sxs-lookup"><span data-stu-id="12960-217">Interactive</span></span>

* <span data-ttu-id="12960-218">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="12960-218">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="12960-219">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="12960-219">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="12960-220">IoT</span><span class="sxs-lookup"><span data-stu-id="12960-220">IoT</span></span>

* <span data-ttu-id="12960-221">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="12960-221">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="12960-222">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="12960-222">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="12960-223">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-223">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="12960-224">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="12960-224">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-225">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-225">Monitor</span></span>

* <span data-ttu-id="12960-226">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="12960-226">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="12960-227">Red</span><span class="sxs-lookup"><span data-stu-id="12960-227">Network</span></span>

* <span data-ttu-id="12960-228">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="12960-228">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="12960-229">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-229">Profile</span></span>

* <span data-ttu-id="12960-230">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="12960-230">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="12960-231">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-231">Resource</span></span>

* <span data-ttu-id="12960-232">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="12960-232">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="12960-233">Rol</span><span class="sxs-lookup"><span data-stu-id="12960-233">Role</span></span>

* <span data-ttu-id="12960-234">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="12960-234">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="12960-235">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-235">SQL</span></span>

* <span data-ttu-id="12960-236">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="12960-236">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="12960-237">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="12960-237">Added `sql db rename`</span></span>
* <span data-ttu-id="12960-238">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="12960-238">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="12960-239">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-239">Storage</span></span>

* <span data-ttu-id="12960-240">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="12960-240">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="12960-241">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-241">VM</span></span>

* <span data-ttu-id="12960-242">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="12960-242">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="12960-243">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="12960-243">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="12960-244">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="12960-244">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="12960-245">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="12960-245">January 31, 2018</span></span>

<span data-ttu-id="12960-246">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="12960-246">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="12960-247">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-247">Core</span></span>

* <span data-ttu-id="12960-248">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="12960-248">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="12960-249">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="12960-249">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="12960-250">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="12960-250">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="12960-251">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="12960-251">Use `--verbose` to see</span></span>
* <span data-ttu-id="12960-252">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="12960-252">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="12960-253">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-253">ACS</span></span>

* <span data-ttu-id="12960-254">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="12960-254">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="12960-255">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="12960-255">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-256">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-256">Appservice</span></span>

* <span data-ttu-id="12960-257">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="12960-257">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="12960-258">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="12960-258">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="12960-259">CDN</span><span class="sxs-lookup"><span data-stu-id="12960-259">CDN</span></span>

* <span data-ttu-id="12960-260">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="12960-260">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="12960-261">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="12960-261">CosmosDB</span></span>

* <span data-ttu-id="12960-262">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="12960-262">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="12960-263">Interactive</span><span class="sxs-lookup"><span data-stu-id="12960-263">Interactive</span></span>

* <span data-ttu-id="12960-264">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="12960-264">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="12960-265">Red</span><span class="sxs-lookup"><span data-stu-id="12960-265">Network</span></span>

* <span data-ttu-id="12960-266">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="12960-266">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="12960-267">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="12960-267">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="12960-268">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="12960-268">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="12960-269">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="12960-269">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="12960-270">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="12960-270">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="12960-271">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="12960-271">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="12960-272">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="12960-272">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="12960-273">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="12960-273">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="12960-274">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="12960-274">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="12960-275">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="12960-275">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="12960-276">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-276">Profile</span></span>

* <span data-ttu-id="12960-277">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="12960-277">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="12960-278">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-278">Resource</span></span>

* <span data-ttu-id="12960-279">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="12960-279">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="12960-280">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-280">Storage</span></span>

* <span data-ttu-id="12960-281">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="12960-281">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="12960-282">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="12960-282">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="12960-283">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="12960-283">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="12960-284">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="12960-284">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="12960-285">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="12960-285">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="12960-286">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-286">VM</span></span>

* <span data-ttu-id="12960-287">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="12960-287">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="12960-288">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="12960-288">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="12960-289">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="12960-289">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="12960-290">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="12960-290">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="12960-291">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="12960-291">January 17, 2018</span></span>

<span data-ttu-id="12960-292">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="12960-292">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="12960-293">ACR</span><span class="sxs-lookup"><span data-stu-id="12960-293">ACR</span></span>

* <span data-ttu-id="12960-294">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="12960-294">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="12960-295">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="12960-295">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="12960-296">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-296">ACS</span></span>

* <span data-ttu-id="12960-297">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="12960-297">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="12960-298">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="12960-298">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-299">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-299">Appservice</span></span>

* <span data-ttu-id="12960-300">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="12960-300">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="12960-301">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="12960-301">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="12960-302">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="12960-302">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="12960-303">Backup</span><span class="sxs-lookup"><span data-stu-id="12960-303">Backup</span></span>

* <span data-ttu-id="12960-304">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="12960-304">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="12960-305">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="12960-305">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="12960-306">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="12960-306">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="12960-307">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="12960-307">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="12960-308">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="12960-308">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="12960-309">Batch</span><span class="sxs-lookup"><span data-stu-id="12960-309">Batch</span></span>

* <span data-ttu-id="12960-310">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="12960-310">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="12960-311">Nube</span><span class="sxs-lookup"><span data-stu-id="12960-311">Cloud</span></span>

* <span data-ttu-id="12960-312">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="12960-312">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="12960-313">Consumo</span><span class="sxs-lookup"><span data-stu-id="12960-313">Consumption</span></span>

* <span data-ttu-id="12960-314">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="12960-314">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="12960-315">Event Grid</span><span class="sxs-lookup"><span data-stu-id="12960-315">Event Grid</span></span>

* <span data-ttu-id="12960-316">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="12960-316">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="12960-317">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="12960-317">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="12960-318">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="12960-318">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="12960-319">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="12960-319">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="12960-320">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="12960-320">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="12960-321">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="12960-321">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="12960-322">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="12960-322">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="12960-323">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="12960-323">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="12960-324">Interactive</span><span class="sxs-lookup"><span data-stu-id="12960-324">Interactive</span></span>

* <span data-ttu-id="12960-325">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="12960-325">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="12960-326">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="12960-326">Fixed errors on startup</span></span>
* <span data-ttu-id="12960-327">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="12960-327">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="12960-328">IoT</span><span class="sxs-lookup"><span data-stu-id="12960-328">IoT</span></span>

* <span data-ttu-id="12960-329">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="12960-329">Added support for device provisioning service</span></span>
* <span data-ttu-id="12960-330">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="12960-330">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="12960-331">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="12960-331">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-332">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-332">Monitor</span></span>

* <span data-ttu-id="12960-333">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="12960-333">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="12960-334">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="12960-334">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="12960-335">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="12960-335">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="12960-336">Red</span><span class="sxs-lookup"><span data-stu-id="12960-336">Network</span></span>

* <span data-ttu-id="12960-337">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="12960-337">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="12960-338">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-338">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="12960-339">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-339">Profile</span></span>

* <span data-ttu-id="12960-340">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="12960-340">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="12960-341">Rol</span><span class="sxs-lookup"><span data-stu-id="12960-341">Role</span></span>

* <span data-ttu-id="12960-342">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="12960-342">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="12960-343">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="12960-343">Service Fabric</span></span>

* <span data-ttu-id="12960-344">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="12960-344">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="12960-345">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="12960-345">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="12960-346">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-346">VM</span></span>

* <span data-ttu-id="12960-347">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="12960-347">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="12960-348">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado del `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="12960-348">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="12960-349">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="12960-349">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="12960-350">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="12960-350">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="12960-351">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="12960-351">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="12960-352">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="12960-352">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="12960-353">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="12960-353">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="12960-354">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="12960-354">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="12960-355">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-355">December 19, 2017</span></span>

<span data-ttu-id="12960-356">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="12960-356">Version 2.0.23</span></span>

* <span data-ttu-id="12960-357">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="12960-357">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="12960-358">Contenedor</span><span class="sxs-lookup"><span data-stu-id="12960-358">Container</span></span>

* <span data-ttu-id="12960-359">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="12960-359">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="12960-360">Red</span><span class="sxs-lookup"><span data-stu-id="12960-360">Network</span></span>

* <span data-ttu-id="12960-361">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-361">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="12960-362">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-362">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="12960-363">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-363">Storage</span></span>

* <span data-ttu-id="12960-364">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="12960-364">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="12960-365">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-365">VM</span></span>

* <span data-ttu-id="12960-366">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="12960-366">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="12960-367">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-367">December 5, 2017</span></span>

<span data-ttu-id="12960-368">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="12960-368">Version 2.0.22</span></span>

* <span data-ttu-id="12960-369">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="12960-369">Removed `az component` commands.</span></span> <span data-ttu-id="12960-370">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="12960-370">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="12960-371">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-371">Core</span></span>
* <span data-ttu-id="12960-372">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="12960-372">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="12960-373">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="12960-373">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="12960-374">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-374">ACS</span></span>

* <span data-ttu-id="12960-375">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="12960-375">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="12960-376">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="12960-376">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="12960-377">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="12960-377">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="12960-378">Advisor</span><span class="sxs-lookup"><span data-stu-id="12960-378">Advisor</span></span>

* <span data-ttu-id="12960-379">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="12960-379">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-380">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-380">Appservice</span></span>

* <span data-ttu-id="12960-381">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="12960-381">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="12960-382">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="12960-382">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="12960-383">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="12960-383">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="12960-384">Consumo</span><span class="sxs-lookup"><span data-stu-id="12960-384">Consumption</span></span>

* <span data-ttu-id="12960-385">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="12960-385">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="12960-386">Contenedor</span><span class="sxs-lookup"><span data-stu-id="12960-386">Container</span></span>

* <span data-ttu-id="12960-387">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="12960-387">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-388">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-388">Monitor</span></span>

* <span data-ttu-id="12960-389">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="12960-389">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="12960-390">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-390">Resource</span></span>

* <span data-ttu-id="12960-391">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="12960-391">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="12960-392">Rol</span><span class="sxs-lookup"><span data-stu-id="12960-392">Role</span></span>

* <span data-ttu-id="12960-393">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="12960-393">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="12960-394">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="12960-394">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="12960-395">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="12960-395">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="12960-396">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-396">SQL</span></span>

* <span data-ttu-id="12960-397">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="12960-397">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="12960-398">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="12960-398">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="12960-399">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-399">VM</span></span>

* <span data-ttu-id="12960-400">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="12960-400">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="12960-401">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-401">November 14, 2017</span></span>

<span data-ttu-id="12960-402">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="12960-402">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="12960-403">ACR</span><span class="sxs-lookup"><span data-stu-id="12960-403">ACR</span></span>

* <span data-ttu-id="12960-404">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="12960-404">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="12960-405">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-405">ACS</span></span>

* <span data-ttu-id="12960-406">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="12960-406">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="12960-407">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="12960-407">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="12960-408">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="12960-408">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="12960-409">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="12960-409">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="12960-410">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="12960-410">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-411">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-411">Appservice</span></span>

* <span data-ttu-id="12960-412">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="12960-412">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="12960-413">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="12960-413">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="12960-414">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="12960-414">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="12960-415">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="12960-415">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="12960-416">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="12960-416">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="12960-417">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="12960-417">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="12960-418">Batch</span><span class="sxs-lookup"><span data-stu-id="12960-418">Batch</span></span>

* <span data-ttu-id="12960-419">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="12960-419">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="12960-420">Batchai</span><span class="sxs-lookup"><span data-stu-id="12960-420">Batchai</span></span>

* <span data-ttu-id="12960-421">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="12960-421">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="12960-422">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="12960-422">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="12960-423">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="12960-423">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="12960-424">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="12960-424">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="12960-425">Nube</span><span class="sxs-lookup"><span data-stu-id="12960-425">Cloud</span></span>

* <span data-ttu-id="12960-426">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="12960-426">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="12960-427">Contenedor</span><span class="sxs-lookup"><span data-stu-id="12960-427">Container</span></span>

* <span data-ttu-id="12960-428">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="12960-428">Added support to open multiple ports</span></span>
* <span data-ttu-id="12960-429">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="12960-429">Added container group restart policy</span></span>
* <span data-ttu-id="12960-430">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="12960-430">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="12960-431">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="12960-431">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="12960-432">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="12960-432">Data Lake Analytics</span></span>

* <span data-ttu-id="12960-433">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="12960-433">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="12960-434">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="12960-434">Data Lake Store</span></span>

* <span data-ttu-id="12960-435">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="12960-435">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="12960-436">Extensión</span><span class="sxs-lookup"><span data-stu-id="12960-436">Extension</span></span>

* <span data-ttu-id="12960-437">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="12960-437">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="12960-438">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="12960-438">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="12960-439">IoT</span><span class="sxs-lookup"><span data-stu-id="12960-439">IoT</span></span>

* <span data-ttu-id="12960-440">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="12960-440">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-441">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-441">Monitor</span></span>

* <span data-ttu-id="12960-442">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="12960-442">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="12960-443">Red</span><span class="sxs-lookup"><span data-stu-id="12960-443">Network</span></span>

* <span data-ttu-id="12960-444">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="12960-444">Added support for CAA DNS records</span></span>
* <span data-ttu-id="12960-445">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="12960-445">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="12960-446">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="12960-446">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="12960-447">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="12960-447">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="12960-448">Reservations</span><span class="sxs-lookup"><span data-stu-id="12960-448">Reservations</span></span>

* <span data-ttu-id="12960-449">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="12960-449">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="12960-450">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-450">Resource</span></span>

* <span data-ttu-id="12960-451">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="12960-451">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="12960-452">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-452">SQL</span></span>

* <span data-ttu-id="12960-453">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-453">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="12960-454">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-454">Storage</span></span>

* <span data-ttu-id="12960-455">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="12960-455">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="12960-456">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="12960-456">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="12960-457">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="12960-457">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="12960-458">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="12960-458">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="12960-459">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="12960-459">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="12960-460">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="12960-460">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="12960-461">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="12960-461">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="12960-462">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-462">VM</span></span>

* <span data-ttu-id="12960-463">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="12960-463">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="12960-464">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="12960-464">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="12960-465">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="12960-465">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="12960-466">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="12960-466">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="12960-467">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="12960-467">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="12960-468">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-468">October 24, 2017</span></span>

<span data-ttu-id="12960-469">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="12960-469">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="12960-470">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-470">Core</span></span>

* <span data-ttu-id="12960-471">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="12960-471">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="12960-472">ACR</span><span class="sxs-lookup"><span data-stu-id="12960-472">ACR</span></span>

* <span data-ttu-id="12960-473">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="12960-473">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="12960-474">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="12960-474">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="12960-475">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="12960-475">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="12960-476">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-476">ACS</span></span>

* <span data-ttu-id="12960-477">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="12960-477">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="12960-478">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="12960-478">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-479">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-479">Appservice</span></span>

* <span data-ttu-id="12960-480">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="12960-480">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="12960-481">Componente</span><span class="sxs-lookup"><span data-stu-id="12960-481">Component</span></span>

* <span data-ttu-id="12960-482">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="12960-482">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-483">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-483">Monitor</span></span>

* <span data-ttu-id="12960-484">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="12960-484">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="12960-485">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-485">Resource</span></span>

* <span data-ttu-id="12960-486">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="12960-486">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="12960-487">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="12960-487">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="12960-488">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-488">VM</span></span>

* <span data-ttu-id="12960-489">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="12960-489">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="12960-490">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-490">October 9, 2017</span></span>

<span data-ttu-id="12960-491">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="12960-491">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="12960-492">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-492">Core</span></span>

* <span data-ttu-id="12960-493">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="12960-493">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-494">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-494">Appservice</span></span>

* <span data-ttu-id="12960-495">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="12960-495">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="12960-496">Batch</span><span class="sxs-lookup"><span data-stu-id="12960-496">Batch</span></span>

* <span data-ttu-id="12960-497">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="12960-497">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="12960-498">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="12960-498">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="12960-499">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="12960-499">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="12960-500">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="12960-500">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="12960-501">Batchai</span><span class="sxs-lookup"><span data-stu-id="12960-501">Batchai</span></span>

* <span data-ttu-id="12960-502">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="12960-502">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="12960-503">Keyvault</span><span class="sxs-lookup"><span data-stu-id="12960-503">Keyvault</span></span>

* <span data-ttu-id="12960-504">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="12960-504">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="12960-505">(#4448)</span><span class="sxs-lookup"><span data-stu-id="12960-505">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="12960-506">Red</span><span class="sxs-lookup"><span data-stu-id="12960-506">Network</span></span>

* <span data-ttu-id="12960-507">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="12960-507">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="12960-508">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="12960-508">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="12960-509">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-509">Resource</span></span>

* <span data-ttu-id="12960-510">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="12960-510">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="12960-511">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="12960-511">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="12960-512">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="12960-512">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="12960-513">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="12960-513">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="12960-514">Sql</span><span class="sxs-lookup"><span data-stu-id="12960-514">Sql</span></span>

* <span data-ttu-id="12960-515">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="12960-515">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="12960-516">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="12960-516">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="12960-517">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="12960-517">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="12960-518">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-518">Storage</span></span>

* <span data-ttu-id="12960-519">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="12960-519">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="12960-520">Vm</span><span class="sxs-lookup"><span data-stu-id="12960-520">Vm</span></span>

* <span data-ttu-id="12960-521">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="12960-521">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="12960-522">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="12960-522">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="12960-523">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="12960-523">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="12960-524">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="12960-524">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="12960-525">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="12960-525">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="12960-526">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-526">September 22, 2017</span></span>

<span data-ttu-id="12960-527">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="12960-527">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="12960-528">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-528">Resource</span></span>

* <span data-ttu-id="12960-529">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="12960-529">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="12960-530">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="12960-530">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="12960-531">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="12960-531">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="12960-532">[NUEVO CAMBIO] Se cambió el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="12960-532">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="12960-533">Red</span><span class="sxs-lookup"><span data-stu-id="12960-533">Network</span></span>

* <span data-ttu-id="12960-534">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="12960-534">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="12960-535">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="12960-535">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="12960-536">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="12960-536">Added `asg` application security group commands</span></span>
* <span data-ttu-id="12960-537">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="12960-537">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="12960-538">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-538">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="12960-539">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-539">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="12960-540">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="12960-540">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="12960-541">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-541">Storage</span></span>

* <span data-ttu-id="12960-542">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="12960-542">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="12960-543">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="12960-543">Eventgrid</span></span>

* <span data-ttu-id="12960-544">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="12960-544">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="12960-545">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-545">SQL</span></span>

* <span data-ttu-id="12960-546">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="12960-546">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="12960-547">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="12960-547">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="12960-548">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="12960-548">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="12960-549">Keyvault</span><span class="sxs-lookup"><span data-stu-id="12960-549">Keyvault</span></span>

* <span data-ttu-id="12960-550">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="12960-550">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="12960-551">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-551">VM</span></span>

* <span data-ttu-id="12960-552">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="12960-552">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="12960-553">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="12960-553">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="12960-554">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="12960-554">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="12960-555">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="12960-555">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="12960-556">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="12960-556">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="12960-557">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="12960-557">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="12960-558">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-558">ACS</span></span>

* <span data-ttu-id="12960-559">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="12960-559">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-560">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-560">Appservice</span></span>

* <span data-ttu-id="12960-561">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="12960-561">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="12960-562">Backup</span><span class="sxs-lookup"><span data-stu-id="12960-562">Backup</span></span>

* <span data-ttu-id="12960-563">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="12960-563">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="12960-564">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-564">September 11, 2017</span></span>

<span data-ttu-id="12960-565">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="12960-565">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="12960-566">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-566">Core</span></span>

* <span data-ttu-id="12960-567">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="12960-567">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="12960-568">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="12960-568">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="12960-569">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-569">Acs</span></span>

* <span data-ttu-id="12960-570">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="12960-570">Added `acs list-locations` command</span></span>
* <span data-ttu-id="12960-571">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="12960-571">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-572">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-572">Appservice</span></span>

* <span data-ttu-id="12960-573">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="12960-573">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="12960-574">CDN</span><span class="sxs-lookup"><span data-stu-id="12960-574">CDN</span></span>

* <span data-ttu-id="12960-575">Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="12960-575">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="12960-576">Extensión</span><span class="sxs-lookup"><span data-stu-id="12960-576">Extension</span></span>

* <span data-ttu-id="12960-577">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="12960-577">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="12960-578">Keyvault</span><span class="sxs-lookup"><span data-stu-id="12960-578">Keyvault</span></span>

* <span data-ttu-id="12960-579">Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="12960-579">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="12960-580">Red</span><span class="sxs-lookup"><span data-stu-id="12960-580">Network</span></span>

* <span data-ttu-id="12960-581">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="12960-581">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="12960-582">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="12960-582">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="12960-583">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="12960-583">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="12960-584">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="12960-584">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="12960-585">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="12960-585">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="12960-586">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-586">Resource</span></span>

* <span data-ttu-id="12960-587">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="12960-587">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="12960-588">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="12960-588">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="12960-589">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="12960-589">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="12960-590">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="12960-590">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="12960-591">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-591">SQL</span></span>

* <span data-ttu-id="12960-592">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="12960-592">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="12960-593">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-593">VM</span></span>

* <span data-ttu-id="12960-594">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="12960-594">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="12960-595">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="12960-595">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="12960-596">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="12960-596">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="12960-597">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="12960-597">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="12960-598">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="12960-598">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="12960-599">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-599">August 31, 2017</span></span>

<span data-ttu-id="12960-600">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="12960-600">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="12960-601">Keyvault</span><span class="sxs-lookup"><span data-stu-id="12960-601">Keyvault</span></span>

* <span data-ttu-id="12960-602">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="12960-602">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="12960-603">Sf</span><span class="sxs-lookup"><span data-stu-id="12960-603">Sf</span></span>

* <span data-ttu-id="12960-604">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="12960-604">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="12960-605">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-605">Storage</span></span>

* <span data-ttu-id="12960-606">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="12960-606">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="12960-607">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="12960-607">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="12960-608">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-608">August 28, 2017</span></span>

<span data-ttu-id="12960-609">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="12960-609">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="12960-610">CLI</span><span class="sxs-lookup"><span data-stu-id="12960-610">CLI</span></span>

* <span data-ttu-id="12960-611">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="12960-611">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="12960-612">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-612">ACS</span></span>

* <span data-ttu-id="12960-613">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="12960-613">Corrected preview regions.</span></span>
* <span data-ttu-id="12960-614">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="12960-614">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="12960-615">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="12960-615">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-616">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-616">Appservice</span></span>

* <span data-ttu-id="12960-617">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="12960-617">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="12960-618">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="12960-618">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="12960-619">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="12960-619">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="12960-620">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="12960-620">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="12960-621">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="12960-621">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="12960-622">IoT</span><span class="sxs-lookup"><span data-stu-id="12960-622">IoT</span></span>

* <span data-ttu-id="12960-623">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="12960-623">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="12960-624">Red</span><span class="sxs-lookup"><span data-stu-id="12960-624">Network</span></span>

* <span data-ttu-id="12960-625">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="12960-625">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="12960-626">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="12960-626">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="12960-627">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="12960-627">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="12960-628">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="12960-628">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="12960-629">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="12960-629">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="12960-630">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-630">Profile</span></span>

* <span data-ttu-id="12960-631">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="12960-631">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="12960-632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="12960-632">Service Fabric</span></span>

* <span data-ttu-id="12960-633">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="12960-633">Preview release</span></span>
* <span data-ttu-id="12960-634">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="12960-634">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="12960-635">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="12960-635">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="12960-636">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="12960-636">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="12960-637">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-637">Storage</span></span>

* <span data-ttu-id="12960-638">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="12960-638">Enabled setting blob tier</span></span>
* <span data-ttu-id="12960-639">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="12960-639">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="12960-640">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="12960-640">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="12960-641">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="12960-641">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="12960-642">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="12960-642">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="12960-643">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="12960-643">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="12960-644">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-644">VM</span></span>

* <span data-ttu-id="12960-645">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="12960-645">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="12960-646">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="12960-646">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="12960-647">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="12960-647">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="12960-648">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="12960-648">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="12960-649">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="12960-649">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="12960-650">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="12960-650">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="12960-651">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-651">August 15, 2017</span></span>

<span data-ttu-id="12960-652">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="12960-652">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="12960-653">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-653">ACS</span></span>

* <span data-ttu-id="12960-654">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="12960-654">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-655">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-655">Appservice</span></span>

* <span data-ttu-id="12960-656">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="12960-656">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="12960-657">Event Grid</span><span class="sxs-lookup"><span data-stu-id="12960-657">Event Grid</span></span>

* <span data-ttu-id="12960-658">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="12960-658">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="12960-659">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-659">August 11, 2017</span></span>

<span data-ttu-id="12960-660">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="12960-660">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="12960-661">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-661">ACS</span></span>

* <span data-ttu-id="12960-662">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="12960-662">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="12960-663">Batch</span><span class="sxs-lookup"><span data-stu-id="12960-663">Batch</span></span>

* <span data-ttu-id="12960-664">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="12960-664">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="12960-665">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="12960-665">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="12960-666">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="12960-666">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="12960-667">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="12960-667">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="12960-668">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="12960-668">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="12960-669">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="12960-669">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="12960-670">Componente</span><span class="sxs-lookup"><span data-stu-id="12960-670">Component</span></span>

* <span data-ttu-id="12960-671">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="12960-671">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="12960-672">Contenedor</span><span class="sxs-lookup"><span data-stu-id="12960-672">Container</span></span>

* <span data-ttu-id="12960-673">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="12960-673">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="12960-674">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="12960-674">Data Lake Store</span></span>

* <span data-ttu-id="12960-675">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="12960-675">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="12960-676">Event Grid</span><span class="sxs-lookup"><span data-stu-id="12960-676">Event Grid</span></span>

* <span data-ttu-id="12960-677">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="12960-677">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="12960-678">Red</span><span class="sxs-lookup"><span data-stu-id="12960-678">Network</span></span>

* <span data-ttu-id="12960-679">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="12960-679">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="12960-680">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="12960-680">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="12960-681">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="12960-681">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="12960-682">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="12960-682">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="12960-683">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-683">Profile</span></span>

* <span data-ttu-id="12960-684">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="12960-684">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="12960-685">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-685">Storage</span></span>

* <span data-ttu-id="12960-686">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="12960-686">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="12960-687">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-687">VM</span></span>

* <span data-ttu-id="12960-688">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="12960-688">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="12960-689">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="12960-689">Exposed `list-skus` command</span></span>
* <span data-ttu-id="12960-690">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="12960-690">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="12960-691">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="12960-691">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="12960-692">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="12960-692">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="12960-693">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-693">July 28, 2017</span></span>

<span data-ttu-id="12960-694">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="12960-694">Version 2.0.12</span></span>

* <span data-ttu-id="12960-695">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="12960-695">Added container commands</span></span>
* <span data-ttu-id="12960-696">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="12960-696">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="12960-697">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-697">Core</span></span>

* <span data-ttu-id="12960-698">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="12960-698">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="12960-699">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="12960-699">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="12960-700">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="12960-700">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="12960-701">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="12960-701">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="12960-702">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="12960-702">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="12960-703">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="12960-703">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="12960-704">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="12960-704">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="12960-705">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="12960-705">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="12960-706">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="12960-706">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="12960-707">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="12960-707">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="12960-708">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="12960-708">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="12960-709">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="12960-709">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="12960-710">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="12960-710">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="12960-711">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="12960-711">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="12960-712">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="12960-712">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="12960-713">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="12960-713">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="12960-714">ACR</span><span class="sxs-lookup"><span data-stu-id="12960-714">ACR</span></span>

* <span data-ttu-id="12960-715">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="12960-715">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="12960-716">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="12960-716">Support SKU update for managed registries</span></span>
* <span data-ttu-id="12960-717">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="12960-717">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="12960-718">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="12960-718">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="12960-719">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="12960-719">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="12960-720">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="12960-720">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="12960-721">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-721">ACS</span></span>

* <span data-ttu-id="12960-722">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="12960-722">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-723">Appservice</span><span class="sxs-lookup"><span data-stu-id="12960-723">Appservice</span></span>

* <span data-ttu-id="12960-724">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="12960-724">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="12960-725">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="12960-725">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="12960-726">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="12960-726">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="12960-727">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="12960-727">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="12960-728">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="12960-728">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="12960-729">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="12960-729">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="12960-730">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="12960-730">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="12960-731">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="12960-731">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="12960-732">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="12960-732">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="12960-733">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="12960-733">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="12960-734">Batch</span><span class="sxs-lookup"><span data-stu-id="12960-734">Batch</span></span>

* <span data-ttu-id="12960-735">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="12960-735">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="12960-736">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="12960-736">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="12960-737">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="12960-737">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="12960-738">CDN</span><span class="sxs-lookup"><span data-stu-id="12960-738">CDN</span></span>

* <span data-ttu-id="12960-739">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="12960-739">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="12960-740">Nube</span><span class="sxs-lookup"><span data-stu-id="12960-740">Cloud</span></span>

* <span data-ttu-id="12960-741">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="12960-741">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="12960-742">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="12960-742">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="12960-743">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="12960-743">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="12960-744">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="12960-744">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="12960-745">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="12960-745">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="12960-746">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="12960-746">CosmosDB</span></span>

* <span data-ttu-id="12960-747">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="12960-747">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="12960-748">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="12960-748">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="12960-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="12960-749">Data Lake Analytics</span></span>

* <span data-ttu-id="12960-750">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="12960-750">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="12960-751">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="12960-751">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="12960-752">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="12960-752">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="12960-753">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="12960-753">Data Lake Store</span></span>

* <span data-ttu-id="12960-754">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="12960-754">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="12960-755">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="12960-755">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="12960-756">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="12960-756">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="12960-757">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="12960-757">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="12960-758">Interactive</span><span class="sxs-lookup"><span data-stu-id="12960-758">Interactive</span></span>

* <span data-ttu-id="12960-759">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="12960-759">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="12960-760">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="12960-760">Increased test coverage</span></span>
* <span data-ttu-id="12960-761">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="12960-761">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="12960-762">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="12960-762">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="12960-763">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="12960-763">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="12960-764">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="12960-764">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="12960-765">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="12960-765">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="12960-766">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="12960-766">Added `--progress` flag</span></span>
* <span data-ttu-id="12960-767">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="12960-767">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="12960-768">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="12960-768">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="12960-769">IoT</span><span class="sxs-lookup"><span data-stu-id="12960-769">IoT</span></span>

* <span data-ttu-id="12960-770">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="12960-770">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="12960-771">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="12960-771">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="12960-772">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="12960-772">Key vault</span></span>

* <span data-ttu-id="12960-773">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="12960-773">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="12960-774">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="12960-774">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="12960-775">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="12960-775">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="12960-776">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="12960-776">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="12960-777">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="12960-777">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="12960-778">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="12960-778">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="12960-779">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="12960-779">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="12960-780">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="12960-780">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="12960-781">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="12960-781">Lab</span></span>

* <span data-ttu-id="12960-782">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="12960-782">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="12960-783">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="12960-783">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-784">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-784">Monitor</span></span>

* <span data-ttu-id="12960-785">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="12960-785">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="12960-786">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="12960-786">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="12960-787">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="12960-787">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="12960-788">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="12960-788">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="12960-789">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="12960-789">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="12960-790">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="12960-790">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="12960-791">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="12960-791">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="12960-792">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="12960-792">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="12960-793">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="12960-793">`location` no longer required</span></span>
  * <span data-ttu-id="12960-794">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="12960-794">Add name and ID support for target</span></span>
  * <span data-ttu-id="12960-795">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="12960-795">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="12960-796">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="12960-796">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="12960-797">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="12960-797">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="12960-798">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="12960-798">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="12960-799">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="12960-799">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="12960-800">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="12960-800">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="12960-801">Red</span><span class="sxs-lookup"><span data-stu-id="12960-801">Network</span></span>

* <span data-ttu-id="12960-802">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="12960-802">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="12960-803">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="12960-803">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="12960-804">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="12960-804">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="12960-805">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="12960-805">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="12960-806">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="12960-806">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="12960-807">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="12960-807">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="12960-808">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="12960-808">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="12960-809">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="12960-809">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="12960-810">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="12960-810">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="12960-811">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="12960-811">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="12960-812">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="12960-812">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="12960-813">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="12960-813">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="12960-814">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="12960-814">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="12960-815">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="12960-815">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="12960-816">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="12960-816">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="12960-817">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="12960-817">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="12960-818">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="12960-818">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="12960-819">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="12960-819">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="12960-820">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="12960-820">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="12960-821">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="12960-821">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="12960-822">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="12960-822">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="12960-823">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="12960-823">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="12960-824">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="12960-824">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="12960-825">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="12960-825">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="12960-826">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="12960-826">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="12960-827">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="12960-827">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="12960-828">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="12960-828">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="12960-829">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-829">Profile</span></span>

* <span data-ttu-id="12960-830">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="12960-830">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="12960-831">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="12960-831">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="12960-832">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="12960-832">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="12960-833">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="12960-833">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="12960-834">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="12960-834">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="12960-835">RDBMS</span><span class="sxs-lookup"><span data-stu-id="12960-835">RDBMS</span></span>

* <span data-ttu-id="12960-836">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="12960-836">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="12960-837">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="12960-837">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="12960-838">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="12960-838">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="12960-839">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="12960-839">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="12960-840">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-840">Resource</span></span>

* <span data-ttu-id="12960-841">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="12960-841">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="12960-842">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="12960-842">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="12960-843">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="12960-843">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="12960-844">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="12960-844">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="12960-845">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="12960-845">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="12960-846">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="12960-846">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="12960-847">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="12960-847">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="12960-848">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="12960-848">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="12960-849">Rol</span><span class="sxs-lookup"><span data-stu-id="12960-849">Role</span></span>

* <span data-ttu-id="12960-850">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="12960-850">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="12960-851">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="12960-851">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="12960-852">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="12960-852">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="12960-853">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="12960-853">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="12960-854">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="12960-854">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="12960-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="12960-855">Service Fabric</span></span>
* <span data-ttu-id="12960-856">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="12960-856">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="12960-857">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="12960-857">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="12960-858">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="12960-858">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="12960-859">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-859">SQL</span></span>

* <span data-ttu-id="12960-860">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="12960-860">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="12960-861">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="12960-861">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="12960-862">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="12960-862">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="12960-863">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-863">Storage</span></span>

* <span data-ttu-id="12960-864">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="12960-864">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="12960-865">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="12960-865">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="12960-866">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="12960-866">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="12960-867">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="12960-867">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="12960-868">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="12960-868">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="12960-869">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="12960-869">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="12960-870">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-870">VM</span></span>

* <span data-ttu-id="12960-871">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="12960-871">Support configuring nsg</span></span>
* <span data-ttu-id="12960-872">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="12960-872">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="12960-873">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="12960-873">Support managed service identities</span></span>
* <span data-ttu-id="12960-874">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="12960-874">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="12960-875">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="12960-875">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="12960-876">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-876">May 10, 2017</span></span>

<span data-ttu-id="12960-877">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="12960-877">Version 2.0.6</span></span>

* <span data-ttu-id="12960-878">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="12960-878">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="12960-879">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="12960-879">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="12960-880">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="12960-880">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="12960-881">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="12960-881">Include Cognitive Services module.</span></span>
* <span data-ttu-id="12960-882">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="12960-882">Include Service Fabric module.</span></span>
* <span data-ttu-id="12960-883">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="12960-883">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="12960-884">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="12960-884">Add support for CDN commands.</span></span>
* <span data-ttu-id="12960-885">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="12960-885">Remove Container module.</span></span>
* <span data-ttu-id="12960-886">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="12960-886">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="12960-887">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="12960-887">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="12960-888">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-888">Core</span></span>

* <span data-ttu-id="12960-889">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="12960-889">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="12960-890">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="12960-890">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="12960-891">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="12960-891">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="12960-892">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="12960-892">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="12960-893">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="12960-893">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="12960-894">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="12960-894">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="12960-895">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="12960-895">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="12960-896">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="12960-896">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="12960-897">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="12960-897">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="12960-898">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="12960-898">core: Improved performance</span></span>
* <span data-ttu-id="12960-899">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="12960-899">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="12960-900">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="12960-900">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="12960-901">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-901">ACS</span></span>

* <span data-ttu-id="12960-902">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="12960-902">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="12960-903">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="12960-903">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="12960-904">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="12960-904">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="12960-905">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="12960-905">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-906">AppService</span><span class="sxs-lookup"><span data-stu-id="12960-906">AppService</span></span>

* <span data-ttu-id="12960-907">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="12960-907">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="12960-908">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="12960-908">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="12960-909">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="12960-909">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="12960-910">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="12960-910">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="12960-911">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="12960-911">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="12960-912">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="12960-912">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="12960-913">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="12960-913">support slot swap with preview</span></span>
* <span data-ttu-id="12960-914">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="12960-914">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="12960-915">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="12960-915">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="12960-916">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="12960-916">CosmosDB</span></span>

* <span data-ttu-id="12960-917">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="12960-917">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="12960-918">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="12960-918">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="12960-919">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="12960-919">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="12960-920">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="12960-920">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="12960-921">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="12960-921">Data Lake Analytics</span></span>

* <span data-ttu-id="12960-922">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="12960-922">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="12960-923">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="12960-923">Add support for new catalog item type: package.</span></span> <span data-ttu-id="12960-924">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="12960-924">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="12960-925">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="12960-925">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="12960-926">Tabla</span><span class="sxs-lookup"><span data-stu-id="12960-926">Table</span></span>
  * <span data-ttu-id="12960-927">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="12960-927">Table valued function</span></span>
  * <span data-ttu-id="12960-928">Ver</span><span class="sxs-lookup"><span data-stu-id="12960-928">View</span></span>
  * <span data-ttu-id="12960-929">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="12960-929">Table Statistics.</span></span> <span data-ttu-id="12960-930">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="12960-930">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="12960-931">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="12960-931">Data Lake Store</span></span>

* <span data-ttu-id="12960-932">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="12960-932">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="12960-933">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="12960-933">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="12960-934">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="12960-934">missed help for access show.</span></span> <span data-ttu-id="12960-935">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="12960-935">adding it.</span></span> <span data-ttu-id="12960-936">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="12960-936">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="12960-937">Buscar</span><span class="sxs-lookup"><span data-stu-id="12960-937">Find</span></span>

* <span data-ttu-id="12960-938">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="12960-938">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="12960-939">KeyVault</span><span class="sxs-lookup"><span data-stu-id="12960-939">KeyVault</span></span>

* <span data-ttu-id="12960-940">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="12960-940">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="12960-941">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="12960-941">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="12960-942">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="12960-942">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="12960-943">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="12960-943">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="12960-944">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="12960-944">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="12960-945">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="12960-945">Lab</span></span>

* <span data-ttu-id="12960-946">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="12960-946">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="12960-947">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="12960-947">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="12960-948">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="12960-948">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="12960-949">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="12960-949">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="12960-950">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="12960-950">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="12960-951">Supervisión</span><span class="sxs-lookup"><span data-stu-id="12960-951">Monitor</span></span>

* <span data-ttu-id="12960-952">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="12960-952">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="12960-953">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="12960-953">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="12960-954">Red</span><span class="sxs-lookup"><span data-stu-id="12960-954">Network</span></span>

* <span data-ttu-id="12960-955">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="12960-955">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="12960-956">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="12960-956">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="12960-957">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="12960-957">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="12960-958">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="12960-958">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="12960-959">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="12960-959">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="12960-960">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="12960-960">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="12960-961">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="12960-961">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="12960-962">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="12960-962">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="12960-963">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="12960-963">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="12960-964">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="12960-964">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="12960-965">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="12960-965">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="12960-966">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="12960-966">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="12960-967">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="12960-967">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="12960-968">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="12960-968">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="12960-969">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="12960-969">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="12960-970">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="12960-970">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="12960-971">Perfil</span><span class="sxs-lookup"><span data-stu-id="12960-971">Profile</span></span>

* <span data-ttu-id="12960-972">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="12960-972">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="12960-973">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="12960-973">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="12960-974">Redis</span><span class="sxs-lookup"><span data-stu-id="12960-974">Redis</span></span>

* <span data-ttu-id="12960-975">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="12960-975">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="12960-976">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="12960-976">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="12960-977">Recurso</span><span class="sxs-lookup"><span data-stu-id="12960-977">Resource</span></span>

* <span data-ttu-id="12960-978">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="12960-978">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="12960-979">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="12960-979">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="12960-980">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="12960-980">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="12960-981">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="12960-981">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="12960-982">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="12960-982">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="12960-983">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="12960-983">Add docs for az lock update.</span></span> <span data-ttu-id="12960-984">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="12960-984">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="12960-985">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="12960-985">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="12960-986">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="12960-986">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="12960-987">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="12960-987">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="12960-988">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="12960-988">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="12960-989">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="12960-989">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="12960-990">Rol</span><span class="sxs-lookup"><span data-stu-id="12960-990">Role</span></span>

* <span data-ttu-id="12960-991">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="12960-991">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="12960-992">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="12960-992">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="12960-993">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="12960-993">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="12960-994">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="12960-994">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="12960-995">SQL</span><span class="sxs-lookup"><span data-stu-id="12960-995">SQL</span></span>

* <span data-ttu-id="12960-996">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="12960-996">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="12960-997">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="12960-997">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="12960-998">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-998">Storage</span></span>

* <span data-ttu-id="12960-999">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="12960-999">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="12960-1000">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="12960-1000">Add support for incremental blob copy</span></span>
* <span data-ttu-id="12960-1001">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="12960-1001">Add support for large block blob upload</span></span>
* <span data-ttu-id="12960-1002">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="12960-1002">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="12960-1003">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-1003">VM</span></span>

* <span data-ttu-id="12960-1004">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="12960-1004">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="12960-1005">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="12960-1005">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="12960-1006">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="12960-1006">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="12960-1007">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="12960-1007">az vm/vmss disk</span></span>
  3. <span data-ttu-id="12960-1008">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="12960-1008">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="12960-1009">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="12960-1009">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="12960-1010">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="12960-1010">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="12960-1011">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-1011">April 3, 2017</span></span>

<span data-ttu-id="12960-1012">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="12960-1012">Version 2.0.2</span></span>

<span data-ttu-id="12960-1013">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="12960-1013">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="12960-1014">Núcleo</span><span class="sxs-lookup"><span data-stu-id="12960-1014">Core</span></span>

* <span data-ttu-id="12960-1015">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="12960-1015">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="12960-1016">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="12960-1016">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="12960-1017">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="12960-1017">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="12960-1018">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="12960-1018">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="12960-1019">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="12960-1019">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="12960-1020">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="12960-1020">Add prompting for missing template parameters.</span></span> <span data-ttu-id="12960-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="12960-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="12960-1022">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="12960-1022">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="12960-1023">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="12960-1023">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="12960-1024">ACS</span><span class="sxs-lookup"><span data-stu-id="12960-1024">ACS</span></span>

* <span data-ttu-id="12960-1025">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="12960-1025">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="12960-1026">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="12960-1026">Add support for ssh key password prompting.</span></span> <span data-ttu-id="12960-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="12960-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="12960-1028">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="12960-1028">Add support for windows clusters.</span></span> <span data-ttu-id="12960-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="12960-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="12960-1030">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="12960-1030">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="12960-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="12960-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="12960-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="12960-1032">AppService</span></span>

* <span data-ttu-id="12960-1033">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="12960-1033">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="12960-1034">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="12960-1034">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="12960-1035">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="12960-1035">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="12960-1036">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="12960-1036">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="12960-1037">DataLake</span><span class="sxs-lookup"><span data-stu-id="12960-1037">DataLake</span></span>

* <span data-ttu-id="12960-1038">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="12960-1038">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="12960-1039">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="12960-1039">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="12960-1040">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="12960-1040">DocuemntDB</span></span>

* <span data-ttu-id="12960-1041">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="12960-1041">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="12960-1042">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="12960-1042">VM</span></span>

* <span data-ttu-id="12960-1043">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="12960-1043">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="12960-1044">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="12960-1044">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="12960-1045">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="12960-1045">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="12960-1046">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="12960-1046">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="12960-1047">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="12960-1047">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="12960-1048">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="12960-1048">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="12960-1049">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="12960-1049">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="12960-1050">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="12960-1050">February 27, 2017</span></span>

<span data-ttu-id="12960-1051">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="12960-1051">Version 2.0.0</span></span>

<span data-ttu-id="12960-1052">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="12960-1052">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="12960-1053">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="12960-1053">General availability applies to these command modules:</span></span>
- <span data-ttu-id="12960-1054">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="12960-1054">Container Service (acs)</span></span>
- <span data-ttu-id="12960-1055">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="12960-1055">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="12960-1056">Redes</span><span class="sxs-lookup"><span data-stu-id="12960-1056">Networking</span></span>
- <span data-ttu-id="12960-1057">Storage</span><span class="sxs-lookup"><span data-stu-id="12960-1057">Storage</span></span>

<span data-ttu-id="12960-1058">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12960-1058">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="12960-1059">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="12960-1059">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="12960-1060">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="12960-1060">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="12960-1061">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="12960-1061">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="12960-1062">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="12960-1062">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="12960-1063">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="12960-1063">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="12960-1064">Algunos de los módulos de comando tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="12960-1064">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="12960-1065">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="12960-1065">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="12960-1066">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="12960-1066">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="12960-1067">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="12960-1067">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="12960-1068">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="12960-1068">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="12960-1069">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="12960-1069">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="12960-1070">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="12960-1070">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="12960-1071">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="12960-1071">Provide feedback from the command line with the `az feedback` command.</span></span>

