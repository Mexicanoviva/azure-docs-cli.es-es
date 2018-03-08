---
title: "Notas de la versión de la CLI de Azure 2.0"
description: "Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0"
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 01078b7a3665f563f0a6b1d809c9a41f18d136d6
ms.sourcegitcommit: f3ab5da6019083ef2482b62c7355817e6170dcfb
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="dea7d-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="dea7d-103">Azure CLI 2.0 release notes</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="dea7d-104">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="dea7d-104">February 27, 2018</span></span>

<span data-ttu-id="dea7d-105">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="dea7d-105">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="dea7d-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-106">Core</span></span>

* <span data-ttu-id="dea7d-107">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="dea7d-107">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="dea7d-108">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="dea7d-108">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="dea7d-109">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="dea7d-109">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-110">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-110">ACS</span></span>

* <span data-ttu-id="dea7d-111">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="dea7d-111">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="dea7d-112">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="dea7d-112">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="dea7d-113">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="dea7d-113">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="dea7d-114">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="dea7d-114">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-115">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-115">Appservice</span></span>

* <span data-ttu-id="dea7d-116">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="dea7d-116">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="dea7d-117">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="dea7d-117">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="dea7d-118">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="dea7d-118">Cognitive Services</span></span>

* <span data-ttu-id="dea7d-119">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="dea7d-119">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="dea7d-120">Consumo</span><span class="sxs-lookup"><span data-stu-id="dea7d-120">Consumption</span></span>

* <span data-ttu-id="dea7d-121">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="dea7d-121">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="dea7d-122">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="dea7d-122">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="dea7d-123">Contenedor</span><span class="sxs-lookup"><span data-stu-id="dea7d-123">Container</span></span>

* <span data-ttu-id="dea7d-124">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="dea7d-124">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-125">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-125">Network</span></span>

* <span data-ttu-id="dea7d-126">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="dea7d-126">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-127">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-127">Resource</span></span>

* <span data-ttu-id="dea7d-128">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="dea7d-128">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="dea7d-129">Rol</span><span class="sxs-lookup"><span data-stu-id="dea7d-129">Role</span></span>

* <span data-ttu-id="dea7d-130">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="dea7d-130">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-131">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-131">SQL</span></span>

* <span data-ttu-id="dea7d-132">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="dea7d-132">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-133">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-133">Storage</span></span>

* <span data-ttu-id="dea7d-134">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-134">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-135">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-135">VM</span></span>

* <span data-ttu-id="dea7d-136">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="dea7d-136">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="dea7d-137">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="dea7d-137">February 13, 2018</span></span>

<span data-ttu-id="dea7d-138">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="dea7d-138">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="dea7d-139">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-139">Core</span></span>

* <span data-ttu-id="dea7d-140">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="dea7d-140">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-141">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-141">ACS</span></span>

* <span data-ttu-id="dea7d-142">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-142">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="dea7d-143">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-143">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="dea7d-144">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="dea7d-144">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="dea7d-145">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="dea7d-145">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="dea7d-146">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="dea7d-146">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="dea7d-147">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="dea7d-147">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="dea7d-148">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="dea7d-148">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="dea7d-149">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="dea7d-149">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-150">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-150">Appservice</span></span>

* <span data-ttu-id="dea7d-151">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="dea7d-151">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="dea7d-152">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="dea7d-152">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="dea7d-153">CDN</span><span class="sxs-lookup"><span data-stu-id="dea7d-153">CDN</span></span>

* <span data-ttu-id="dea7d-154">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-154">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="dea7d-155">Contenedor</span><span class="sxs-lookup"><span data-stu-id="dea7d-155">Container</span></span>

* <span data-ttu-id="dea7d-156">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="dea7d-156">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="dea7d-157">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="dea7d-157">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dea7d-158">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="dea7d-158">CosmosDB</span></span>

* <span data-ttu-id="dea7d-159">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="dea7d-159">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="dea7d-160">Extensión</span><span class="sxs-lookup"><span data-stu-id="dea7d-160">Extension</span></span>

* <span data-ttu-id="dea7d-161">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-161">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="dea7d-162">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-162">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="dea7d-163">Comentarios</span><span class="sxs-lookup"><span data-stu-id="dea7d-163">Feedback</span></span>

* <span data-ttu-id="dea7d-164">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="dea7d-164">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="dea7d-165">Interactive</span><span class="sxs-lookup"><span data-stu-id="dea7d-165">Interactive</span></span>

* <span data-ttu-id="dea7d-166">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="dea7d-166">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="dea7d-167">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="dea7d-167">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="dea7d-168">IoT</span><span class="sxs-lookup"><span data-stu-id="dea7d-168">IoT</span></span>

* <span data-ttu-id="dea7d-169">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-169">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="dea7d-170">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-170">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="dea7d-171">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-171">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="dea7d-172">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="dea7d-172">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="dea7d-173">Supervisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-173">Monitor</span></span>

* <span data-ttu-id="dea7d-174">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-174">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-175">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-175">Network</span></span>

* <span data-ttu-id="dea7d-176">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="dea7d-176">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="dea7d-177">Perfil</span><span class="sxs-lookup"><span data-stu-id="dea7d-177">Profile</span></span>

* <span data-ttu-id="dea7d-178">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="dea7d-178">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-179">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-179">Resource</span></span>

* <span data-ttu-id="dea7d-180">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="dea7d-180">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="dea7d-181">Rol</span><span class="sxs-lookup"><span data-stu-id="dea7d-181">Role</span></span>

* <span data-ttu-id="dea7d-182">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-182">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-183">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-183">SQL</span></span>

* <span data-ttu-id="dea7d-184">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-184">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="dea7d-185">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-185">Added `sql db rename`</span></span>
* <span data-ttu-id="dea7d-186">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="dea7d-186">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-187">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-187">Storage</span></span>

* <span data-ttu-id="dea7d-188">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="dea7d-188">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-189">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-189">VM</span></span>

* <span data-ttu-id="dea7d-190">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="dea7d-190">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="dea7d-191">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="dea7d-191">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="dea7d-192">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="dea7d-192">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="dea7d-193">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="dea7d-193">January 31, 2018</span></span>

<span data-ttu-id="dea7d-194">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="dea7d-194">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="dea7d-195">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-195">Core</span></span>

* <span data-ttu-id="dea7d-196">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="dea7d-196">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="dea7d-197">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="dea7d-197">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="dea7d-198">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="dea7d-198">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="dea7d-199">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="dea7d-199">Use `--verbose` to see</span></span>
* <span data-ttu-id="dea7d-200">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="dea7d-200">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-201">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-201">ACS</span></span>

* <span data-ttu-id="dea7d-202">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="dea7d-202">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="dea7d-203">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="dea7d-203">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-204">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-204">Appservice</span></span>

* <span data-ttu-id="dea7d-205">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="dea7d-205">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="dea7d-206">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="dea7d-206">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="dea7d-207">CDN</span><span class="sxs-lookup"><span data-stu-id="dea7d-207">CDN</span></span>

* <span data-ttu-id="dea7d-208">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-208">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dea7d-209">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="dea7d-209">CosmosDB</span></span>

* <span data-ttu-id="dea7d-210">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="dea7d-210">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="dea7d-211">Interactive</span><span class="sxs-lookup"><span data-stu-id="dea7d-211">Interactive</span></span>

* <span data-ttu-id="dea7d-212">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="dea7d-212">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-213">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-213">Network</span></span>

* <span data-ttu-id="dea7d-214">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-214">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="dea7d-215">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="dea7d-215">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="dea7d-216">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-216">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="dea7d-217">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-217">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="dea7d-218">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="dea7d-218">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="dea7d-219">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="dea7d-219">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="dea7d-220">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="dea7d-220">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="dea7d-221">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="dea7d-221">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="dea7d-222">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="dea7d-222">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="dea7d-223">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="dea7d-223">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="dea7d-224">Perfil</span><span class="sxs-lookup"><span data-stu-id="dea7d-224">Profile</span></span>

* <span data-ttu-id="dea7d-225">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="dea7d-225">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-226">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-226">Resource</span></span>

* <span data-ttu-id="dea7d-227">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="dea7d-227">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-228">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-228">Storage</span></span>

* <span data-ttu-id="dea7d-229">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="dea7d-229">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="dea7d-230">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="dea7d-230">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="dea7d-231">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="dea7d-231">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="dea7d-232">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-232">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="dea7d-233">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="dea7d-233">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-234">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-234">VM</span></span>

* <span data-ttu-id="dea7d-235">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="dea7d-235">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="dea7d-236">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="dea7d-236">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="dea7d-237">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="dea7d-237">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="dea7d-238">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-238">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="dea7d-239">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="dea7d-239">January 17, 2018</span></span>

<span data-ttu-id="dea7d-240">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="dea7d-240">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="dea7d-241">ACR</span><span class="sxs-lookup"><span data-stu-id="dea7d-241">ACR</span></span>

* <span data-ttu-id="dea7d-242">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="dea7d-242">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="dea7d-243">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="dea7d-243">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-244">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-244">ACS</span></span>

* <span data-ttu-id="dea7d-245">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="dea7d-245">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="dea7d-246">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="dea7d-246">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-247">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-247">Appservice</span></span>

* <span data-ttu-id="dea7d-248">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="dea7d-248">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="dea7d-249">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="dea7d-249">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="dea7d-250">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="dea7d-250">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="dea7d-251">Backup</span><span class="sxs-lookup"><span data-stu-id="dea7d-251">Backup</span></span>

* <span data-ttu-id="dea7d-252">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="dea7d-252">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="dea7d-253">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="dea7d-253">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="dea7d-254">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="dea7d-254">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="dea7d-255">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="dea7d-255">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="dea7d-256">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="dea7d-256">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="dea7d-257">Batch</span><span class="sxs-lookup"><span data-stu-id="dea7d-257">Batch</span></span>

* <span data-ttu-id="dea7d-258">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="dea7d-258">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="dea7d-259">Nube</span><span class="sxs-lookup"><span data-stu-id="dea7d-259">Cloud</span></span>

* <span data-ttu-id="dea7d-260">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="dea7d-260">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="dea7d-261">Consumo</span><span class="sxs-lookup"><span data-stu-id="dea7d-261">Consumption</span></span>

* <span data-ttu-id="dea7d-262">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="dea7d-262">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="dea7d-263">Event Grid</span><span class="sxs-lookup"><span data-stu-id="dea7d-263">Event Grid</span></span>

* <span data-ttu-id="dea7d-264">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="dea7d-264">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="dea7d-265">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="dea7d-265">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="dea7d-266">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-266">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="dea7d-267">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="dea7d-267">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="dea7d-268">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-268">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="dea7d-269">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-269">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="dea7d-270">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="dea7d-270">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="dea7d-271">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="dea7d-271">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="dea7d-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="dea7d-272">Interactive</span></span>

* <span data-ttu-id="dea7d-273">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="dea7d-273">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="dea7d-274">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="dea7d-274">Fixed errors on startup</span></span>
* <span data-ttu-id="dea7d-275">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="dea7d-275">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="dea7d-276">IoT</span><span class="sxs-lookup"><span data-stu-id="dea7d-276">IoT</span></span>

* <span data-ttu-id="dea7d-277">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="dea7d-277">Added support for device provisioning service</span></span>
* <span data-ttu-id="dea7d-278">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="dea7d-278">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="dea7d-279">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="dea7d-279">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="dea7d-280">Supervisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-280">Monitor</span></span>

* <span data-ttu-id="dea7d-281">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="dea7d-281">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="dea7d-282">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-282">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="dea7d-283">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="dea7d-283">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-284">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-284">Network</span></span>

* <span data-ttu-id="dea7d-285">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-285">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="dea7d-286">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-286">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="dea7d-287">Perfil</span><span class="sxs-lookup"><span data-stu-id="dea7d-287">Profile</span></span>

* <span data-ttu-id="dea7d-288">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="dea7d-288">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="dea7d-289">Rol</span><span class="sxs-lookup"><span data-stu-id="dea7d-289">Role</span></span>

* <span data-ttu-id="dea7d-290">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="dea7d-290">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="dea7d-291">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dea7d-291">Service Fabric</span></span>

* <span data-ttu-id="dea7d-292">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="dea7d-292">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="dea7d-293">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="dea7d-293">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-294">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-294">VM</span></span>

* <span data-ttu-id="dea7d-295">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="dea7d-295">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="dea7d-296">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado del `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="dea7d-296">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="dea7d-297">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="dea7d-297">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="dea7d-298">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="dea7d-298">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="dea7d-299">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="dea7d-299">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="dea7d-300">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-300">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="dea7d-301">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-301">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="dea7d-302">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="dea7d-302">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="dea7d-303">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-303">December 19, 2017</span></span>

<span data-ttu-id="dea7d-304">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="dea7d-304">Version 2.0.23</span></span>

* <span data-ttu-id="dea7d-305">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="dea7d-305">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="dea7d-306">Contenedor</span><span class="sxs-lookup"><span data-stu-id="dea7d-306">Container</span></span>

* <span data-ttu-id="dea7d-307">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="dea7d-307">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-308">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-308">Network</span></span>

* <span data-ttu-id="dea7d-309">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-309">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="dea7d-310">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-310">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-311">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-311">Storage</span></span>

* <span data-ttu-id="dea7d-312">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="dea7d-312">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-313">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-313">VM</span></span>

* <span data-ttu-id="dea7d-314">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="dea7d-314">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="dea7d-315">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-315">December 5, 2017</span></span>

<span data-ttu-id="dea7d-316">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="dea7d-316">Version 2.0.22</span></span>

* <span data-ttu-id="dea7d-317">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-317">Removed `az component` commands.</span></span> <span data-ttu-id="dea7d-318">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="dea7d-318">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="dea7d-319">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-319">Core</span></span>
* <span data-ttu-id="dea7d-320">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="dea7d-320">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="dea7d-321">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="dea7d-321">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-322">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-322">ACS</span></span>

* <span data-ttu-id="dea7d-323">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="dea7d-323">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="dea7d-324">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-324">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="dea7d-325">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="dea7d-325">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="dea7d-326">Advisor</span><span class="sxs-lookup"><span data-stu-id="dea7d-326">Advisor</span></span>

* <span data-ttu-id="dea7d-327">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="dea7d-327">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-328">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-328">Appservice</span></span>

* <span data-ttu-id="dea7d-329">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="dea7d-329">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="dea7d-330">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="dea7d-330">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="dea7d-331">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="dea7d-331">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="dea7d-332">Consumo</span><span class="sxs-lookup"><span data-stu-id="dea7d-332">Consumption</span></span>

* <span data-ttu-id="dea7d-333">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="dea7d-333">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="dea7d-334">Contenedor</span><span class="sxs-lookup"><span data-stu-id="dea7d-334">Container</span></span>

* <span data-ttu-id="dea7d-335">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="dea7d-335">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="dea7d-336">Supervisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-336">Monitor</span></span>

* <span data-ttu-id="dea7d-337">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="dea7d-337">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-338">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-338">Resource</span></span>

* <span data-ttu-id="dea7d-339">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="dea7d-339">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="dea7d-340">Rol</span><span class="sxs-lookup"><span data-stu-id="dea7d-340">Role</span></span>

* <span data-ttu-id="dea7d-341">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="dea7d-341">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="dea7d-342">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="dea7d-342">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="dea7d-343">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="dea7d-343">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-344">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-344">SQL</span></span>

* <span data-ttu-id="dea7d-345">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="dea7d-345">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="dea7d-346">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-346">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-347">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-347">VM</span></span>

* <span data-ttu-id="dea7d-348">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="dea7d-348">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="dea7d-349">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-349">November 14, 2017</span></span>

<span data-ttu-id="dea7d-350">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="dea7d-350">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="dea7d-351">ACR</span><span class="sxs-lookup"><span data-stu-id="dea7d-351">ACR</span></span>

* <span data-ttu-id="dea7d-352">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="dea7d-352">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="dea7d-353">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-353">ACS</span></span>

* <span data-ttu-id="dea7d-354">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="dea7d-354">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="dea7d-355">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-355">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="dea7d-356">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="dea7d-356">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="dea7d-357">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="dea7d-357">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="dea7d-358">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="dea7d-358">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-359">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-359">Appservice</span></span>

* <span data-ttu-id="dea7d-360">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="dea7d-360">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="dea7d-361">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="dea7d-361">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="dea7d-362">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="dea7d-362">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="dea7d-363">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="dea7d-363">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="dea7d-364">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="dea7d-364">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="dea7d-365">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="dea7d-365">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="dea7d-366">Batch</span><span class="sxs-lookup"><span data-stu-id="dea7d-366">Batch</span></span>

* <span data-ttu-id="dea7d-367">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="dea7d-367">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="dea7d-368">Batchai</span><span class="sxs-lookup"><span data-stu-id="dea7d-368">Batchai</span></span>

* <span data-ttu-id="dea7d-369">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-369">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="dea7d-370">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-370">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="dea7d-371">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="dea7d-371">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="dea7d-372">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-372">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="dea7d-373">Nube</span><span class="sxs-lookup"><span data-stu-id="dea7d-373">Cloud</span></span>

* <span data-ttu-id="dea7d-374">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="dea7d-374">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="dea7d-375">Contenedor</span><span class="sxs-lookup"><span data-stu-id="dea7d-375">Container</span></span>

* <span data-ttu-id="dea7d-376">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="dea7d-376">Added support to open multiple ports</span></span>
* <span data-ttu-id="dea7d-377">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="dea7d-377">Added container group restart policy</span></span>
* <span data-ttu-id="dea7d-378">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="dea7d-378">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="dea7d-379">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="dea7d-379">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="dea7d-380">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="dea7d-380">Data Lake Analytics</span></span>

* <span data-ttu-id="dea7d-381">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="dea7d-381">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="dea7d-382">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="dea7d-382">Data Lake Store</span></span>

* <span data-ttu-id="dea7d-383">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="dea7d-383">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="dea7d-384">Extensión</span><span class="sxs-lookup"><span data-stu-id="dea7d-384">Extension</span></span>

* <span data-ttu-id="dea7d-385">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="dea7d-385">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="dea7d-386">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="dea7d-386">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="dea7d-387">IoT</span><span class="sxs-lookup"><span data-stu-id="dea7d-387">IoT</span></span>

* <span data-ttu-id="dea7d-388">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="dea7d-388">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="dea7d-389">Supervisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-389">Monitor</span></span>

* <span data-ttu-id="dea7d-390">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-390">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-391">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-391">Network</span></span>

* <span data-ttu-id="dea7d-392">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="dea7d-392">Added support for CAA DNS records</span></span>
* <span data-ttu-id="dea7d-393">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-393">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="dea7d-394">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-394">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="dea7d-395">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="dea7d-395">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="dea7d-396">Reservations</span><span class="sxs-lookup"><span data-stu-id="dea7d-396">Reservations</span></span>

* <span data-ttu-id="dea7d-397">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="dea7d-397">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-398">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-398">Resource</span></span>

* <span data-ttu-id="dea7d-399">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-399">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-400">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-400">SQL</span></span>

* <span data-ttu-id="dea7d-401">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-401">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-402">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-402">Storage</span></span>

* <span data-ttu-id="dea7d-403">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="dea7d-403">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="dea7d-404">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="dea7d-404">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="dea7d-405">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="dea7d-405">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="dea7d-406">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="dea7d-406">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="dea7d-407">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-407">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="dea7d-408">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="dea7d-408">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="dea7d-409">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="dea7d-409">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-410">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-410">VM</span></span>

* <span data-ttu-id="dea7d-411">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="dea7d-411">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="dea7d-412">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="dea7d-412">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="dea7d-413">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="dea7d-413">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="dea7d-414">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-414">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="dea7d-415">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="dea7d-415">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="dea7d-416">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-416">October 24, 2017</span></span>

<span data-ttu-id="dea7d-417">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="dea7d-417">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="dea7d-418">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-418">Core</span></span>

* <span data-ttu-id="dea7d-419">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="dea7d-419">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="dea7d-420">ACR</span><span class="sxs-lookup"><span data-stu-id="dea7d-420">ACR</span></span>

* <span data-ttu-id="dea7d-421">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="dea7d-421">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="dea7d-422">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="dea7d-422">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="dea7d-423">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="dea7d-423">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-424">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-424">ACS</span></span>

* <span data-ttu-id="dea7d-425">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="dea7d-425">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="dea7d-426">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="dea7d-426">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-427">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-427">Appservice</span></span>

* <span data-ttu-id="dea7d-428">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="dea7d-428">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="dea7d-429">Componente</span><span class="sxs-lookup"><span data-stu-id="dea7d-429">Component</span></span>

* <span data-ttu-id="dea7d-430">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="dea7d-430">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="dea7d-431">Supervisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-431">Monitor</span></span>

* <span data-ttu-id="dea7d-432">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-432">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-433">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-433">Resource</span></span>

* <span data-ttu-id="dea7d-434">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="dea7d-434">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="dea7d-435">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="dea7d-435">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-436">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-436">VM</span></span>

* <span data-ttu-id="dea7d-437">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-437">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="dea7d-438">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-438">October 9, 2017</span></span>

<span data-ttu-id="dea7d-439">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="dea7d-439">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="dea7d-440">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-440">Core</span></span>

* <span data-ttu-id="dea7d-441">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="dea7d-441">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-442">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-442">Appservice</span></span>

* <span data-ttu-id="dea7d-443">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="dea7d-443">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="dea7d-444">Batch</span><span class="sxs-lookup"><span data-stu-id="dea7d-444">Batch</span></span>

* <span data-ttu-id="dea7d-445">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="dea7d-445">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="dea7d-446">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="dea7d-446">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="dea7d-447">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="dea7d-447">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="dea7d-448">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="dea7d-448">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="dea7d-449">Batchai</span><span class="sxs-lookup"><span data-stu-id="dea7d-449">Batchai</span></span>

* <span data-ttu-id="dea7d-450">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="dea7d-450">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="dea7d-451">Keyvault</span><span class="sxs-lookup"><span data-stu-id="dea7d-451">Keyvault</span></span>

* <span data-ttu-id="dea7d-452">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="dea7d-452">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="dea7d-453">(#4448)</span><span class="sxs-lookup"><span data-stu-id="dea7d-453">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="dea7d-454">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-454">Network</span></span>

* <span data-ttu-id="dea7d-455">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="dea7d-455">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="dea7d-456">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="dea7d-456">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-457">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-457">Resource</span></span>

* <span data-ttu-id="dea7d-458">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-458">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="dea7d-459">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="dea7d-459">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="dea7d-460">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="dea7d-460">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="dea7d-461">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-461">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-462">Sql</span><span class="sxs-lookup"><span data-stu-id="dea7d-462">Sql</span></span>

* <span data-ttu-id="dea7d-463">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="dea7d-463">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="dea7d-464">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="dea7d-464">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="dea7d-465">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="dea7d-465">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-466">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-466">Storage</span></span>

* <span data-ttu-id="dea7d-467">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="dea7d-467">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-468">Vm</span><span class="sxs-lookup"><span data-stu-id="dea7d-468">Vm</span></span>

* <span data-ttu-id="dea7d-469">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="dea7d-469">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="dea7d-470">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-470">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="dea7d-471">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="dea7d-471">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="dea7d-472">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-472">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="dea7d-473">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-473">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="dea7d-474">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-474">September 22, 2017</span></span>

<span data-ttu-id="dea7d-475">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="dea7d-475">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-476">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-476">Resource</span></span>

* <span data-ttu-id="dea7d-477">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="dea7d-477">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="dea7d-478">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="dea7d-478">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="dea7d-479">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-479">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="dea7d-480">[NUEVO CAMBIO] Se cambió el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="dea7d-480">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-481">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-481">Network</span></span>

* <span data-ttu-id="dea7d-482">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="dea7d-482">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="dea7d-483">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="dea7d-483">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="dea7d-484">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="dea7d-484">Added `asg` application security group commands</span></span>
* <span data-ttu-id="dea7d-485">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-485">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="dea7d-486">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-486">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="dea7d-487">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-487">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="dea7d-488">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-488">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-489">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-489">Storage</span></span>

* <span data-ttu-id="dea7d-490">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="dea7d-490">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="dea7d-491">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="dea7d-491">Eventgrid</span></span>

* <span data-ttu-id="dea7d-492">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="dea7d-492">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-493">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-493">SQL</span></span>

* <span data-ttu-id="dea7d-494">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="dea7d-494">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="dea7d-495">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="dea7d-495">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="dea7d-496">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-496">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="dea7d-497">Keyvault</span><span class="sxs-lookup"><span data-stu-id="dea7d-497">Keyvault</span></span>

* <span data-ttu-id="dea7d-498">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="dea7d-498">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-499">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-499">VM</span></span>

* <span data-ttu-id="dea7d-500">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-500">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="dea7d-501">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="dea7d-501">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="dea7d-502">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-502">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="dea7d-503">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="dea7d-503">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="dea7d-504">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="dea7d-504">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="dea7d-505">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="dea7d-505">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-506">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-506">ACS</span></span>

* <span data-ttu-id="dea7d-507">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-507">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-508">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-508">Appservice</span></span>

* <span data-ttu-id="dea7d-509">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="dea7d-509">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="dea7d-510">Backup</span><span class="sxs-lookup"><span data-stu-id="dea7d-510">Backup</span></span>

* <span data-ttu-id="dea7d-511">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="dea7d-511">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="dea7d-512">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-512">September 11, 2017</span></span>

<span data-ttu-id="dea7d-513">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="dea7d-513">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="dea7d-514">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-514">Core</span></span>

* <span data-ttu-id="dea7d-515">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="dea7d-515">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="dea7d-516">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="dea7d-516">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-517">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-517">Acs</span></span>

* <span data-ttu-id="dea7d-518">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-518">Added `acs list-locations` command</span></span>
* <span data-ttu-id="dea7d-519">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="dea7d-519">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-520">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-520">Appservice</span></span>

* <span data-ttu-id="dea7d-521">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="dea7d-521">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="dea7d-522">CDN</span><span class="sxs-lookup"><span data-stu-id="dea7d-522">CDN</span></span>

* <span data-ttu-id="dea7d-523">Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-523">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="dea7d-524">Extensión</span><span class="sxs-lookup"><span data-stu-id="dea7d-524">Extension</span></span>

* <span data-ttu-id="dea7d-525">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="dea7d-525">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="dea7d-526">Keyvault</span><span class="sxs-lookup"><span data-stu-id="dea7d-526">Keyvault</span></span>

* <span data-ttu-id="dea7d-527">Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-527">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-528">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-528">Network</span></span>

* <span data-ttu-id="dea7d-529">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-529">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="dea7d-530">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-530">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="dea7d-531">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-531">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="dea7d-532">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-532">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="dea7d-533">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-533">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-534">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-534">Resource</span></span>

* <span data-ttu-id="dea7d-535">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-535">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="dea7d-536">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-536">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="dea7d-537">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="dea7d-537">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="dea7d-538">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="dea7d-538">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-539">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-539">SQL</span></span>

* <span data-ttu-id="dea7d-540">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-540">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-541">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-541">VM</span></span>

* <span data-ttu-id="dea7d-542">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-542">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="dea7d-543">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="dea7d-543">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="dea7d-544">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-544">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="dea7d-545">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="dea7d-545">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="dea7d-546">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-546">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="dea7d-547">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-547">August 31, 2017</span></span>

<span data-ttu-id="dea7d-548">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="dea7d-548">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="dea7d-549">Keyvault</span><span class="sxs-lookup"><span data-stu-id="dea7d-549">Keyvault</span></span>

* <span data-ttu-id="dea7d-550">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-550">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="dea7d-551">Sf</span><span class="sxs-lookup"><span data-stu-id="dea7d-551">Sf</span></span>

* <span data-ttu-id="dea7d-552">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="dea7d-552">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-553">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-553">Storage</span></span>

* <span data-ttu-id="dea7d-554">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="dea7d-554">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="dea7d-555">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="dea7d-555">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="dea7d-556">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-556">August 28, 2017</span></span>

<span data-ttu-id="dea7d-557">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="dea7d-557">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="dea7d-558">CLI</span><span class="sxs-lookup"><span data-stu-id="dea7d-558">CLI</span></span>

* <span data-ttu-id="dea7d-559">Se agregó una nota legal a `--version`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-559">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-560">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-560">ACS</span></span>

* <span data-ttu-id="dea7d-561">Se corrigieron las regiones en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="dea7d-561">Corrected preview regions.</span></span>
* <span data-ttu-id="dea7d-562">Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.</span><span class="sxs-lookup"><span data-stu-id="dea7d-562">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="dea7d-563">Se optimizó la salida del comando acs.</span><span class="sxs-lookup"><span data-stu-id="dea7d-563">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-564">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-564">Appservice</span></span>

* <span data-ttu-id="dea7d-565">[NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-565">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="dea7d-566">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-566">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="dea7d-567">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-567">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="dea7d-568">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="dea7d-568">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="dea7d-569">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="dea7d-569">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="dea7d-570">IoT</span><span class="sxs-lookup"><span data-stu-id="dea7d-570">IoT</span></span>

* <span data-ttu-id="dea7d-571">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="dea7d-571">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-572">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-572">Network</span></span>

* <span data-ttu-id="dea7d-573">[NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-573">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="dea7d-574">[NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-574">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="dea7d-575">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-575">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="dea7d-576">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-576">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="dea7d-577">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-577">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="dea7d-578">Perfil</span><span class="sxs-lookup"><span data-stu-id="dea7d-578">Profile</span></span>

* <span data-ttu-id="dea7d-579">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="dea7d-579">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="dea7d-580">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dea7d-580">Service Fabric</span></span>

* <span data-ttu-id="dea7d-581">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="dea7d-581">Preview release</span></span>
* <span data-ttu-id="dea7d-582">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="dea7d-582">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="dea7d-583">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="dea7d-583">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="dea7d-584">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-584">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-585">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-585">Storage</span></span>

* <span data-ttu-id="dea7d-586">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="dea7d-586">Enabled setting blob tier</span></span>
* <span data-ttu-id="dea7d-587">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="dea7d-587">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="dea7d-588">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-588">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="dea7d-589">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="dea7d-589">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="dea7d-590">[NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-590">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="dea7d-591">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="dea7d-591">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-592">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-592">VM</span></span>

* <span data-ttu-id="dea7d-593">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-593">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="dea7d-594">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-594">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="dea7d-595">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-595">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="dea7d-596">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="dea7d-596">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="dea7d-597">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="dea7d-597">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="dea7d-598">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-598">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="dea7d-599">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-599">August 15, 2017</span></span>

<span data-ttu-id="dea7d-600">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="dea7d-600">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-601">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-601">ACS</span></span>

* <span data-ttu-id="dea7d-602">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="dea7d-602">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-603">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-603">Appservice</span></span>

* <span data-ttu-id="dea7d-604">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="dea7d-604">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="dea7d-605">Event Grid</span><span class="sxs-lookup"><span data-stu-id="dea7d-605">Event Grid</span></span>

* <span data-ttu-id="dea7d-606">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="dea7d-606">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="dea7d-607">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-607">August 11, 2017</span></span>

<span data-ttu-id="dea7d-608">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="dea7d-608">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-609">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-609">ACS</span></span>

* <span data-ttu-id="dea7d-610">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="dea7d-610">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="dea7d-611">Batch</span><span class="sxs-lookup"><span data-stu-id="dea7d-611">Batch</span></span>

* <span data-ttu-id="dea7d-612">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="dea7d-612">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="dea7d-613">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="dea7d-613">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="dea7d-614">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="dea7d-614">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="dea7d-615">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="dea7d-615">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="dea7d-616">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="dea7d-616">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="dea7d-617">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="dea7d-617">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="dea7d-618">Componente</span><span class="sxs-lookup"><span data-stu-id="dea7d-618">Component</span></span>

* <span data-ttu-id="dea7d-619">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="dea7d-619">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="dea7d-620">Contenedor</span><span class="sxs-lookup"><span data-stu-id="dea7d-620">Container</span></span>

* <span data-ttu-id="dea7d-621">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="dea7d-621">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="dea7d-622">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="dea7d-622">Data Lake Store</span></span>

* <span data-ttu-id="dea7d-623">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="dea7d-623">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="dea7d-624">Event Grid</span><span class="sxs-lookup"><span data-stu-id="dea7d-624">Event Grid</span></span>

* <span data-ttu-id="dea7d-625">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="dea7d-625">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-626">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-626">Network</span></span>

* <span data-ttu-id="dea7d-627">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="dea7d-627">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="dea7d-628">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-628">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="dea7d-629">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="dea7d-629">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="dea7d-630">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-630">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="dea7d-631">Perfil</span><span class="sxs-lookup"><span data-stu-id="dea7d-631">Profile</span></span>

* <span data-ttu-id="dea7d-632">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="dea7d-632">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-633">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-633">Storage</span></span>

* <span data-ttu-id="dea7d-634">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="dea7d-634">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-635">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-635">VM</span></span>

* <span data-ttu-id="dea7d-636">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="dea7d-636">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="dea7d-637">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-637">Exposed `list-skus` command</span></span>
* <span data-ttu-id="dea7d-638">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="dea7d-638">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="dea7d-639">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="dea7d-639">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="dea7d-640">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="dea7d-640">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="dea7d-641">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-641">July 28, 2017</span></span>

<span data-ttu-id="dea7d-642">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="dea7d-642">Version 2.0.12</span></span>

* <span data-ttu-id="dea7d-643">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="dea7d-643">Added container commands</span></span>
* <span data-ttu-id="dea7d-644">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="dea7d-644">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="dea7d-645">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-645">Core</span></span>

* <span data-ttu-id="dea7d-646">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="dea7d-646">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="dea7d-647">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="dea7d-647">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="dea7d-648">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="dea7d-648">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="dea7d-649">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="dea7d-649">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="dea7d-650">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="dea7d-650">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="dea7d-651">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="dea7d-651">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="dea7d-652">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="dea7d-652">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="dea7d-653">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="dea7d-653">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="dea7d-654">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="dea7d-654">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="dea7d-655">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="dea7d-655">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="dea7d-656">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="dea7d-656">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="dea7d-657">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="dea7d-657">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="dea7d-658">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-658">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="dea7d-659">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-659">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="dea7d-660">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="dea7d-660">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="dea7d-661">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="dea7d-661">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="dea7d-662">ACR</span><span class="sxs-lookup"><span data-stu-id="dea7d-662">ACR</span></span>

* <span data-ttu-id="dea7d-663">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="dea7d-663">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="dea7d-664">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="dea7d-664">Support SKU update for managed registries</span></span>
* <span data-ttu-id="dea7d-665">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-665">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="dea7d-666">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="dea7d-666">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="dea7d-667">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="dea7d-667">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="dea7d-668">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="dea7d-668">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-669">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-669">ACS</span></span>

* <span data-ttu-id="dea7d-670">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="dea7d-670">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-671">Appservice</span><span class="sxs-lookup"><span data-stu-id="dea7d-671">Appservice</span></span>

* <span data-ttu-id="dea7d-672">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="dea7d-672">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="dea7d-673">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="dea7d-673">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="dea7d-674">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-674">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="dea7d-675">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="dea7d-675">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="dea7d-676">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="dea7d-676">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="dea7d-677">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="dea7d-677">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="dea7d-678">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="dea7d-678">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="dea7d-679">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="dea7d-679">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="dea7d-680">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="dea7d-680">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="dea7d-681">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="dea7d-681">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="dea7d-682">Batch</span><span class="sxs-lookup"><span data-stu-id="dea7d-682">Batch</span></span>

* <span data-ttu-id="dea7d-683">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="dea7d-683">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="dea7d-684">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-684">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="dea7d-685">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-685">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="dea7d-686">CDN</span><span class="sxs-lookup"><span data-stu-id="dea7d-686">CDN</span></span>

* <span data-ttu-id="dea7d-687">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.</span><span class="sxs-lookup"><span data-stu-id="dea7d-687">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="dea7d-688">Nube</span><span class="sxs-lookup"><span data-stu-id="dea7d-688">Cloud</span></span>

* <span data-ttu-id="dea7d-689">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="dea7d-689">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="dea7d-690">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="dea7d-690">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="dea7d-691">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="dea7d-691">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="dea7d-692">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="dea7d-692">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="dea7d-693">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-693">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dea7d-694">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="dea7d-694">CosmosDB</span></span>

* <span data-ttu-id="dea7d-695">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="dea7d-695">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="dea7d-696">Se agregó compatibilidad para TTL predeterminado de colección.</span><span class="sxs-lookup"><span data-stu-id="dea7d-696">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="dea7d-697">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="dea7d-697">Data Lake Analytics</span></span>

* <span data-ttu-id="dea7d-698">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-698">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="dea7d-699">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-699">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="dea7d-700">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-700">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="dea7d-701">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="dea7d-701">Data Lake Store</span></span>

* <span data-ttu-id="dea7d-702">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-702">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="dea7d-703">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="dea7d-703">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="dea7d-704">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-704">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="dea7d-705">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="dea7d-705">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="dea7d-706">Interactive</span><span class="sxs-lookup"><span data-stu-id="dea7d-706">Interactive</span></span>

* <span data-ttu-id="dea7d-707">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="dea7d-707">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="dea7d-708">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-708">Increased test coverage</span></span>
* <span data-ttu-id="dea7d-709">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="dea7d-709">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="dea7d-710">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="dea7d-710">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="dea7d-711">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="dea7d-711">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="dea7d-712">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="dea7d-712">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="dea7d-713">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="dea7d-713">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="dea7d-714">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-714">Added `--progress` flag</span></span>
* <span data-ttu-id="dea7d-715">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="dea7d-715">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="dea7d-716">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="dea7d-716">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="dea7d-717">IoT</span><span class="sxs-lookup"><span data-stu-id="dea7d-717">IoT</span></span>

* <span data-ttu-id="dea7d-718">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="dea7d-718">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="dea7d-719">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="dea7d-719">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="dea7d-720">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="dea7d-720">Key vault</span></span>

* <span data-ttu-id="dea7d-721">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="dea7d-721">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="dea7d-722">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="dea7d-722">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="dea7d-723">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="dea7d-723">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="dea7d-724">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="dea7d-724">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="dea7d-725">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="dea7d-725">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="dea7d-726">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="dea7d-726">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="dea7d-727">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="dea7d-727">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="dea7d-728">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="dea7d-728">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="dea7d-729">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="dea7d-729">Lab</span></span>

* <span data-ttu-id="dea7d-730">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-730">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="dea7d-731">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-731">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="dea7d-732">Supervisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-732">Monitor</span></span>

* <span data-ttu-id="dea7d-733">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="dea7d-733">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="dea7d-734">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-734">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="dea7d-735">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-735">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="dea7d-736">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-736">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="dea7d-737">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-737">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="dea7d-738">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="dea7d-738">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="dea7d-739">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="dea7d-739">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="dea7d-740">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-740">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="dea7d-741">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="dea7d-741">`location` no longer required</span></span>
  * <span data-ttu-id="dea7d-742">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="dea7d-742">Add name and ID support for target</span></span>
  * <span data-ttu-id="dea7d-743">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-743">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="dea7d-744">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="dea7d-744">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="dea7d-745">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="dea7d-745">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="dea7d-746">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="dea7d-746">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="dea7d-747">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-747">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="dea7d-748">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="dea7d-748">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-749">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-749">Network</span></span>

* <span data-ttu-id="dea7d-750">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-750">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="dea7d-751">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-751">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="dea7d-752">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="dea7d-752">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="dea7d-753">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="dea7d-753">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="dea7d-754">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-754">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="dea7d-755">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-755">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="dea7d-756">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="dea7d-756">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="dea7d-757">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="dea7d-757">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="dea7d-758">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="dea7d-758">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="dea7d-759">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="dea7d-759">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="dea7d-760">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-760">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="dea7d-761">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-761">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="dea7d-762">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="dea7d-762">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="dea7d-763">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-763">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="dea7d-764">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-764">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="dea7d-765">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-765">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="dea7d-766">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="dea7d-766">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="dea7d-767">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-767">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="dea7d-768">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-768">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="dea7d-769">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-769">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="dea7d-770">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-770">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="dea7d-771">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-771">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="dea7d-772">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-772">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="dea7d-773">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="dea7d-773">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="dea7d-774">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="dea7d-774">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="dea7d-775">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="dea7d-775">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="dea7d-776">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="dea7d-776">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="dea7d-777">Perfil</span><span class="sxs-lookup"><span data-stu-id="dea7d-777">Profile</span></span>

* <span data-ttu-id="dea7d-778">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="dea7d-778">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="dea7d-779">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="dea7d-779">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="dea7d-780">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="dea7d-780">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="dea7d-781">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="dea7d-781">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="dea7d-782">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="dea7d-782">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="dea7d-783">RDBMS</span><span class="sxs-lookup"><span data-stu-id="dea7d-783">RDBMS</span></span>

* <span data-ttu-id="dea7d-784">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="dea7d-784">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="dea7d-785">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="dea7d-785">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="dea7d-786">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="dea7d-786">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="dea7d-787">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="dea7d-787">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-788">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-788">Resource</span></span>

* <span data-ttu-id="dea7d-789">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-789">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="dea7d-790">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-790">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="dea7d-791">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-791">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="dea7d-792">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-792">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="dea7d-793">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="dea7d-793">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="dea7d-794">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-794">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="dea7d-795">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="dea7d-795">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="dea7d-796">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-796">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="dea7d-797">Rol</span><span class="sxs-lookup"><span data-stu-id="dea7d-797">Role</span></span>

* <span data-ttu-id="dea7d-798">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="dea7d-798">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="dea7d-799">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="dea7d-799">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="dea7d-800">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-800">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="dea7d-801">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-801">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="dea7d-802">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-802">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="dea7d-803">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dea7d-803">Service Fabric</span></span>
* <span data-ttu-id="dea7d-804">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="dea7d-804">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="dea7d-805">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="dea7d-805">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="dea7d-806">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="dea7d-806">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-807">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-807">SQL</span></span>

* <span data-ttu-id="dea7d-808">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="dea7d-808">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="dea7d-809">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-809">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="dea7d-810">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-810">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-811">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-811">Storage</span></span>

* <span data-ttu-id="dea7d-812">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="dea7d-812">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="dea7d-813">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="dea7d-813">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="dea7d-814">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="dea7d-814">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="dea7d-815">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="dea7d-815">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="dea7d-816">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="dea7d-816">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="dea7d-817">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="dea7d-817">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-818">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-818">VM</span></span>

* <span data-ttu-id="dea7d-819">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="dea7d-819">Support configuring nsg</span></span>
* <span data-ttu-id="dea7d-820">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="dea7d-820">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="dea7d-821">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="dea7d-821">Support managed service identities</span></span>
* <span data-ttu-id="dea7d-822">Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-822">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="dea7d-823">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="dea7d-823">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="dea7d-824">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-824">May 10, 2017</span></span>

<span data-ttu-id="dea7d-825">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="dea7d-825">Version 2.0.6</span></span>

* <span data-ttu-id="dea7d-826">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="dea7d-826">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="dea7d-827">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="dea7d-827">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="dea7d-828">Se incluyen los módulos de Data Lake Analytics y Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="dea7d-828">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="dea7d-829">Se incluye el módulo de Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="dea7d-829">Include Cognitive Services module.</span></span>
* <span data-ttu-id="dea7d-830">Se incluye el módulo de Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="dea7d-830">Include Service Fabric module.</span></span>
* <span data-ttu-id="dea7d-831">Se incluye el módulo de Interactive (se cambia el nombre de az-shell).</span><span class="sxs-lookup"><span data-stu-id="dea7d-831">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="dea7d-832">Se agrega compatibilidad con los comandos de la red CDN.</span><span class="sxs-lookup"><span data-stu-id="dea7d-832">Add support for CDN commands.</span></span>
* <span data-ttu-id="dea7d-833">Se quita el módulo de Container.</span><span class="sxs-lookup"><span data-stu-id="dea7d-833">Remove Container module.</span></span>
* <span data-ttu-id="dea7d-834">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="dea7d-834">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="dea7d-835">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="dea7d-835">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="dea7d-836">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-836">Core</span></span>

* <span data-ttu-id="dea7d-837">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="dea7d-837">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="dea7d-838">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="dea7d-838">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="dea7d-839">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="dea7d-839">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="dea7d-840">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="dea7d-840">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="dea7d-841">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="dea7d-841">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="dea7d-842">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="dea7d-842">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="dea7d-843">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="dea7d-843">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="dea7d-844">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="dea7d-844">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="dea7d-845">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="dea7d-845">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="dea7d-846">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="dea7d-846">core: Improved performance</span></span>
* <span data-ttu-id="dea7d-847">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="dea7d-847">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="dea7d-848">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="dea7d-848">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-849">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-849">ACS</span></span>

* <span data-ttu-id="dea7d-850">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="dea7d-850">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="dea7d-851">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="dea7d-851">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="dea7d-852">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="dea7d-852">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="dea7d-853">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="dea7d-853">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-854">AppService</span><span class="sxs-lookup"><span data-stu-id="dea7d-854">AppService</span></span>

* <span data-ttu-id="dea7d-855">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="dea7d-855">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="dea7d-856">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="dea7d-856">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="dea7d-857">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="dea7d-857">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="dea7d-858">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="dea7d-858">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="dea7d-859">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="dea7d-859">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="dea7d-860">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="dea7d-860">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="dea7d-861">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="dea7d-861">support slot swap with preview</span></span>
* <span data-ttu-id="dea7d-862">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="dea7d-862">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="dea7d-863">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="dea7d-863">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dea7d-864">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="dea7d-864">CosmosDB</span></span>

* <span data-ttu-id="dea7d-865">Cambiar el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="dea7d-865">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="dea7d-866">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="dea7d-866">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="dea7d-867">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="dea7d-867">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="dea7d-868">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="dea7d-868">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="dea7d-869">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="dea7d-869">Data Lake Analytics</span></span>

* <span data-ttu-id="dea7d-870">Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error</span><span class="sxs-lookup"><span data-stu-id="dea7d-870">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="dea7d-871">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="dea7d-871">Add support for new catalog item type: package.</span></span> <span data-ttu-id="dea7d-872">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="dea7d-872">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="dea7d-873">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="dea7d-873">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="dea7d-874">Tabla</span><span class="sxs-lookup"><span data-stu-id="dea7d-874">Table</span></span>
  * <span data-ttu-id="dea7d-875">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="dea7d-875">Table valued function</span></span>
  * <span data-ttu-id="dea7d-876">Ver</span><span class="sxs-lookup"><span data-stu-id="dea7d-876">View</span></span>
  * <span data-ttu-id="dea7d-877">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="dea7d-877">Table Statistics.</span></span> <span data-ttu-id="dea7d-878">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="dea7d-878">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="dea7d-879">Almacén de Data Lake</span><span class="sxs-lookup"><span data-stu-id="dea7d-879">Data Lake Store</span></span>

* <span data-ttu-id="dea7d-880">Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.</span><span class="sxs-lookup"><span data-stu-id="dea7d-880">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="dea7d-881">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="dea7d-881">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="dea7d-882">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="dea7d-882">missed help for access show.</span></span> <span data-ttu-id="dea7d-883">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="dea7d-883">adding it.</span></span> <span data-ttu-id="dea7d-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="dea7d-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="dea7d-885">Buscar</span><span class="sxs-lookup"><span data-stu-id="dea7d-885">Find</span></span>

* <span data-ttu-id="dea7d-886">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="dea7d-886">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="dea7d-887">KeyVault</span><span class="sxs-lookup"><span data-stu-id="dea7d-887">KeyVault</span></span>

* <span data-ttu-id="dea7d-888">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="dea7d-888">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="dea7d-889">BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="dea7d-889">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="dea7d-890">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="dea7d-890">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="dea7d-891">Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".</span><span class="sxs-lookup"><span data-stu-id="dea7d-891">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="dea7d-892">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="dea7d-892">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="dea7d-893">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="dea7d-893">Lab</span></span>

* <span data-ttu-id="dea7d-894">Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="dea7d-894">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="dea7d-895">Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="dea7d-895">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="dea7d-896">Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="dea7d-896">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="dea7d-897">Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="dea7d-897">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="dea7d-898">Agregar comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="dea7d-898">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="dea7d-899">Supervisión</span><span class="sxs-lookup"><span data-stu-id="dea7d-899">Monitor</span></span>

* <span data-ttu-id="dea7d-900">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="dea7d-900">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="dea7d-901">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="dea7d-901">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="dea7d-902">Red</span><span class="sxs-lookup"><span data-stu-id="dea7d-902">Network</span></span>

* <span data-ttu-id="dea7d-903">Agregar comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="dea7d-903">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="dea7d-904">Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-904">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="dea7d-905">Agregar la compatibilidad del drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="dea7d-905">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="dea7d-906">Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="dea7d-906">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="dea7d-907">Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="dea7d-907">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="dea7d-908">Agregar compatibilidad para enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="dea7d-908">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="dea7d-909">Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="dea7d-909">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="dea7d-910">Agregar compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="dea7d-910">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="dea7d-911">Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="dea7d-911">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="dea7d-912">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="dea7d-912">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="dea7d-913">Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="dea7d-913">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="dea7d-914">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-914">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="dea7d-915">Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente</span><span class="sxs-lookup"><span data-stu-id="dea7d-915">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="dea7d-916">Corregir errores en `dns zone import` donde los registros no se han importado correctamente</span><span class="sxs-lookup"><span data-stu-id="dea7d-916">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="dea7d-917">Corregir errores donde `traffic-manager endpoint update` no ha funcionado</span><span class="sxs-lookup"><span data-stu-id="dea7d-917">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="dea7d-918">Agregar los comandos de versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="dea7d-918">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="dea7d-919">Perfil</span><span class="sxs-lookup"><span data-stu-id="dea7d-919">Profile</span></span>

* <span data-ttu-id="dea7d-920">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="dea7d-920">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="dea7d-921">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="dea7d-921">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="dea7d-922">Redis</span><span class="sxs-lookup"><span data-stu-id="dea7d-922">Redis</span></span>

* <span data-ttu-id="dea7d-923">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="dea7d-923">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="dea7d-924">Dejar de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="dea7d-924">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="dea7d-925">Recurso</span><span class="sxs-lookup"><span data-stu-id="dea7d-925">Resource</span></span>

* <span data-ttu-id="dea7d-926">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="dea7d-926">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="dea7d-927">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="dea7d-927">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="dea7d-928">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="dea7d-928">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="dea7d-929">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="dea7d-929">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="dea7d-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="dea7d-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="dea7d-931">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="dea7d-931">Add docs for az lock update.</span></span> <span data-ttu-id="dea7d-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="dea7d-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="dea7d-933">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="dea7d-933">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="dea7d-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="dea7d-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="dea7d-935">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="dea7d-935">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="dea7d-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="dea7d-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="dea7d-937">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="dea7d-937">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="dea7d-938">Rol</span><span class="sxs-lookup"><span data-stu-id="dea7d-938">Role</span></span>

* <span data-ttu-id="dea7d-939">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="dea7d-939">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="dea7d-940">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="dea7d-940">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="dea7d-941">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="dea7d-941">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="dea7d-942">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="dea7d-942">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="dea7d-943">SQL</span><span class="sxs-lookup"><span data-stu-id="dea7d-943">SQL</span></span>

* <span data-ttu-id="dea7d-944">Agregar los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="dea7d-944">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="dea7d-945">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="dea7d-945">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="dea7d-946">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-946">Storage</span></span>

* <span data-ttu-id="dea7d-947">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="dea7d-947">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="dea7d-948">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="dea7d-948">Add support for incremental blob copy</span></span>
* <span data-ttu-id="dea7d-949">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="dea7d-949">Add support for large block blob upload</span></span>
* <span data-ttu-id="dea7d-950">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="dea7d-950">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-951">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-951">VM</span></span>

* <span data-ttu-id="dea7d-952">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="dea7d-952">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="dea7d-953">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="dea7d-953">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="dea7d-954">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="dea7d-954">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="dea7d-955">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="dea7d-955">az vm/vmss disk</span></span>
  3. <span data-ttu-id="dea7d-956">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="dea7d-956">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="dea7d-957">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="dea7d-957">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="dea7d-958">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="dea7d-958">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="dea7d-959">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-959">April 3, 2017</span></span>

<span data-ttu-id="dea7d-960">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="dea7d-960">Version 2.0.2</span></span>

<span data-ttu-id="dea7d-961">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.</span><span class="sxs-lookup"><span data-stu-id="dea7d-961">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="dea7d-962">Núcleo</span><span class="sxs-lookup"><span data-stu-id="dea7d-962">Core</span></span>

* <span data-ttu-id="dea7d-963">Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.</span><span class="sxs-lookup"><span data-stu-id="dea7d-963">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="dea7d-964">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="dea7d-964">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="dea7d-965">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="dea7d-965">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="dea7d-966">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="dea7d-966">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="dea7d-967">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="dea7d-967">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="dea7d-968">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="dea7d-968">Add prompting for missing template parameters.</span></span> <span data-ttu-id="dea7d-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="dea7d-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="dea7d-970">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="dea7d-970">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="dea7d-971">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="dea7d-971">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="dea7d-972">ACS</span><span class="sxs-lookup"><span data-stu-id="dea7d-972">ACS</span></span>

* <span data-ttu-id="dea7d-973">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="dea7d-973">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="dea7d-974">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="dea7d-974">Add support for ssh key password prompting.</span></span> <span data-ttu-id="dea7d-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="dea7d-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="dea7d-976">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="dea7d-976">Add support for windows clusters.</span></span> <span data-ttu-id="dea7d-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="dea7d-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="dea7d-978">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="dea7d-978">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="dea7d-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="dea7d-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="dea7d-980">AppService</span><span class="sxs-lookup"><span data-stu-id="dea7d-980">AppService</span></span>

* <span data-ttu-id="dea7d-981">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="dea7d-981">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="dea7d-982">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="dea7d-982">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="dea7d-983">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="dea7d-983">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="dea7d-984">AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="dea7d-984">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="dea7d-985">DataLake</span><span class="sxs-lookup"><span data-stu-id="dea7d-985">DataLake</span></span>

* <span data-ttu-id="dea7d-986">Versión inicial del módulo de Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="dea7d-986">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="dea7d-987">Versión inicial del módulo de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="dea7d-987">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="dea7d-988">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="dea7d-988">DocuemntDB</span></span>

* <span data-ttu-id="dea7d-989">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="dea7d-989">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="dea7d-990">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="dea7d-990">VM</span></span>

* <span data-ttu-id="dea7d-991">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="dea7d-991">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="dea7d-992">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="dea7d-992">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="dea7d-993">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="dea7d-993">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="dea7d-994">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="dea7d-994">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="dea7d-995">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="dea7d-995">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="dea7d-996">Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="dea7d-996">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="dea7d-997">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="dea7d-997">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="dea7d-998">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="dea7d-998">February 27, 2017</span></span>

<span data-ttu-id="dea7d-999">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="dea7d-999">Version 2.0.0</span></span>

<span data-ttu-id="dea7d-1000">La CLI de Azure 2.0 es la primera versión con disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1000">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="dea7d-1001">La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="dea7d-1001">General availability applies to these command modules:</span></span>
- <span data-ttu-id="dea7d-1002">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="dea7d-1002">Container Service (acs)</span></span>
- <span data-ttu-id="dea7d-1003">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="dea7d-1003">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="dea7d-1004">Redes</span><span class="sxs-lookup"><span data-stu-id="dea7d-1004">Networking</span></span>
- <span data-ttu-id="dea7d-1005">Storage</span><span class="sxs-lookup"><span data-stu-id="dea7d-1005">Storage</span></span>

<span data-ttu-id="dea7d-1006">Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1006">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="dea7d-1007">Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="dea7d-1007">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="dea7d-1008">Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1008">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="dea7d-1009">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1009">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="dea7d-1010">Para comprobar la versión de la CLI, use `az --version`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1010">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="dea7d-1011">El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1011">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="dea7d-1012">Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="dea7d-1012">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="dea7d-1013">Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1013">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="dea7d-1014">También tenemos versiones preliminares nocturnas de la CLI.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1014">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="dea7d-1015">Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="dea7d-1015">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="dea7d-1016">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="dea7d-1016">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="dea7d-1017">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="dea7d-1017">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="dea7d-1018">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="dea7d-1018">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="dea7d-1019">Envíe comentarios desde la línea de comandos con el comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="dea7d-1019">Provide feedback from the command line with the `az feedback` command.</span></span>

