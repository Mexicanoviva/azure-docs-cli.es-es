---
title: "Notas de la versión de la CLI de Azure 2.0"
description: "Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0"
keywords: "CLI de Azure 2.0, notas de la versión"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/17/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 86babea3030ea932de1858a391014e5d0bba7f73
ms.sourcegitcommit: cae66f994cb7b7f829f75ac528093fdb6851f64e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="cda21-104">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="cda21-104">Azure CLI 2.0 release notes</span></span>

## <a name="january-17-2018"></a><span data-ttu-id="cda21-105">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="cda21-105">January 17, 2018</span></span>

<span data-ttu-id="cda21-106">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="cda21-106">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="cda21-107">ACR</span><span class="sxs-lookup"><span data-stu-id="cda21-107">ACR</span></span>

* <span data-ttu-id="cda21-108">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="cda21-108">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="cda21-109">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="cda21-109">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-110">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-110">ACS</span></span>

* <span data-ttu-id="cda21-111">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="cda21-111">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="cda21-112">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="cda21-112">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-113">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-113">Appservice</span></span>

* <span data-ttu-id="cda21-114">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="cda21-114">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="cda21-115">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="cda21-115">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="cda21-116">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="cda21-116">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="cda21-117">Backup</span><span class="sxs-lookup"><span data-stu-id="cda21-117">Backup</span></span>

* <span data-ttu-id="cda21-118">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="cda21-118">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="cda21-119">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="cda21-119">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="cda21-120">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="cda21-120">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="cda21-121">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="cda21-121">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="cda21-122">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="cda21-122">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="cda21-123">Batch</span><span class="sxs-lookup"><span data-stu-id="cda21-123">Batch</span></span>

* <span data-ttu-id="cda21-124">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="cda21-124">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="cda21-125">Nube</span><span class="sxs-lookup"><span data-stu-id="cda21-125">Cloud</span></span>

* <span data-ttu-id="cda21-126">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="cda21-126">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="cda21-127">Consumo</span><span class="sxs-lookup"><span data-stu-id="cda21-127">Consumption</span></span>

* <span data-ttu-id="cda21-128">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="cda21-128">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="cda21-129">Event Grid</span><span class="sxs-lookup"><span data-stu-id="cda21-129">Event Grid</span></span>

* <span data-ttu-id="cda21-130">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="cda21-130">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="cda21-131">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="cda21-131">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="cda21-132">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="cda21-132">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="cda21-133">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="cda21-133">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="cda21-134">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="cda21-134">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="cda21-135">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="cda21-135">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="cda21-136">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="cda21-136">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="cda21-137">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="cda21-137">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="cda21-138">Interactive</span><span class="sxs-lookup"><span data-stu-id="cda21-138">Interactive</span></span>

* <span data-ttu-id="cda21-139">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="cda21-139">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="cda21-140">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="cda21-140">Fixed errors on startup</span></span>
* <span data-ttu-id="cda21-141">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="cda21-141">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="cda21-142">IoT</span><span class="sxs-lookup"><span data-stu-id="cda21-142">IoT</span></span>

* <span data-ttu-id="cda21-143">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="cda21-143">Added support for device provisioning service</span></span>
* <span data-ttu-id="cda21-144">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="cda21-144">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="cda21-145">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="cda21-145">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="cda21-146">Supervisión</span><span class="sxs-lookup"><span data-stu-id="cda21-146">Monitor</span></span>

* <span data-ttu-id="cda21-147">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="cda21-147">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="cda21-148">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="cda21-148">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="cda21-149">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="cda21-149">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span> 

### <a name="network"></a><span data-ttu-id="cda21-150">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-150">Network</span></span>

* <span data-ttu-id="cda21-151">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="cda21-151">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="cda21-152">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-152">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="cda21-153">Perfil</span><span class="sxs-lookup"><span data-stu-id="cda21-153">Profile</span></span>

* <span data-ttu-id="cda21-154">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="cda21-154">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="cda21-155">Rol</span><span class="sxs-lookup"><span data-stu-id="cda21-155">Role</span></span>

* <span data-ttu-id="cda21-156">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="cda21-156">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cda21-157">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cda21-157">Service Fabric</span></span>

* <span data-ttu-id="cda21-158">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="cda21-158">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="cda21-159">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="cda21-159">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-160">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-160">VM</span></span>

* <span data-ttu-id="cda21-161">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="cda21-161">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="cda21-162">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado del `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="cda21-162">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="cda21-163">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="cda21-163">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="cda21-164">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="cda21-164">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="cda21-165">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="cda21-165">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="cda21-166">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="cda21-166">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="cda21-167">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="cda21-167">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="cda21-168">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="cda21-168">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="cda21-169">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-169">December 19, 2017</span></span>

<span data-ttu-id="cda21-170">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="cda21-170">Version 2.0.23</span></span>

* <span data-ttu-id="cda21-171">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="cda21-171">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="cda21-172">Contenedor</span><span class="sxs-lookup"><span data-stu-id="cda21-172">Container</span></span>

* <span data-ttu-id="cda21-173">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="cda21-173">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="cda21-174">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-174">Network</span></span>

* <span data-ttu-id="cda21-175">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-175">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="cda21-176">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-176">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-177">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-177">Storage</span></span>

* <span data-ttu-id="cda21-178">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="cda21-178">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-179">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-179">VM</span></span>

* <span data-ttu-id="cda21-180">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="cda21-180">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="cda21-181">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-181">December 5, 2017</span></span>

<span data-ttu-id="cda21-182">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="cda21-182">Version 2.0.22</span></span>

* <span data-ttu-id="cda21-183">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="cda21-183">Removed `az component` commands.</span></span> <span data-ttu-id="cda21-184">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="cda21-184">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="cda21-185">Núcleo</span><span class="sxs-lookup"><span data-stu-id="cda21-185">Core</span></span>
* <span data-ttu-id="cda21-186">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="cda21-186">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="cda21-187">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="cda21-187">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-188">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-188">ACS</span></span>

* <span data-ttu-id="cda21-189">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="cda21-189">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="cda21-190">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="cda21-190">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="cda21-191">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="cda21-191">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="cda21-192">Advisor</span><span class="sxs-lookup"><span data-stu-id="cda21-192">Advisor</span></span>

* <span data-ttu-id="cda21-193">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="cda21-193">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-194">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-194">Appservice</span></span>

* <span data-ttu-id="cda21-195">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="cda21-195">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="cda21-196">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="cda21-196">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="cda21-197">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="cda21-197">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="cda21-198">Consumo</span><span class="sxs-lookup"><span data-stu-id="cda21-198">Consumption</span></span>

* <span data-ttu-id="cda21-199">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="cda21-199">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="cda21-200">Contenedor</span><span class="sxs-lookup"><span data-stu-id="cda21-200">Container</span></span>

* <span data-ttu-id="cda21-201">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="cda21-201">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="cda21-202">Supervisión</span><span class="sxs-lookup"><span data-stu-id="cda21-202">Monitor</span></span>

* <span data-ttu-id="cda21-203">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="cda21-203">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-204">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-204">Resource</span></span>

* <span data-ttu-id="cda21-205">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="cda21-205">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="cda21-206">Rol</span><span class="sxs-lookup"><span data-stu-id="cda21-206">Role</span></span>

* <span data-ttu-id="cda21-207">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="cda21-207">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="cda21-208">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="cda21-208">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="cda21-209">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="cda21-209">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="cda21-210">SQL</span><span class="sxs-lookup"><span data-stu-id="cda21-210">SQL</span></span>

* <span data-ttu-id="cda21-211">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="cda21-211">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="cda21-212">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="cda21-212">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-213">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-213">VM</span></span>

* <span data-ttu-id="cda21-214">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="cda21-214">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="cda21-215">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-215">November 14, 2017</span></span>

<span data-ttu-id="cda21-216">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="cda21-216">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="cda21-217">ACR</span><span class="sxs-lookup"><span data-stu-id="cda21-217">ACR</span></span>

* <span data-ttu-id="cda21-218">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="cda21-218">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="cda21-219">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-219">ACS</span></span>

* <span data-ttu-id="cda21-220">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="cda21-220">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="cda21-221">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="cda21-221">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="cda21-222">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="cda21-222">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="cda21-223">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="cda21-223">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="cda21-224">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="cda21-224">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-225">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-225">Appservice</span></span>

* <span data-ttu-id="cda21-226">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="cda21-226">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="cda21-227">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="cda21-227">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="cda21-228">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="cda21-228">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="cda21-229">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="cda21-229">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="cda21-230">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="cda21-230">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="cda21-231">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="cda21-231">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="cda21-232">Batch</span><span class="sxs-lookup"><span data-stu-id="cda21-232">Batch</span></span>

* <span data-ttu-id="cda21-233">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="cda21-233">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="cda21-234">Batchai</span><span class="sxs-lookup"><span data-stu-id="cda21-234">Batchai</span></span>

* <span data-ttu-id="cda21-235">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="cda21-235">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="cda21-236">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="cda21-236">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="cda21-237">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="cda21-237">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="cda21-238">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="cda21-238">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="cda21-239">Nube</span><span class="sxs-lookup"><span data-stu-id="cda21-239">Cloud</span></span>

* <span data-ttu-id="cda21-240">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="cda21-240">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="cda21-241">Contenedor</span><span class="sxs-lookup"><span data-stu-id="cda21-241">Container</span></span>

* <span data-ttu-id="cda21-242">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="cda21-242">Added support to open multiple ports</span></span>
* <span data-ttu-id="cda21-243">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="cda21-243">Added container group restart policy</span></span>
* <span data-ttu-id="cda21-244">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="cda21-244">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="cda21-245">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="cda21-245">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="cda21-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="cda21-246">Data Lake Analytics</span></span>

* <span data-ttu-id="cda21-247">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="cda21-247">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="cda21-248">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="cda21-248">Data Lake Store</span></span>

* <span data-ttu-id="cda21-249">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="cda21-249">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="cda21-250">Extensión</span><span class="sxs-lookup"><span data-stu-id="cda21-250">Extension</span></span>

* <span data-ttu-id="cda21-251">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="cda21-251">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="cda21-252">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="cda21-252">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="cda21-253">IoT</span><span class="sxs-lookup"><span data-stu-id="cda21-253">IoT</span></span>

* <span data-ttu-id="cda21-254">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="cda21-254">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="cda21-255">Supervisión</span><span class="sxs-lookup"><span data-stu-id="cda21-255">Monitor</span></span>

* <span data-ttu-id="cda21-256">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="cda21-256">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="cda21-257">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-257">Network</span></span>

* <span data-ttu-id="cda21-258">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="cda21-258">Added support for CAA DNS records</span></span>
* <span data-ttu-id="cda21-259">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="cda21-259">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="cda21-260">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-260">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="cda21-261">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="cda21-261">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="cda21-262">Reservations</span><span class="sxs-lookup"><span data-stu-id="cda21-262">Reservations</span></span>

* <span data-ttu-id="cda21-263">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="cda21-263">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-264">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-264">Resource</span></span>

* <span data-ttu-id="cda21-265">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-265">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="cda21-266">SQL</span><span class="sxs-lookup"><span data-stu-id="cda21-266">SQL</span></span>

* <span data-ttu-id="cda21-267">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-267">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-268">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-268">Storage</span></span>

* <span data-ttu-id="cda21-269">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="cda21-269">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="cda21-270">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="cda21-270">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="cda21-271">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="cda21-271">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="cda21-272">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="cda21-272">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="cda21-273">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="cda21-273">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="cda21-274">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="cda21-274">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="cda21-275">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="cda21-275">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-276">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-276">VM</span></span>

* <span data-ttu-id="cda21-277">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="cda21-277">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="cda21-278">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="cda21-278">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="cda21-279">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="cda21-279">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="cda21-280">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="cda21-280">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="cda21-281">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="cda21-281">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="cda21-282">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-282">October 24, 2017</span></span>

<span data-ttu-id="cda21-283">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="cda21-283">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="cda21-284">Núcleo</span><span class="sxs-lookup"><span data-stu-id="cda21-284">Core</span></span>

* <span data-ttu-id="cda21-285">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="cda21-285">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="cda21-286">ACR</span><span class="sxs-lookup"><span data-stu-id="cda21-286">ACR</span></span>

* <span data-ttu-id="cda21-287">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="cda21-287">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="cda21-288">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="cda21-288">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="cda21-289">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="cda21-289">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-290">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-290">ACS</span></span>

* <span data-ttu-id="cda21-291">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="cda21-291">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="cda21-292">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="cda21-292">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-293">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-293">Appservice</span></span>

* <span data-ttu-id="cda21-294">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="cda21-294">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="cda21-295">Componente</span><span class="sxs-lookup"><span data-stu-id="cda21-295">Component</span></span>

* <span data-ttu-id="cda21-296">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="cda21-296">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="cda21-297">Supervisión</span><span class="sxs-lookup"><span data-stu-id="cda21-297">Monitor</span></span>

* <span data-ttu-id="cda21-298">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="cda21-298">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-299">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-299">Resource</span></span>

* <span data-ttu-id="cda21-300">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="cda21-300">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="cda21-301">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="cda21-301">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-302">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-302">VM</span></span>

* <span data-ttu-id="cda21-303">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="cda21-303">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="cda21-304">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-304">October 9, 2017</span></span>

<span data-ttu-id="cda21-305">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="cda21-305">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="cda21-306">Núcleo</span><span class="sxs-lookup"><span data-stu-id="cda21-306">Core</span></span>

* <span data-ttu-id="cda21-307">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="cda21-307">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-308">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-308">Appservice</span></span>

* <span data-ttu-id="cda21-309">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="cda21-309">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="cda21-310">Batch</span><span class="sxs-lookup"><span data-stu-id="cda21-310">Batch</span></span>

* <span data-ttu-id="cda21-311">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="cda21-311">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="cda21-312">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="cda21-312">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="cda21-313">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="cda21-313">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="cda21-314">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="cda21-314">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="cda21-315">Batchai</span><span class="sxs-lookup"><span data-stu-id="cda21-315">Batchai</span></span>

* <span data-ttu-id="cda21-316">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="cda21-316">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="cda21-317">Keyvault</span><span class="sxs-lookup"><span data-stu-id="cda21-317">Keyvault</span></span>

* <span data-ttu-id="cda21-318">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="cda21-318">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="cda21-319">(#4448)</span><span class="sxs-lookup"><span data-stu-id="cda21-319">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="cda21-320">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-320">Network</span></span>

* <span data-ttu-id="cda21-321">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="cda21-321">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="cda21-322">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="cda21-322">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-323">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-323">Resource</span></span>

* <span data-ttu-id="cda21-324">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-324">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="cda21-325">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="cda21-325">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="cda21-326">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="cda21-326">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="cda21-327">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-327">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="cda21-328">Sql</span><span class="sxs-lookup"><span data-stu-id="cda21-328">Sql</span></span>

* <span data-ttu-id="cda21-329">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="cda21-329">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="cda21-330">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="cda21-330">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="cda21-331">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="cda21-331">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-332">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-332">Storage</span></span>

* <span data-ttu-id="cda21-333">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="cda21-333">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-334">Vm</span><span class="sxs-lookup"><span data-stu-id="cda21-334">Vm</span></span>

* <span data-ttu-id="cda21-335">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="cda21-335">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="cda21-336">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="cda21-336">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="cda21-337">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="cda21-337">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="cda21-338">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="cda21-338">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="cda21-339">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="cda21-339">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="cda21-340">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-340">September 22, 2017</span></span>

<span data-ttu-id="cda21-341">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="cda21-341">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-342">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-342">Resource</span></span>

* <span data-ttu-id="cda21-343">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="cda21-343">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="cda21-344">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="cda21-344">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="cda21-345">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="cda21-345">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="cda21-346">[NUEVO CAMBIO] Se cambió el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="cda21-346">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="cda21-347">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-347">Network</span></span>

* <span data-ttu-id="cda21-348">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="cda21-348">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="cda21-349">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="cda21-349">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="cda21-350">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="cda21-350">Added `asg` application security group commands</span></span>
* <span data-ttu-id="cda21-351">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-351">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="cda21-352">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-352">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="cda21-353">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-353">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="cda21-354">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="cda21-354">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-355">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-355">Storage</span></span>

* <span data-ttu-id="cda21-356">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="cda21-356">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="cda21-357">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="cda21-357">Eventgrid</span></span>

* <span data-ttu-id="cda21-358">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="cda21-358">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="cda21-359">SQL</span><span class="sxs-lookup"><span data-stu-id="cda21-359">SQL</span></span>

* <span data-ttu-id="cda21-360">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="cda21-360">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="cda21-361">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="cda21-361">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="cda21-362">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cda21-362">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="cda21-363">Keyvault</span><span class="sxs-lookup"><span data-stu-id="cda21-363">Keyvault</span></span>

* <span data-ttu-id="cda21-364">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="cda21-364">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-365">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-365">VM</span></span>

* <span data-ttu-id="cda21-366">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="cda21-366">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="cda21-367">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="cda21-367">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="cda21-368">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="cda21-368">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="cda21-369">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="cda21-369">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="cda21-370">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="cda21-370">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="cda21-371">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="cda21-371">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-372">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-372">ACS</span></span>

* <span data-ttu-id="cda21-373">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-373">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-374">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-374">Appservice</span></span>

* <span data-ttu-id="cda21-375">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="cda21-375">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="cda21-376">Backup</span><span class="sxs-lookup"><span data-stu-id="cda21-376">Backup</span></span>

* <span data-ttu-id="cda21-377">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="cda21-377">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="cda21-378">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-378">September 11, 2017</span></span>

<span data-ttu-id="cda21-379">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="cda21-379">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="cda21-380">Núcleo</span><span class="sxs-lookup"><span data-stu-id="cda21-380">Core</span></span>

* <span data-ttu-id="cda21-381">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="cda21-381">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="cda21-382">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="cda21-382">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-383">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-383">Acs</span></span>

* <span data-ttu-id="cda21-384">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="cda21-384">Added `acs list-locations` command</span></span>
* <span data-ttu-id="cda21-385">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="cda21-385">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-386">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-386">Appservice</span></span>

* <span data-ttu-id="cda21-387">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="cda21-387">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="cda21-388">CDN</span><span class="sxs-lookup"><span data-stu-id="cda21-388">CDN</span></span>

* <span data-ttu-id="cda21-389">Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-389">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="cda21-390">Extensión</span><span class="sxs-lookup"><span data-stu-id="cda21-390">Extension</span></span>

* <span data-ttu-id="cda21-391">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="cda21-391">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="cda21-392">Keyvault</span><span class="sxs-lookup"><span data-stu-id="cda21-392">Keyvault</span></span>

* <span data-ttu-id="cda21-393">Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="cda21-393">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="cda21-394">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-394">Network</span></span>

* <span data-ttu-id="cda21-395">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="cda21-395">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="cda21-396">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-396">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="cda21-397">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-397">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="cda21-398">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-398">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="cda21-399">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-399">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-400">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-400">Resource</span></span>

* <span data-ttu-id="cda21-401">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-401">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="cda21-402">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-402">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="cda21-403">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="cda21-403">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="cda21-404">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="cda21-404">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="cda21-405">SQL</span><span class="sxs-lookup"><span data-stu-id="cda21-405">SQL</span></span>

* <span data-ttu-id="cda21-406">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="cda21-406">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-407">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-407">VM</span></span>

* <span data-ttu-id="cda21-408">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="cda21-408">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="cda21-409">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="cda21-409">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="cda21-410">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-410">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="cda21-411">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="cda21-411">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="cda21-412">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="cda21-412">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="cda21-413">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-413">August 31, 2017</span></span>

<span data-ttu-id="cda21-414">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="cda21-414">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="cda21-415">Keyvault</span><span class="sxs-lookup"><span data-stu-id="cda21-415">Keyvault</span></span>

* <span data-ttu-id="cda21-416">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="cda21-416">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="cda21-417">Sf</span><span class="sxs-lookup"><span data-stu-id="cda21-417">Sf</span></span>

* <span data-ttu-id="cda21-418">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="cda21-418">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-419">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-419">Storage</span></span>

* <span data-ttu-id="cda21-420">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="cda21-420">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="cda21-421">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="cda21-421">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="cda21-422">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-422">August 28, 2017</span></span>

<span data-ttu-id="cda21-423">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="cda21-423">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="cda21-424">CLI</span><span class="sxs-lookup"><span data-stu-id="cda21-424">CLI</span></span>

* <span data-ttu-id="cda21-425">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="cda21-425">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-426">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-426">ACS</span></span>

* <span data-ttu-id="cda21-427">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="cda21-427">Corrected preview regions.</span></span>
* <span data-ttu-id="cda21-428">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="cda21-428">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="cda21-429">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="cda21-429">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-430">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-430">Appservice</span></span>

* <span data-ttu-id="cda21-431">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="cda21-431">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="cda21-432">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="cda21-432">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="cda21-433">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="cda21-433">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="cda21-434">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="cda21-434">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="cda21-435">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="cda21-435">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="cda21-436">IoT</span><span class="sxs-lookup"><span data-stu-id="cda21-436">IoT</span></span>

* <span data-ttu-id="cda21-437">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="cda21-437">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="cda21-438">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-438">Network</span></span>

* <span data-ttu-id="cda21-439">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="cda21-439">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="cda21-440">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cda21-440">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="cda21-441">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cda21-441">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="cda21-442">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-442">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="cda21-443">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-443">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="cda21-444">Perfil</span><span class="sxs-lookup"><span data-stu-id="cda21-444">Profile</span></span>

* <span data-ttu-id="cda21-445">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="cda21-445">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cda21-446">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cda21-446">Service Fabric</span></span>

* <span data-ttu-id="cda21-447">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="cda21-447">Preview release</span></span>
* <span data-ttu-id="cda21-448">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="cda21-448">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="cda21-449">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="cda21-449">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="cda21-450">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="cda21-450">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-451">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-451">Storage</span></span>

* <span data-ttu-id="cda21-452">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="cda21-452">Enabled setting blob tier</span></span>
* <span data-ttu-id="cda21-453">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="cda21-453">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="cda21-454">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="cda21-454">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="cda21-455">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="cda21-455">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="cda21-456">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-456">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="cda21-457">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="cda21-457">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-458">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-458">VM</span></span>

* <span data-ttu-id="cda21-459">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="cda21-459">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="cda21-460">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-460">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="cda21-461">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-461">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="cda21-462">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="cda21-462">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="cda21-463">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="cda21-463">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="cda21-464">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-464">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="cda21-465">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-465">August 15, 2017</span></span>

<span data-ttu-id="cda21-466">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="cda21-466">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-467">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-467">ACS</span></span>

* <span data-ttu-id="cda21-468">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="cda21-468">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-469">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-469">Appservice</span></span>

* <span data-ttu-id="cda21-470">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="cda21-470">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="cda21-471">Event Grid</span><span class="sxs-lookup"><span data-stu-id="cda21-471">Event Grid</span></span>

* <span data-ttu-id="cda21-472">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="cda21-472">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="cda21-473">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-473">August 11, 2017</span></span>

<span data-ttu-id="cda21-474">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="cda21-474">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-475">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-475">ACS</span></span>

* <span data-ttu-id="cda21-476">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="cda21-476">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="cda21-477">Batch</span><span class="sxs-lookup"><span data-stu-id="cda21-477">Batch</span></span>

* <span data-ttu-id="cda21-478">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="cda21-478">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="cda21-479">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="cda21-479">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="cda21-480">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="cda21-480">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="cda21-481">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="cda21-481">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="cda21-482">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="cda21-482">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="cda21-483">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="cda21-483">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="cda21-484">Componente</span><span class="sxs-lookup"><span data-stu-id="cda21-484">Component</span></span>

* <span data-ttu-id="cda21-485">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="cda21-485">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="cda21-486">Contenedor</span><span class="sxs-lookup"><span data-stu-id="cda21-486">Container</span></span>

* <span data-ttu-id="cda21-487">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="cda21-487">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="cda21-488">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="cda21-488">Data Lake Store</span></span>

* <span data-ttu-id="cda21-489">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="cda21-489">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="cda21-490">Event Grid</span><span class="sxs-lookup"><span data-stu-id="cda21-490">Event Grid</span></span>

* <span data-ttu-id="cda21-491">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="cda21-491">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="cda21-492">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-492">Network</span></span>

* <span data-ttu-id="cda21-493">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="cda21-493">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="cda21-494">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cda21-494">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="cda21-495">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="cda21-495">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="cda21-496">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="cda21-496">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="cda21-497">Perfil</span><span class="sxs-lookup"><span data-stu-id="cda21-497">Profile</span></span>

* <span data-ttu-id="cda21-498">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="cda21-498">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-499">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-499">Storage</span></span>

* <span data-ttu-id="cda21-500">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="cda21-500">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-501">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-501">VM</span></span>

* <span data-ttu-id="cda21-502">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="cda21-502">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="cda21-503">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="cda21-503">Exposed `list-skus` command</span></span>
* <span data-ttu-id="cda21-504">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="cda21-504">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="cda21-505">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="cda21-505">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="cda21-506">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="cda21-506">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="cda21-507">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-507">July 28, 2017</span></span>

<span data-ttu-id="cda21-508">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="cda21-508">Version 2.0.12</span></span>

* <span data-ttu-id="cda21-509">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="cda21-509">Added container commands</span></span>
* <span data-ttu-id="cda21-510">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="cda21-510">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="cda21-511">Núcleo</span><span class="sxs-lookup"><span data-stu-id="cda21-511">Core</span></span>

* <span data-ttu-id="cda21-512">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="cda21-512">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="cda21-513">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="cda21-513">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="cda21-514">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="cda21-514">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="cda21-515">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="cda21-515">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="cda21-516">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="cda21-516">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="cda21-517">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="cda21-517">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="cda21-518">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="cda21-518">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="cda21-519">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="cda21-519">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="cda21-520">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="cda21-520">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="cda21-521">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="cda21-521">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="cda21-522">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="cda21-522">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="cda21-523">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="cda21-523">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="cda21-524">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="cda21-524">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="cda21-525">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="cda21-525">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="cda21-526">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="cda21-526">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="cda21-527">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="cda21-527">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="cda21-528">ACR</span><span class="sxs-lookup"><span data-stu-id="cda21-528">ACR</span></span>

* <span data-ttu-id="cda21-529">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="cda21-529">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="cda21-530">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="cda21-530">Support SKU update for managed registries</span></span>
* <span data-ttu-id="cda21-531">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="cda21-531">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="cda21-532">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="cda21-532">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="cda21-533">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="cda21-533">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="cda21-534">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="cda21-534">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-535">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-535">ACS</span></span>

* <span data-ttu-id="cda21-536">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="cda21-536">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-537">Appservice</span><span class="sxs-lookup"><span data-stu-id="cda21-537">Appservice</span></span>

* <span data-ttu-id="cda21-538">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="cda21-538">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="cda21-539">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="cda21-539">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="cda21-540">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="cda21-540">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="cda21-541">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="cda21-541">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="cda21-542">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="cda21-542">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="cda21-543">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="cda21-543">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="cda21-544">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="cda21-544">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="cda21-545">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="cda21-545">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="cda21-546">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="cda21-546">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="cda21-547">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="cda21-547">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="cda21-548">Batch</span><span class="sxs-lookup"><span data-stu-id="cda21-548">Batch</span></span>

* <span data-ttu-id="cda21-549">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="cda21-549">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="cda21-550">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="cda21-550">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="cda21-551">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-551">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="cda21-552">CDN</span><span class="sxs-lookup"><span data-stu-id="cda21-552">CDN</span></span>

* <span data-ttu-id="cda21-553">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="cda21-553">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="cda21-554">Nube</span><span class="sxs-lookup"><span data-stu-id="cda21-554">Cloud</span></span>

* <span data-ttu-id="cda21-555">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="cda21-555">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="cda21-556">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="cda21-556">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="cda21-557">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="cda21-557">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="cda21-558">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="cda21-558">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="cda21-559">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="cda21-559">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cda21-560">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="cda21-560">CosmosDB</span></span>

* <span data-ttu-id="cda21-561">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="cda21-561">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="cda21-562">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="cda21-562">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="cda21-563">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="cda21-563">Data Lake Analytics</span></span>

* <span data-ttu-id="cda21-564">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="cda21-564">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="cda21-565">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="cda21-565">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="cda21-566">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="cda21-566">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="cda21-567">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="cda21-567">Data Lake Store</span></span>

* <span data-ttu-id="cda21-568">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-568">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="cda21-569">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="cda21-569">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="cda21-570">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="cda21-570">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="cda21-571">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="cda21-571">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="cda21-572">Interactive</span><span class="sxs-lookup"><span data-stu-id="cda21-572">Interactive</span></span>

* <span data-ttu-id="cda21-573">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="cda21-573">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="cda21-574">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="cda21-574">Increased test coverage</span></span>
* <span data-ttu-id="cda21-575">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="cda21-575">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="cda21-576">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="cda21-576">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="cda21-577">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="cda21-577">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="cda21-578">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="cda21-578">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="cda21-579">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="cda21-579">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="cda21-580">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="cda21-580">Added `--progress` flag</span></span>
* <span data-ttu-id="cda21-581">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="cda21-581">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="cda21-582">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="cda21-582">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="cda21-583">IoT</span><span class="sxs-lookup"><span data-stu-id="cda21-583">IoT</span></span>

* <span data-ttu-id="cda21-584">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="cda21-584">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="cda21-585">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="cda21-585">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="cda21-586">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="cda21-586">Key vault</span></span>

* <span data-ttu-id="cda21-587">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="cda21-587">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="cda21-588">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="cda21-588">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="cda21-589">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="cda21-589">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="cda21-590">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="cda21-590">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="cda21-591">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="cda21-591">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="cda21-592">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="cda21-592">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="cda21-593">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="cda21-593">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="cda21-594">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="cda21-594">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="cda21-595">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="cda21-595">Lab</span></span>

* <span data-ttu-id="cda21-596">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="cda21-596">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="cda21-597">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="cda21-597">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="cda21-598">Supervisión</span><span class="sxs-lookup"><span data-stu-id="cda21-598">Monitor</span></span>

* <span data-ttu-id="cda21-599">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="cda21-599">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="cda21-600">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="cda21-600">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="cda21-601">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="cda21-601">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="cda21-602">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="cda21-602">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="cda21-603">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="cda21-603">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="cda21-604">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="cda21-604">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="cda21-605">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="cda21-605">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="cda21-606">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="cda21-606">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="cda21-607">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="cda21-607">`location` no longer required</span></span>
  * <span data-ttu-id="cda21-608">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="cda21-608">Add name and ID support for target</span></span>
  * <span data-ttu-id="cda21-609">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="cda21-609">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="cda21-610">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="cda21-610">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="cda21-611">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="cda21-611">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="cda21-612">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="cda21-612">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="cda21-613">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="cda21-613">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="cda21-614">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="cda21-614">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="cda21-615">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-615">Network</span></span>

* <span data-ttu-id="cda21-616">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="cda21-616">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="cda21-617">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-617">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="cda21-618">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="cda21-618">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="cda21-619">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="cda21-619">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="cda21-620">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-620">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="cda21-621">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="cda21-621">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="cda21-622">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="cda21-622">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="cda21-623">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="cda21-623">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="cda21-624">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="cda21-624">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="cda21-625">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="cda21-625">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="cda21-626">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="cda21-626">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="cda21-627">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="cda21-627">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="cda21-628">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="cda21-628">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="cda21-629">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-629">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="cda21-630">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-630">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="cda21-631">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-631">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="cda21-632">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="cda21-632">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="cda21-633">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="cda21-633">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="cda21-634">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-634">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="cda21-635">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-635">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="cda21-636">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-636">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="cda21-637">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="cda21-637">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="cda21-638">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="cda21-638">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="cda21-639">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="cda21-639">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="cda21-640">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="cda21-640">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="cda21-641">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="cda21-641">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="cda21-642">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="cda21-642">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="cda21-643">Perfil</span><span class="sxs-lookup"><span data-stu-id="cda21-643">Profile</span></span>

* <span data-ttu-id="cda21-644">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="cda21-644">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="cda21-645">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="cda21-645">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="cda21-646">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="cda21-646">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="cda21-647">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="cda21-647">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="cda21-648">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="cda21-648">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="cda21-649">RDBMS</span><span class="sxs-lookup"><span data-stu-id="cda21-649">RDBMS</span></span>

* <span data-ttu-id="cda21-650">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="cda21-650">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="cda21-651">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="cda21-651">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="cda21-652">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="cda21-652">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="cda21-653">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="cda21-653">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-654">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-654">Resource</span></span>

* <span data-ttu-id="cda21-655">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-655">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="cda21-656">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="cda21-656">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="cda21-657">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="cda21-657">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="cda21-658">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="cda21-658">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="cda21-659">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="cda21-659">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="cda21-660">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="cda21-660">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="cda21-661">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="cda21-661">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="cda21-662">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="cda21-662">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="cda21-663">Rol</span><span class="sxs-lookup"><span data-stu-id="cda21-663">Role</span></span>

* <span data-ttu-id="cda21-664">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="cda21-664">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="cda21-665">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="cda21-665">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="cda21-666">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="cda21-666">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="cda21-667">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="cda21-667">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="cda21-668">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="cda21-668">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cda21-669">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cda21-669">Service Fabric</span></span>
* <span data-ttu-id="cda21-670">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="cda21-670">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="cda21-671">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="cda21-671">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="cda21-672">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="cda21-672">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="cda21-673">SQL</span><span class="sxs-lookup"><span data-stu-id="cda21-673">SQL</span></span>

* <span data-ttu-id="cda21-674">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="cda21-674">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="cda21-675">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="cda21-675">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="cda21-676">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="cda21-676">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-677">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-677">Storage</span></span>

* <span data-ttu-id="cda21-678">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="cda21-678">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="cda21-679">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="cda21-679">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="cda21-680">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="cda21-680">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="cda21-681">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="cda21-681">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="cda21-682">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="cda21-682">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="cda21-683">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="cda21-683">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-684">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-684">VM</span></span>

* <span data-ttu-id="cda21-685">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="cda21-685">Support configuring nsg</span></span>
* <span data-ttu-id="cda21-686">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="cda21-686">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="cda21-687">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="cda21-687">Support managed service identities</span></span>
* <span data-ttu-id="cda21-688">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="cda21-688">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="cda21-689">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="cda21-689">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="cda21-690">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-690">May 10, 2017</span></span>

<span data-ttu-id="cda21-691">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="cda21-691">Version 2.0.6</span></span>

* <span data-ttu-id="cda21-692">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="cda21-692">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="cda21-693">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="cda21-693">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="cda21-694">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="cda21-694">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="cda21-695">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="cda21-695">Include Cognitive Services module.</span></span>
* <span data-ttu-id="cda21-696">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="cda21-696">Include Service Fabric module.</span></span>
* <span data-ttu-id="cda21-697">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="cda21-697">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="cda21-698">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="cda21-698">Add support for CDN commands.</span></span>
* <span data-ttu-id="cda21-699">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="cda21-699">Remove Container module.</span></span>
* <span data-ttu-id="cda21-700">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="cda21-700">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="cda21-701">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="cda21-701">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="cda21-702">Núcleo</span><span class="sxs-lookup"><span data-stu-id="cda21-702">Core</span></span>

* <span data-ttu-id="cda21-703">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="cda21-703">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="cda21-704">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="cda21-704">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="cda21-705">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="cda21-705">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="cda21-706">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="cda21-706">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="cda21-707">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="cda21-707">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="cda21-708">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="cda21-708">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="cda21-709">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="cda21-709">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="cda21-710">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="cda21-710">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="cda21-711">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="cda21-711">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="cda21-712">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="cda21-712">core: Improved performance</span></span>
* <span data-ttu-id="cda21-713">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="cda21-713">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="cda21-714">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="cda21-714">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-715">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-715">ACS</span></span>

* <span data-ttu-id="cda21-716">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="cda21-716">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="cda21-717">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="cda21-717">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="cda21-718">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="cda21-718">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="cda21-719">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="cda21-719">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-720">AppService</span><span class="sxs-lookup"><span data-stu-id="cda21-720">AppService</span></span>

* <span data-ttu-id="cda21-721">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="cda21-721">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="cda21-722">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="cda21-722">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="cda21-723">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="cda21-723">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="cda21-724">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="cda21-724">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="cda21-725">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="cda21-725">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="cda21-726">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="cda21-726">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="cda21-727">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="cda21-727">support slot swap with preview</span></span>
* <span data-ttu-id="cda21-728">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="cda21-728">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="cda21-729">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="cda21-729">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cda21-730">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="cda21-730">CosmosDB</span></span>

* <span data-ttu-id="cda21-731">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="cda21-731">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="cda21-732">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="cda21-732">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="cda21-733">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="cda21-733">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="cda21-734">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="cda21-734">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="cda21-735">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="cda21-735">Data Lake Analytics</span></span>

* <span data-ttu-id="cda21-736">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="cda21-736">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="cda21-737">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="cda21-737">Add support for new catalog item type: package.</span></span> <span data-ttu-id="cda21-738">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="cda21-738">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="cda21-739">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="cda21-739">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="cda21-740">Tabla</span><span class="sxs-lookup"><span data-stu-id="cda21-740">Table</span></span>
  * <span data-ttu-id="cda21-741">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="cda21-741">Table valued function</span></span>
  * <span data-ttu-id="cda21-742">Ver</span><span class="sxs-lookup"><span data-stu-id="cda21-742">View</span></span>
  * <span data-ttu-id="cda21-743">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="cda21-743">Table Statistics.</span></span> <span data-ttu-id="cda21-744">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="cda21-744">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="cda21-745">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="cda21-745">Data Lake Store</span></span>

* <span data-ttu-id="cda21-746">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="cda21-746">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="cda21-747">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="cda21-747">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="cda21-748">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="cda21-748">missed help for access show.</span></span> <span data-ttu-id="cda21-749">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="cda21-749">adding it.</span></span> <span data-ttu-id="cda21-750">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="cda21-750">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="cda21-751">Buscar</span><span class="sxs-lookup"><span data-stu-id="cda21-751">Find</span></span>

* <span data-ttu-id="cda21-752">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="cda21-752">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="cda21-753">KeyVault</span><span class="sxs-lookup"><span data-stu-id="cda21-753">KeyVault</span></span>

* <span data-ttu-id="cda21-754">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="cda21-754">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="cda21-755">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="cda21-755">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="cda21-756">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="cda21-756">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="cda21-757">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="cda21-757">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="cda21-758">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="cda21-758">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="cda21-759">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="cda21-759">Lab</span></span>

* <span data-ttu-id="cda21-760">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="cda21-760">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="cda21-761">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="cda21-761">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="cda21-762">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="cda21-762">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="cda21-763">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="cda21-763">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="cda21-764">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="cda21-764">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="cda21-765">Supervisión</span><span class="sxs-lookup"><span data-stu-id="cda21-765">Monitor</span></span>

* <span data-ttu-id="cda21-766">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="cda21-766">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="cda21-767">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="cda21-767">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="cda21-768">Red</span><span class="sxs-lookup"><span data-stu-id="cda21-768">Network</span></span>

* <span data-ttu-id="cda21-769">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="cda21-769">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="cda21-770">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="cda21-770">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="cda21-771">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="cda21-771">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="cda21-772">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="cda21-772">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="cda21-773">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="cda21-773">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="cda21-774">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="cda21-774">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="cda21-775">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="cda21-775">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="cda21-776">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="cda21-776">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="cda21-777">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="cda21-777">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="cda21-778">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="cda21-778">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="cda21-779">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="cda21-779">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="cda21-780">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="cda21-780">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="cda21-781">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="cda21-781">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="cda21-782">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="cda21-782">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="cda21-783">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="cda21-783">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="cda21-784">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="cda21-784">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="cda21-785">Perfil</span><span class="sxs-lookup"><span data-stu-id="cda21-785">Profile</span></span>

* <span data-ttu-id="cda21-786">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="cda21-786">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="cda21-787">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="cda21-787">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="cda21-788">Redis</span><span class="sxs-lookup"><span data-stu-id="cda21-788">Redis</span></span>

* <span data-ttu-id="cda21-789">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="cda21-789">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="cda21-790">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="cda21-790">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="cda21-791">Recurso</span><span class="sxs-lookup"><span data-stu-id="cda21-791">Resource</span></span>

* <span data-ttu-id="cda21-792">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="cda21-792">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="cda21-793">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="cda21-793">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="cda21-794">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="cda21-794">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="cda21-795">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="cda21-795">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="cda21-796">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="cda21-796">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="cda21-797">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="cda21-797">Add docs for az lock update.</span></span> <span data-ttu-id="cda21-798">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="cda21-798">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="cda21-799">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="cda21-799">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="cda21-800">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="cda21-800">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="cda21-801">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="cda21-801">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="cda21-802">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="cda21-802">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="cda21-803">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="cda21-803">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="cda21-804">Rol</span><span class="sxs-lookup"><span data-stu-id="cda21-804">Role</span></span>

* <span data-ttu-id="cda21-805">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="cda21-805">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="cda21-806">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="cda21-806">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="cda21-807">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="cda21-807">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="cda21-808">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="cda21-808">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="cda21-809">SQL</span><span class="sxs-lookup"><span data-stu-id="cda21-809">SQL</span></span>

* <span data-ttu-id="cda21-810">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="cda21-810">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="cda21-811">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="cda21-811">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="cda21-812">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-812">Storage</span></span>

* <span data-ttu-id="cda21-813">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="cda21-813">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="cda21-814">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="cda21-814">Add support for incremental blob copy</span></span>
* <span data-ttu-id="cda21-815">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="cda21-815">Add support for large block blob upload</span></span>
* <span data-ttu-id="cda21-816">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="cda21-816">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-817">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-817">VM</span></span>

* <span data-ttu-id="cda21-818">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="cda21-818">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="cda21-819">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="cda21-819">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="cda21-820">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="cda21-820">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="cda21-821">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="cda21-821">az vm/vmss disk</span></span>
  3. <span data-ttu-id="cda21-822">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="cda21-822">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="cda21-823">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="cda21-823">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="cda21-824">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="cda21-824">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="cda21-825">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-825">April 3, 2017</span></span>

<span data-ttu-id="cda21-826">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="cda21-826">Version 2.0.2</span></span>

<span data-ttu-id="cda21-827">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="cda21-827">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="cda21-828">Núcleo</span><span class="sxs-lookup"><span data-stu-id="cda21-828">Core</span></span>

* <span data-ttu-id="cda21-829">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="cda21-829">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="cda21-830">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="cda21-830">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="cda21-831">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="cda21-831">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="cda21-832">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="cda21-832">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="cda21-833">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="cda21-833">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="cda21-834">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="cda21-834">Add prompting for missing template parameters.</span></span> <span data-ttu-id="cda21-835">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="cda21-835">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="cda21-836">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="cda21-836">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="cda21-837">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="cda21-837">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="cda21-838">ACS</span><span class="sxs-lookup"><span data-stu-id="cda21-838">ACS</span></span>

* <span data-ttu-id="cda21-839">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="cda21-839">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="cda21-840">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="cda21-840">Add support for ssh key password prompting.</span></span> <span data-ttu-id="cda21-841">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="cda21-841">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="cda21-842">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="cda21-842">Add support for windows clusters.</span></span> <span data-ttu-id="cda21-843">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="cda21-843">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="cda21-844">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="cda21-844">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="cda21-845">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="cda21-845">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="cda21-846">AppService</span><span class="sxs-lookup"><span data-stu-id="cda21-846">AppService</span></span>

* <span data-ttu-id="cda21-847">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="cda21-847">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="cda21-848">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="cda21-848">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="cda21-849">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="cda21-849">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="cda21-850">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="cda21-850">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="cda21-851">DataLake</span><span class="sxs-lookup"><span data-stu-id="cda21-851">DataLake</span></span>

* <span data-ttu-id="cda21-852">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="cda21-852">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="cda21-853">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="cda21-853">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="cda21-854">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="cda21-854">DocuemntDB</span></span>

* <span data-ttu-id="cda21-855">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="cda21-855">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="cda21-856">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="cda21-856">VM</span></span>

* <span data-ttu-id="cda21-857">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="cda21-857">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="cda21-858">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="cda21-858">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="cda21-859">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="cda21-859">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="cda21-860">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="cda21-860">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="cda21-861">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="cda21-861">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="cda21-862">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="cda21-862">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="cda21-863">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="cda21-863">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="cda21-864">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="cda21-864">February 27, 2017</span></span>

<span data-ttu-id="cda21-865">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="cda21-865">Version 2.0.0</span></span>

<span data-ttu-id="cda21-866">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="cda21-866">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="cda21-867">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="cda21-867">General availability applies to these command modules:</span></span>
- <span data-ttu-id="cda21-868">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="cda21-868">Container Service (acs)</span></span>
- <span data-ttu-id="cda21-869">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="cda21-869">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="cda21-870">Redes</span><span class="sxs-lookup"><span data-stu-id="cda21-870">Networking</span></span>
- <span data-ttu-id="cda21-871">Storage</span><span class="sxs-lookup"><span data-stu-id="cda21-871">Storage</span></span>

<span data-ttu-id="cda21-872">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cda21-872">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="cda21-873">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="cda21-873">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="cda21-874">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="cda21-874">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="cda21-875">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="cda21-875">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="cda21-876">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="cda21-876">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="cda21-877">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="cda21-877">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="cda21-878">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="cda21-878">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="cda21-879">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="cda21-879">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="cda21-880">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="cda21-880">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="cda21-881">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="cda21-881">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="cda21-882">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="cda21-882">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="cda21-883">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="cda21-883">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="cda21-884">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="cda21-884">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="cda21-885">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="cda21-885">Provide feedback from the command line with the `az feedback` command.</span></span>

